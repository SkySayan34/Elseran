---
type: lieu
nom: Test fils
categorie: sous_region
lieu_parent: Test origine
securite: Haute
date_creation: 2026-07-06
---

# Test fils

> [!infobox]+ carte
> ![[carte_placeholder.jpg|cover]]
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `= this.categorie ` |
> | **Se trouve dans** | `= link(this.lieu_parent) ` |
> | **Sécurité** | `= this.securite ` |


```leaflet
id: leaflet-map-<% tp.file.title %>
image: [[carte_placeholder.jpg]]
height: 500px
lat: 50
long: 50
minZoom: 1
maxZoom: 10
defaultZoom: 7
unit: meters
scale: 1
darkMode: false
```

## 🗺️ Description générale
*(Écris ici l'ambiance visuelle, l'architecture, le climat ou la première impression des joueurs en arrivant)*

- 

## 📜 Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

- 

## 🏠 Points d'intérêt (Sous-lieux)
*(Si c'est une ville : les tavernes, temples, boutiques. Si c'est une région : les villages, ruines, etc.)*

```dataview
LIST
where contains(type, "lieu") and contains(lieu_parent, this.file.name)

```

---

## 🛠️ Recensement local (Dataview)

### 👥 Habitants et PNJ présents
*Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter.*

```dataview
TABLE faction AS "Faction", description AS "Description"
WHERE contains(list(lieu), this.file.name) and (contains(type, "PNJ") or contains(type, "PJ"))
SORT file.name ASC
```
