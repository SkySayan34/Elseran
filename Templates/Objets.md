<%*
let title = tp.file.title;  
if (title.startsWith("Sans titre") || title.startsWith("Untitled") || title === "Template Objet Magique") {  
	title = await tp.system.prompt("Nom de l'objet magique :");  
	await tp.file.rename(title);  
}

const type = await tp.system.suggester(["Arme", "Armure", "Objet merveilleux", "Potion", "Bâton", "Bague", "Collier", "Autre"],  
["Arme", "Armure", "Objet merveilleux", "Potion", "Bâton", "Bague", "Collier", "Autre"])

const rareté = await tp.system.suggester(["Commun", "Peu commun", "Rare", "Très rare", "Légendaire", "Artefact"],  
["Commun", "Peu commun", "Rare", "Très rare", "Légendaire", "Artefact"])

const sousCatégorie = await tp.system.prompt("Sous-catégorie (ex: Épée courte, Bouclier, Anneau de protection) :")

const niveau = await tp.system.prompt("Niveau (1-20) :")  
const requis = await tp.system.prompt("Requis (Classe/Niveau/Alignement/Autre, laisser vide si aucun) :")  
const attunement = await tp.system.suggester(["Oui", "Non"], ["Oui", "Non"])


tR += `---
type: objet_magique
nom: ${title}
rareté: ${rareté}
catégorie: ${type}
sous_catégorie: ${sousCatégorie}
niveau: ${niveau}
requis: ${requis}
attunement: ${attunement}
tags : objet
---

# ${title}

`;
-%>

> [!infobox]+ image
> ![[carte_placeholder.jpg|cover h small]]
> ###### Informations générales
> | | |
> |---|---|
> | **Type** | `$= dv.current().catégorie` |
> | **Rareté** | `$= dv.current().rareté` |
> | **Sous-catégorie** | `$= dv.current().sous_catégorie` |
> | **Niveau** | `$= dv.current().niveau`|
> | **Attunement** | `$= dv.current().attunement` |
> | **Requis** | `$= dv.current().requis` |
