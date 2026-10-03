---
type: lieu
nom: Athenaeum de Myrrha
categorie: location_precise
lieu_parent: "[[Anneau des Maîtres]]"
securite: Normale
tags: lieu
---

# Athenaeum de Myrrha

> [!infobox]+ carte
> ![[Athenaeum de Myrrha.jpg|cover]]
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **Se trouve dans** | `$= dv.fileLink(dv.current().lieu_parent)` |
> | **Sécurité** | `$= dv.current().securite` |

##  Description générale
*(L'ambiance visuelle, l'architecture, la première impression des joueurs en arrivant)*

- Une bibliothèque monumentale et un sanctuaire d'étude dédié à [[Myrrha]], déesse fondatrice du savoir et de la magie : le cœur de la [[Cour des Échos]] et le coffre-mémoire du [[Serment des Racines]].
- L'architecture entrelace la pierre impériale et le vivant : colonnes de marbre blanc enserrées par des racines du [[Mir'Sylva]] qui montent jusqu'aux voûtes et **poussent elles-mêmes les rayonnages** — la forêt est le mobilier, le marbre est le squelette.
- Lumière dorée des hautes fenêtres rondes, poussière qui flotte comme un encens profane, des échelles sur rails le long des étagères-racines, silence de cathédrale.
- On y entre à voix basse : ici, la mémoire est sacrée, et l'écho d'une phrase fausse y paraît presque une profanation.

##  Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

- Édifié après la [[Guerre des Racines]] comme **mémoire commune du pacte** : la Ville y consigna ses archives historiques, ses anciennes cartes d'[[Elseran]] et les écrits diplomatiques liés au Serment.
- Le [[Collège des Chantres d'Écorce]] y entretient le scriptorium et veille à la transcription de la mémoire orale.
- C'est ici que siège la [[Cour des Échos]] : les racines du Mir'Sylva traversant l'îlot baignent ses fondations, si bien que **le moindre mensonge prêté sur le Serment résonne dans l'Arbre** — les druides de l'Écoute sylvestre peuvent l'y confirmer.
- Secret : la **Voûte des Chartes**, sous trois sceaux, garde les originaux du Serment des Racines — et certaines cartes anciennes que le [[Conseil du Lien]] préférerait voir rester à l'abri.

##  Points d'intérêt (Sous-lieux)

- **La Salle des Échos** : l'auditoire de la Cour, en hémicycle — dais du Juge-Écho, deux sièges d'Écoutes (impérial et sylvestre), bancs courbes ; acoustique parfaite, calculée pour qu'aucune voix ne tremble sans qu'on l'entende.
- **La Grande Voûte des Chartes** : l'archive scellée du Serment, porte ronde à trois sceaux, enclavée dans un affleurement de racine et de roche.
- **La Salle des Cartes** : les anciennes cartes d'Elseran, rouleaux et cabinets à planoires — l'endroit où l'on vient chercher un chemin oublié.
- **Le Scriptorium** : les longues tables des scribes du Collège des Chantres d'Écorce.
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

- *(à remplir après la Session « Plaider Coupable » : le procès de [[Vox Cineris]] le 40-07-403, le témoignage de [[Morgath]], l'exposition d'[[Ambroise de Valcourt]]...)*