<%*
// Un petit prompt Templater pour nommer ta note proprement à la création
let title = tp.file.title;
if (title.startsWith("Sans titre") || title.startsWith("Untitled") || title === "Template PNJ") {
    title = await tp.system.prompt("Nom du PNJ :");
    await tp.file.rename(title);
}

const statut = await tp.system.suggester(["Vivant","Mort","Disparu","Inconnu"],["Vivant","Mort","Disparu","Inconnu"])
const faction = await tp.system.prompt("Quel Faction ?")
const fonction = await tp.system.prompt("Quel Fonction ?")
const lieu = await tp.system.prompt("Où est-il ? (ex: Elseran/Sylve d'Aerwyn/Frondains/Mirenfeld/Croisée des Chemins/Auberge du Chêne Vert)")
const alignement = await tp.system.suggester(["LB","NB","CB","LN","N","CN","LM","NM","CM"],["LB","NB","CB","LN","N","CN","LM","NM","CM"])
const race = await tp.system.prompt("Quelle Race ?")
const classe = await tp.system.prompt("Quelle Classe ?")
const genre = await tp.system.suggester(["Homme","Femme","Non-Binaire"],["Homme","Femme","Non-Binaire"])
const description = await tp.system.prompt("Qui est-ce ?")

tR += `---
type: PNJ
statut: ${statut}
faction: ${faction}
fonction: ${fonction}
lieu: ${lieu}
alignement: ${alignement}
race: ${race}
classe: ${classe}
genre: ${genre}
description: ${description}
date_de_création: ${tp.file.creation_date("YYYY-MM-DD")}
---

# ${title}

> [!infobox]+ portrait
> ![[carte_placeholder.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | \`= link(this.faction)\` |
> | **Fonction** | \`= link(this.fonction)\` |
> | **Lieu** | \`= link(this.lieu)\` |
> | **Statut** | \`= this.statut\` |

`;
-%>

##  Description & Psychologie

* **Apparence :** 
* **Personnalité :** 
* **Motivation principale :** 
* **Secrets / Ce qu'il cache :** 

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- 

##  Relations & Connexions
* **Alliés :** 
* **Ennemis :** 
* **Réseau :** 

##  Coulisses du MJ
*Cette section se remplit automatiquement si d'autres notes (quêtes, sessions, rumeurs) mentionnent ce PNJ.*

### Quêtes liées
```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM "Chant des Cendres/Quêtes"
WHERE contains(file.links, this.file.link.path)
```


### Journal des rencontres
```dataview
LIST
FROM "Chant des Cendres/Sessions"
WHERE contains(file.outlinks, this.file.link.path)
SORT file.ctime DESC
```
