---
type: faction
nom: Ordre Impérial de la Lumière
categorie: Religion
quartier_general: "[[Cathédrale de la Lumière]]"
dirigeant:
alignement: LM
influence: Normale
cree_le: 2026-06-15
---

# 🛡️ Organisation : Ordre Impérial de la Lumière

> [!infobox]+ blason
> ![[blason_placeholder.jpg|cover]]
> ###### Fiche d'identité
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **QG Principal** | `$= dv.current().quartier_general` |
> | **Dirigeant** | `$= dv.current().dirigeant` |
> | **Influence** | `$= dv.current().influence` |

## 👁️ Présentation & Philosophie
* **Devise / Dicton :** *«  »*
* **Doctrine / Objectif :** 
* **Ressources & Moyens :** *(Richesse, armée, magie, réseau d'espionnage...)*

- 

## 📜 Histoire & Secrets
*(Les origines de la faction, ses anciens dirigeants, ses rivalités historiques et ce qu'elle cache au grand public)*

- 

## 🧭 Relations Extérieures
* **Alliés :** 
* **Rivalités / Ennemis :** 

---

## 🛠️ Registre des Membres (Dataview)

### 👥 Membres et Affiliés (PJ & PNJ)
*Cette liste est automatique. Elle utilise la méthode textuelle "blindée" pour trouver tous les PNJ et PJ dont la propriété `faction` contient le nom de cette note.*

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
WHERE contains(list(faction), this.file.name) and (contains(type, "PNJ") or contains(type, "PJ"))
SORT file.name ASC
```
### 📋 Objectifs & Quêtes en cours

_Les missions confiées par cette faction ou les intrigues qui la visent directement._

```dataview
TABLE donneur_de_quete AS "Donneur", statut AS "Statut"
WHERE contains(string(faction), string(this.file.name)) AND lower(type) = "quete"
```
