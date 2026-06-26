<%*
// Prompt Templater pour nommer la note à la création
let title = tp.file.title;
if (title.startsWith("Untitled") || title === "Template Faction") {
    title = await tp.system.prompt("Nom de la Faction / Groupe :");
    await tp.file.rename(title);
}
-%>
---
type: faction
nom: <% title %>
categorie:  # [Guilde / Cercle / Culte / Compagnie / Gouvernement]
quartier_general:  # [Lien ou nom du lieu principal, ex: "[[Géographie/Sylve d'Aerwyn/Mirenfeld/Mirenfeld]]"]
dirigeant:  # [Lien ou nom du PNJ à la tête du groupe]
alignement:  # [loyal bon, chaotique mauvais, etc.]
influence:  # [Totale / Haute / Modérée / Faible / Secrète]
cree_le: <% tp.file.creation_date("YYYY-MM-DD") %>
---

# 🛡️ Organisation : <% title %>

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
