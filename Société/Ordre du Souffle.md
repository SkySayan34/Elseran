---
type: faction
nom: Ordre du Souffle
categorie: Guilde
quartier_general: "[[Auberge du Chêne Doré]]"
dirigeant: "[[Zéphirae Anemoi]]"
alignement: LB
influence: Haute
cree_le: 2026-06-13
---

# 🛡️ Organisation : Ordre du Souffle

> [!infobox]+ blason
> ![[Ordre du Souffle.png|cover]]
> ###### Fiche d'identité
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **QG Principal** | `$= dv.current().quartier_general` |
> | **Dirigeant** | `$= dv.current().dirigeant` |
> | **Influence** | `$= dv.current().influence` |

## 👁️ Présentation & Philosophie
* **Devise / Dicton :** *« Lorsque le souffle nous appellera, nous serons là. »*
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
TABLE groupe AS "Groupe / Rôle", description AS "Description", statut AS "Statut"
WHERE contains(string(faction), string(this.file.name)) and (contains(type, "PNJ") or contains(type, "PJ"))
SORT file.name ASC
```
### 📋 Objectifs & Quêtes en cours

_Les missions confiées par cette faction ou les intrigues qui la visent directement._

```dataview
TABLE donneur_de_quete AS "Donneur", statut AS "Statut"
WHERE contains(string(faction), string(this.file.name)) AND lower(type) = "quete"
```
