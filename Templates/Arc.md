<%*
let title = tp.file.title;
if (title.startsWith("Sans titre") || title.startsWith("Untitled")  | title === "Template Arc") {
    title = await tp.system.prompt("Nom de l'arc :");
    await tp.file.rename(title);
}

const dateDebut = tp.file.creation_date("YYYY-MM-DD");
const campagne = await tp.system.prompt("Campagne ? : ")

tR += `---
type: arc
nom: ${title}
campagne: ${campagne}
description: 
statut: à venir
date_debut: ${dateDebut}
---

# 🌌 ${title}

`;
%>

> [!infobox]
> | | |
> |---|---|
> | **Campagne** | `$= dv.fileLink(dv.current().campagne)` |
> | **Statut** | `$= dv.current().statut` |


## 📜 **Résumé**

`$= dv.current(). description`

## Chapitres

```dataview
TABLE description AS "Description", statut AS "Statut", date_debut AS "Début"
FROM #chapitre
WHERE contains(arc, this.file.name)
SORT date_debut ASC
```

## Quêtes Associées

```dataview
TABLE description AS "Description", statut AS "Statut", priorité AS "Priorité"
FROM #quête
WHERE contains(arc, this.file.name)
SORT priorité DESC, date_debut ASC
```
## Sessions :

```dataview
LIST
FROM #session
WHERE contains(arc, this.file.name)
SORT file.name DESC
```