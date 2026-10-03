---
type: lieu
nom: La Serre
categorie: location_precise
lieu_parent: "[[Subracine]]"
securite: Dangereux
tags: lieu
---

# La Serre

> [!infobox]+ carte
> ![[QG des Voragine.jpg|cover]]
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **Se trouve dans** | `$= dv.fileLink(dv.current().lieu_parent)` |
> | **Sécurité** | `$= dv.current().securite` |

##  Description générale
*(L'ambiance visuelle, l'architecture, la première impression des joueurs en arrivant)*

- Une rotonde de verre et de bois noir suspendue au-dessus du néant liquide : l'ancienne **serre-bassin impériale** engloutie lors de la construction des quais du [[Le Rempart (Mirenfeld)|Rempart]], revendiquée et vitrée de neuf par la [[Voragine|Voragine]] — tout le verre est soufflé en sous-main par l'[[Éclat de Verre]].
- La paroi courbe, épaisse et légèrement inégale, plonge sur les **profondeurs de l'[[Anserah]]** : limon en suspension, colonnes de lumière lointaine, et les **racines noyées du [[Mir'Sylva]]** qui s'enroulent dans la pénombre — la guilde travaille littéralement au-dessus des racines du monde.
- À l'intérieur : passerelles de bois noir, table ronde des contrats, registres et coffres, lampe à huile de baleine dont la flamme se double dans le reflet du verre. On n'y parle jamais fort : **le verre porte la voix**.
- Le silence est celui de l'eau : aucun écho de la ville au-dessus, seulement le grondement sourd du courant et, parfois, une vibration lente dans les racines quand le fleuve « décide ».

##  Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

- Édifiée par les bâtisseurs impériaux comme serre d'acclimatation des plantes de la Sylve (bassin d'eau de l'Anserah inclut), elle fut **engloutie par un effondrement des quais** avant même d'être inaugurée — la Ville l'a rayée des registres, le fleuve l'a gardée.
- [[Morgath]], remonté du fond enfant, en a fait son siège : « ce que le fleuve avale lui revient ». C'est ici qu'a lieu l'initiation des **Fonds**, le « retour du fleuve » — dont Morgath ne commente jamais le déroulé.
- Secret : la **Voûte des Dettes**, l'archive de contrats de la guilde, y dort sous trois serrures — y compris le **contrat signé d'[[Ambroise de Valcourt]]** pour l'enlèvement de [[Naelwyn]].

---

##  Habitants et PNJ présents
*Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter.*

```dataview
TABLE faction AS "Faction", description AS "Description"
FROM #PNJ
WHERE contains(list(lieu), this.file.name)
SORT file.name ASC
```

##  Impact du jeu sur le lieu
*(Raconter les éventuels changements qu'ont apportés les joueurs sur le lieu)*

- *(à remplir après la Session « Plaider Coupable » : infiltration, libération de [[Naelwyn]], témoignage de Morgath...)*