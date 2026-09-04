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

const dateCreation = tp.file.creation_date("YYYY-MM-DD")

tR += `---
type: objet_magique
nom: ${title}
rareté: ${rareté}
catégorie: ${type}
sous_catégorie: ${sousCatégorie}
niveau: ${niveau}
requis: ${requis}
attunement: ${attunement}
date_de_création: ${dateCreation}
---

# ${title}

> [!infobox]+ image
> ![[carte_placeholder.jpg|cover h small]]
> ###### Informations générales
> | | |
> |---|---|
> | **Type** | \`= this.catégorie \` |
> | **Rareté** | \`= this.rareté \` |
> | **Sous-catégorie** | \`= this.sous_catégorie \` |
> | **Niveau** | \`= this.niveau \` |
> | **Attunement** | \`= this.attunement \` |
> | **Requis** | \`= this.requis \` |

`;
-%>


