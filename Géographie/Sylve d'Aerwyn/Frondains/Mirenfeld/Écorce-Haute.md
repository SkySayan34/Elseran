---
type: lieu
nom: Écorce-Haute
categorie: Quartier
parent: "[[Mirenfeld]]"
population: "[[elfes]] [[gnomes]] [[halfelins]] [[humains]]"
factions_presentes: "[[Galavorn]] [[Aeriel]] [[Cercle Druidique]] [[Ordre du Souffle]]"
securite: Haute
cree_le: 2026-06-12
derniere_modif: 2026-06-12
---

# 📍 Lieu : Écorce-Haute

> [!infobox]+ carte
> ![[Ecorce-Haute.jpg|cover]]
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **Se trouve dans** | `$= dv.current().parent` |
> | **Sécurité** | `$= dv.current().securite` |
> | **Population** | `$= dv.current().population` |

## 🗺️ Description générale
*(Écris ici l'ambiance visuelle, l'architecture, le climat ou la première impression des joueurs en arrivant)*

- Le quartier noble de la Sylve. Une architecture aérienne et élégante, bâtie à flanc de canopée dans les branches d'arbres séculaires pour accueillir l'élite sylvestre et les dignitaires druidiques.

## 📜 Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

- 

## 🏠 Points d'intérêt (Sous-lieux)
*(Si c'est une ville : les tavernes, temples, boutiques. Si c'est une région : les villages, ruines, etc.)*

* 

---

## 🛠️ Recensement local (Dataview)

### 👥 Habitants et PNJ présents
*Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter.*

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
WHERE contains(list(lieu), this.file.name) and (contains(type, "PNJ") or contains(type, "PJ"))
SORT file.name ASC
```
