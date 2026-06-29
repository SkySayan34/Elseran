<%*
let title = tp.file.title;
if (title.startsWith("Untitled")  | title === "Template Chapitre") {
    title = await tp.system.prompt("Nom du chapitre :");
    await tp.file.rename(title);
}

const description = await tp.system.prompt("Description courte :");
const statut = await tp.system.suggester(["En cours", "Terminé", "À venir"], ["En cours", "Terminé", "À venir"]);
const dateDebut = tp.file.creation_date("YYYY-MM-DD");
const campagne = await tp.system.suggester(["Chant des Cendres", "Contes en Elseran"], ["Chant des Cendres", "Contes en Elseran"]);
const arc = await tp.system.prompt("Nom de l'arc parent (ex: Arc 1 - Le Réveil des Cendres) :");
const region = await tp.system.suggester(["Sylve d'Aerwyn", "Thal'Myrrun", "Vhalarion", "Dhar'Zulun", "Khor'Telun"], ["Sylve d'Aerwyn", "Thal'Myrrun", "Vhalarion", "Dhar'Zulun", "Khor'Telun"])
const sous_region = await tp.system.prompt("Nom de la sous région :")
const location = await tp.system.prompt("Nom de la location (ex : Mirenfeld, Lethariel, ...) :")
const location_precise = await tp.system.prompt("Nom de la location précise (Quartier, bâtiment, ...) :")

tR += `---
type: chapitre
nom: ${title}
arc: ${arc}
campagne: ${campagne}
world: Elseran
region: ${region}
sous_region: ${sous_region}
location: ${location}
location_precise: ${location_precise}
description: "${description}"
statut: ${statut}
date_debut: ${dateDebut}
tag: #chapitre
---

# 📖 ${title}

> [!infobox]
> | | |
> |---|---|
> | **Arc** | \`= link(this.arc) \` |
> | **Campagne** | \`= link(this.campagne) \` |
> | **Statut** | \`= this.statut \` |
> | **Début** | \`= this.date_debut \` |
> | **Lieu** | \`= link(this.location_precise) \` |

## 📜 **Résumé**

\`= this.description \`
`;
%>

## Sessions

```dataview
TABLE date AS "Date Réelle", game_date AS "Date In-Game", location AS "Lieu", characters AS "PJ"
FROM #session
WHERE contains(chapitre, this.file.name)
SORT date ASC
```

## Quêtes

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM #quête 
WHERE contains(chapitre, this.file.name)
SORT statut ASC
```

## PNJ

```dataview
TABLE nom AS "Nom", faction AS "Faction", description AS "Description"
FROM #PNJ OR "PNJ"
WHERE contains(file.outlinks, this.file.link)
SORT file.name ASC
```
