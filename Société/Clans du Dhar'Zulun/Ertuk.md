---
type: faction
categorie: Clan
quartier_general:
dirigeant:
influence: Faible
cree_le: 2026-09-16
tags: société
---

# 🛡️ Organisation : Ertuk
> [!infobox]+ blason
> ![[carte_placeholder.jpg|cover]]
> ###### Fiche d'identité
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **QG Principal** | `$= dv.fileLink(dv.current().quartier_general)` |
> | **Dirigeant** | `$= dv.fileLink(dv.current().dirigeant)` |
> | **Influence** | `$= dv.current().influence` |


## 👁️ Présentation & Philosophie

* **Devise / Dicton :** *Par le sable nous naissons, par les poings nous mourrons*
* **Doctrine / Objectif :** Subsister en Dhar'Zulun
* **Ressources & Moyens :** *(Richesse, armée, magie, réseau d'espionnage...)*

- 

## 📜 Histoire & Secrets
*(Les origines de la faction, ses anciens dirigeants, ses rivalités historiques et ce qu'elle cache au grand public)*

- 

## 🧭 Relations Extérieures

* **Alliés :** 
* **Rivalités / Ennemis :** les autres [[Clans du Dhar'Zulun]].

---

## Registre des Membres

### 👥 Membres et Affiliés (PJ & PNJ)

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
FROM #PNJ AND #PJ
WHERE contains(list(faction), this.file.name)
SORT file.name ASC
```
