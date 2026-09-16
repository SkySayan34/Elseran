---
type: objet_magique
nom: médaillon de Çaph
rareté: Très rare
catégorie: Collier
sous_catégorie: Médaillon
niveau: 8
requis:
attunement: Oui
date_de_création:
tags: objet
---

# médaillon de Çaph


> [!infobox]+ image
> ![[Médaillon de Çaph.jpg|cover h small]]
> ###### Informations générales
> | | |
> |---|---|
> | **Type** | `$= dv.current().catégorie` |
> | **Rareté** | `$= dv.current().rareté` |
> | **Sous-catégorie** | `$= dv.current().sous_catégorie` |
> | **Niveau** | `$= dv.current().niveau`|
> | **Attunement** | `$= dv.current().attunement` |
> | **Requis** | `$= dv.current().requis` |

# Histoire

Ce médaillon appartenait à [[Çaph]], un grand nécromancien au service de l'[[Empire Vhalarionnien]].
Il a été dérobé par un commandant de l'Empire ayant participé à la [[Colonisation du Dhar'Zulun]], principalement en [[Akhzir]].
Une malédiction frappa le voleur, qui l'amena à la mort, tué par celle qu'il tentait de violer.

# Effets

Si la personne qui le porte le conserve durant plus d'un mois, elle commencera à ressentir la [[malédiction de Çaph]] faire effet. La personne portant ce médaillon fait un jet de sauvegarde de constitution DD16 :
- **échec :** un de ses membres se nécrose, son esprit s'altère et elle doit réussir un jet de sauvegarde de sagesse DD15 chaque jour en plus d'un nouveau jet de sauvegarde de constitution DD16 pour ne pas sombrer et devenir un mort vivant. Au bout d'une semaine à tenir, le corps assimile la magie. Chaque échec entraîne une perte de 5PV max. Si la créature tombe à 0, elle sombre.
- **réussite :** la nécrose du médaillon de propage dans un des membres (1d4 pour savoir lequel) mais la magie est harnaché par le corps du porteur. Il débloque des sorts de nécromancie en fonction de son niveau.

# Porteur

```dataview
TABLE faction As "Faction", description as "Description"
FROM #pnj
WHERE contains(file.outlinks, this.file.link)
```

