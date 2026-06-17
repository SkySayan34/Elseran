---
tags:
  - elseran
  - lore/géographie
  - montagnes
type: lieu
nom: Monts d'Elseran
categorie: Région
parent: "[[Elseran]]"
population: Inconnue
factions_presentes:
securite: Non-civilisé
cree_le: 2026-06-06
derniere_modif: 2026-06-06
---

# 📍 Lieu : Monts d'Elseran

> [!infobox]+ carte
> ![[Monts d'Elseran.webp|cover]]
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **Se trouve dans** | `$= dv.current().parent` |
> | **Sécurité** | `$= dv.current().securite` |
> | **Population** | `$= dv.current().population` |

## 🗺️ Description générale
*(Écris ici l'ambiance visuelle, l'architecture, le climat ou la première impression des joueurs en arrivant)*

Les **Monts d'Elseran**, également appelés les **Hauts de Vhalûr** par les anciens peuples, forment une chaîne de montagnes monumentale coupant le continent d'[[Elseran]] du nord au sud. 

C'est dans ces hauteurs escarpées et enneigées, au nord de Khor'Thélûn, que le fleuve sacré de l'[[Anserah]] prend sa source avant de s'écouler pour nourrir la grande [[Sylve d'Aerwyn]].


## 📜 Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

- 

## 🏠 Points d'intérêt (Sous-lieux)
*(Si c'est une ville : les tavernes, temples, boutiques. Si c'est une région : les villages, ruines, etc.)*

* **Point d'intérêt 1 :** Description rapide.
* **Point d'intérêt 2 :** Description rapide.

---

## 🛠️ Recensement local (Dataview)

### 👥 Habitants et PNJ présents
*Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter.*

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
FROM #pnj or ""
WHERE lieu = this.file.link OR contains(lieu, this.file.link)
SORT file.name ASC
```
