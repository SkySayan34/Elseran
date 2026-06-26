---
type: chapitre
nom: Danse Macabre
arc: Mirenfeld
campagne: Chant des Cendres
world: Elseran
description: "\"[[Vox Ceneris]] sont missionnés par l'[[Ordre du Souffle]] d'enquêter sur des morts proche de la [[Taverne des Abysses]]\""
statut: En cours
date_debut: 2026-06-26
---

# 📖 Danse Macabre

> [!infobox]
> | | |
> |---|---|
> | **Arc** | `= this.arc ` |
> | **Campagne** | `= this.campagne ` |
> | **Statut** | `= this.statut ` |
> | **Début** | `= this.date_debut ` |

## 📜 **Résumé**

`= this.description `


## Sessions

```dataview
TABLE date AS "Date Réelle", game_date AS "Date In-Game", location AS "Lieu", characters AS "PJ"
FROM "${campagne}/Sessions"
WHERE contains(chapitre, this.file.name)
SORT date ASC
```

## Quêtes

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM "${campagne}/Quêtes"
WHERE contains(chapitre, this.file.name)
SORT statut ASC
```

## PNJ

```dataview
TABLE nom AS "Nom", faction AS "Faction"
FROM #PNJ OR "PNJ"
WHERE contains(file.outlinks, this.file.link)
SORT file.name ASC
```
