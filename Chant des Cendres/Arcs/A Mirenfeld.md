---
type: arc
nom: A Mirenfeld
campagne: Chant des Cendres
world: Elseran
description: Les aventuriers arrivent à [[Mirenfeld]] où ils rencontreront l'[[Ordre du Souffle]]. Ils accomplissent quelques quêtes ici et découvrent l'histoire de la ville avant de repartir vers d'autres lieux
statut: En cours
date_debut: 2026-03-13
tags:
  - arc
---

# 🌌 A Mirenfeld

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
FROM #chapitre 
WHERE contains(arc, this.file.name)
SORT date_debut ASC
```

## Quêtes Associées

```dataview
TABLE description AS "Objectif", statut AS "Statut", priorité AS "Priorité"
FROM #quête 
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

