---
type: lieu
nom: Dunes Centrales
categorie: sous_region
lieu_parent: Dhar'Zulun
securite: Dangereux
tags: lieu
---

# Dunes Centrales

> [!infobox]+ carte
> ![[carte_placeholder.jpg|cover]]
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **Se trouve dans** | `$= dv.fileLink(dv.current().lieu_parent)` |
> | **Sécurité** | `$= dv.current().securite` |



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

- Le cœur du Dhar'Zulun : l'océan de dunes où vivent les **clans nomades orcs**, les marchands itinérants et leurs pistes. C'est ici que bat le cœur du lore du désert — le [[Glossaire#Le Prix du Sang - Code des Clans Nomades du Dhar'Zulun|Prix du Sang]], les [[Veilleurs d'Ocre]] et leur QG de la Faille d'Ocre, les clans [[Ertuk]] et [[Zarka]] héritiers du schisme des **Mok'Tharak**, et la cité sédentaire Zarka de [[Mokh'Zar]].

##  Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

- 

##  Points d'intérêt (Sous-lieux)
*(Si c'est une ville : les tavernes, temples, boutiques. Si c'est une région : les villages, ruines, etc.)*

```dataview
LIST
FROM #lieu
WHERE contains(lieu_parent, this.file.name)

```

---

##  Habitants et PNJ présents
*Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter.*

```dataview
TABLE faction AS "Faction", description AS "Description"
FROM #PNJ
WHERE contains(list(lieu), this.file.name)
SORT file.name ASC
```

## Impact du jeu sur le lieu
*(Raconter les éventuels changement qu'ont apportés les joueurs sur le lieu)*

