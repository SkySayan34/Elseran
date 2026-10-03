---
type: chapitre
nom: Plaider Coupable
arc: A Mirenfeld
campagne: Chant des Cendres
description: Les PJ se voient convoquer en justice pour meurtres injustes. [[Naelwyn]] est capturé en otage par des mercenaires. La pression monte d'un cran.
statut: à venir
tags: chapitre
---

# 📖 Plaider Coupable


> [!infobox]
> | | |
> |---|---|
> | **Arc** | `$= dv.fileLink(dv.current().arc)` |
> | **Campagne** | `$= dv.fileLink(dv.current().campagne)` |
> | **Statut** | `$= dv.current().arc` |


## 📜 **Résumé**

`$= dv.current().description` 


## Sessions

```dataview
LIST
FROM #session 
WHERE contains(campagne, this.file.name)
SORT file.name DESC
```

## Quêtes

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM #quête
WHERE contains(chapitre, this.file.name)
SORT priorité DESC, date_debut ASC
```

