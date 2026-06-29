---
type: chapitre
nom: Danse Macabre
arc: A Mirenfeld
campagne: Chant des Cendres
world: Elseran
description: "\"[[Vox Ceneris]] sont missionnés par l'[[Ordre du Souffle]] d'enquêter sur des morts proche de la [[Taverne des Abysses]]\""
statut: En cours
date_debut: 2026-06-26
tags:
  - chapitre
region: Sylve d'Aerwyn
sous_region: Frondains
location: Mirenfeld
location_precise: Croisée des Chemins
---

# 📖 Danse Macabre

> [!infobox]
>   | | |
> |---|---|
> | **Arc** | `= link(this.arc)` |
> | **Campagne** | `= link(this.campagne)` |
> | **Statut** | `= this.statut` |
> | **Début** | `= this.date_debut` |
> | **Lieu** | `= link(this.location_precise)` |

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
FROM #quête
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
