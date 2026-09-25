---
type: faction
categorie: Groupe
quartier_general:
tags: société
---

# 🛡️ Groupe : Vox Cineris

> [!infobox]
> ###### Fiche d'identité
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **QG Principal** | `$= dv.fileLink(dv.current().quartier_general)` |
> | **Dirigeant** | `$= dv.fileLink(dv.current().dirigeant)` |
> | **Influence** | `$= dv.current().influence` |



## 📜 Histoire & Secrets
*(Les origines de la faction, ses anciens dirigeants, ses rivalités historiques et ce qu'elle cache au grand public)*

- 

## 🧭 Relations Extérieures

* **Alliés :** [[Société/Ordre du Souffle]]
* **Rivalités / Ennemis :** [[Culte du Néant]]

---

## Registre des Membres

### 👥 Membres et Affiliés (PJ & PNJ)
*Cette liste est automatique. Elle utilise la méthode textuelle "blindée" pour trouver tous les PNJ et PJ dont la propriété `faction` contient le nom de cette note.*

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
FROM #PNJ AND #PJ
WHERE contains(list(faction), this.file.name)
SORT file.name ASC
```
