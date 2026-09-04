<%*
let title = tp.file.title;
if (title.startsWith("Sans titre") || title.startsWith("Untitled")  | title === "Template Chapitre") {
    title = await tp.system.prompt("Nom du chapitre :");
    await tp.file.rename(title);
}

const dateDebut = tp.file.creation_date("YYYY-MM-DD");
const campagne = await tp.system.prompt("Campagne ? : ")
const arc = await tp.system.prompt("Nom de l'arc parent :")

tR += `---
type: chapitre
nom: ${title}
arc: ${arc}
campagne: ${campagne}
description: 
statut: à venir
date_debut: ${dateDebut}
---

# 📖 ${title}

> [!infobox]
> | | |
> |---|---|
> | **Arc** | \`= link(this.arc) \` |
> | **Campagne** | \`= link(this.campagne) \` |
> | **Statut** | \`= this.statut \` |
> | **Début** | \`= this.date_debut \` |

## 📜 **Résumé**

`;
%>

## Sessions

```dataview
LIST
FROM "${campagne}/Sessions"
WHERE contains(campagne, this.file.name)
SORT file.name DESC
```

## Quêtes

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM "${campagne}/Quêtes"
WHERE contains(chapitre, this.file.name)
SORT priorité DESC, date_debut ASC
```

