---
type: arc
nom: A Mirenfeld
campagne: Chant des Cendres
description: Les aventuriers arrivent à [[Mirenfeld]] où ils rencontreront l'[[Ordre du Souffle]]. Ils accomplissent quelques quêtes ici et découvrent l'histoire de la ville avant de repartir vers d'autres lieux
statut: En cours
date: 32-07-403
---

# 🌌 A Mirenfeld



> [!infobox]
> | | |
> |---|---|
> | **Campagne** | `$= dv.fileLink(dv.current().campagne)` |
> | **Statut** | `$= dv.current().statut` |
> | **Date** | `$= dv.fileLink(dv.current().date)`


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
