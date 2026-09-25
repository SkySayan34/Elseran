---
tags: société
type: faction
categorie: Cercle Druidique
quartier_general:
dirigeant: Druan Silme
influence: Faible
---

# 🛡️ Organisation : Cercle de Lir
> [!infobox]+ blason
> ![[Cercle de Lir.png|cover]]
> ###### Fiche d'identité
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **QG Principal** | `$= dv.fileLink(dv.current().quartier_general)` |
> | **Dirigeant** | `$= dv.fileLink(dv.current().dirigeant)` |
> | **Influence** | `$= dv.current().influence` |


## 👁️ Présentation & Philosophie

Le **Cercle de Lir** est un cercle druidique mineur d'[[Elseran]], principalement actif dans les zones de forte résonance sylvestre de la [[Sylve d'Aerwyn]]. 

Ses membres, appelés les druides du Souffle, consacrent leur existence à l'écoute et à la préservation du Souffle de vie. Ils pratiquent l'invocation par résonance pour entrer en communion avec [[Lir - Esprit du Souffle|Lir, l'Esprit du Souffle]], un esprit mineur de l'Air.

## 📜 Histoire & Secrets
*(Les origines de la faction, ses anciens dirigeants, ses rivalités historiques et ce qu'elle cache au grand public)*

- 

## 🧭 Relations Extérieures

* **Alliés :** 
* **Rivalités / Ennemis :** 

---

## Registre des Membres

### 👥 Membres et Affiliés (PJ & PNJ)
*Cette liste est automatique. Elle utilise la méthode textuelle "blindée" pour trouver tous les PNJ et PJ dont la propriété `faction` contient le nom de cette note.*

```dataview
TABLE fonction AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
FROM #PNJ OR #PJ
WHERE contains(faction, this.file.name)
SORT file.name ASC
```