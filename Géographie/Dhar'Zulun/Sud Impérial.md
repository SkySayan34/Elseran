---
type: lieu
nom: Sud Impérial
categorie: sous_region
lieu_parent: Dhar'Zulun
securite: Normale
tags: lieu
---

# Sud Impérial

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

- La partie sud du désert est **gérée par l'[[Empire Vhalarionnien]]**, qui y a établi une partie de sa civilisation — mais elle reste soumise à des **razzias régulières**, auxquelles participent activement les tribus nomades [[Zarka]] et leurs clans alliés.

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

