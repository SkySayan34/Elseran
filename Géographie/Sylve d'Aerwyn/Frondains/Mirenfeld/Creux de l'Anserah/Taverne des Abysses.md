---
type: lieu
nom: Taverne des Abysses
categorie: location_precise
lieu_parent: Creux de l'Anserah
securite: Normale
tags: lieu
---

# Taverne des Abysses

> [!infobox]+ carte
> ![[Géographie/Images Library/Taverne des Abysses.jpg]]
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **Se trouve dans** | `$= dv.fileLink(dv.current().lieu_parent)` |
> | **Sécurité** | `$= dv.current().securite` |


##  Description générale
*(Écris ici l'ambiance visuelle, l'architecture, le climat ou la première impression des joueurs en arrivant)*

- Un ancien entrepôt relooké en cabaret macabre : fausses toiles d'araignées, serveurs grimés, fumée épaisse, nobles en costume qui boivent du vin rouge "sang de dryade"

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

```dataview
LIST
FROM #session 
WHERE contains(file.outlinks, this.file.link)
```
