---
type: arc
nom: En route !
campagne: Chant des Cendres
world: Elseran
description: "Le début et la rencontre des aventuriers. Ils se rejoignent à [[Lethariel]], un petit village au sud des [[Frondains]]. Après cette rencontre ils feront route ensemble vers la capitale : [[Mirenfeld]]"
statut: Terminé
date_debut: 2025-11-29
---

# 🌌 En route !

> [!infobox]
> | | |
> |---|---|
> | **Campagne** | `= this.campagne ` |
> | **Statut** | `= this.statut ` |
> | **Début** | `= this.date_debut ` |

## 📜 **Résumé**

`= this.description `


## Chapitres

```dataview
TABLE description AS "Description", statut AS "Statut", date_debut AS "Début"
FROM "Chant des Cendres/Chapitres"
WHERE contains(arc, this.file.name)
SORT date_debut ASC
```

## Quêtes Associées

```dataview
TABLE description AS "Objectif", statut AS "Statut", priorité AS "Priorité"
FROM "Chant des Cendres/04_Quêtes"
WHERE contains(arc, this.file.name)
SORT priorité DESC, date_debut ASC
```

## PNJ impliqués

```dataview
TABLE nom AS "Nom", faction AS "Faction", fonction AS "Rôle"
FROM #PNJ OR "PNJ"
WHERE contains(file.outlinks, this.file.link) OR contains(quêtes, this.file.name)
SORT file.name ASC
```

## Lieux Principaux

```dataview
LIST
FROM #lieu OR "Géographie"
WHERE contains(file.outlinks, this.file.link)
SORT file.name ASC
```

