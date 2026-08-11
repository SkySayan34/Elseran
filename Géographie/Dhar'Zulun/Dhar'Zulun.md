---
type: lieu
nom: Dhar'Zulun
categorie: region
lieu_parent: Elseran
securite: Dangereux
date_creation: 2026-08-11
---

# Dhar'Zulun

> [!infobox]+ carte
> ![[carte_placeholder.jpg|cover]]
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `= this.categorie ` |
> | **Se trouve dans** | `= link(this.lieu_parent) ` |
> | **Sécurité** | `= this.securite ` |


```leaflet
id: leaflet-map-${title}
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

##  Description générale
*(Écris ici l'ambiance visuelle, l'architecture, le climat ou la première impression des joueurs en arrivant)*

- Le Dhar'Zulun est un grand désert chaud. Les dunes s'étalent à perte de vue. On y trouve quelques peuples nomades, très peu de grandes villes ou cités. Les guerres entre clans sont quotidiennes. La plupart des peuples vivent la nuit ou en souterrain.

##  Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

- Invasion vhalarionnienne par le sud est dans le passé et par la mer, mais qui n'a duré que quelques temps dû au climat aride et au peu de ressources que cela apportait par rapport à ce que ça leur coûtait. 

##  Points d'intérêt (Sous-lieux)
*(Si c'est une ville : les tavernes, temples, boutiques. Si c'est une région : les villages, ruines, etc.)*
```dataview
LIST
where contains(type, "lieu") and contains(lieu_parent, this.file.name)

```

---

##  Habitants et PNJ présents
*Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter.*

```dataview
TABLE faction AS "Faction", description AS "Description"
WHERE contains(list(lieu), this.file.name) and (contains(type, "PNJ") or contains(type, "PJ"))
SORT file.name ASC
```
