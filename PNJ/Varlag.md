---
type: PNJ
statut: Mort
faction: Rukh-Tarr
fonction: Chef de Guerre
lieu: Géographie/Dhar'Zulun/Dhar'Zulun
alignement: CN
race: Orc
classe: Barbare
genre: Homme
description: Le dernier chef à avoir porté le fer en Faille d'Ocre. Sa lignée fut effacée pour l'exemple.
tags: PNJ
---
# Varlag

> [!infobox]+ portrait  
> ![[Varlag.jpg|cover]]
> 
> ###### Infos Rapides
> 
> |   |   |
> |---|---|
> |||
> |**Faction**|`$= dv.fileLink(dv.current().faction)`|
> |**Fonction**|`$= dv.current().fonction`|
> |**Lieu**|`$= dv.fileLink(dv.current().lieu)`|
> |**Statut**|`$= dv.current().statut`|

## Description & Psychologie

- **Apparence :** _(aucune trace visuelle fiable — la mémoire rituelle le décrit plutôt qu'elle ne le montre)_ Un géant même pour un orc, couvert de brands de guerre jusqu'à la mâchoire — le signe d'un homme _à jour de comptes_, ce qui rendait sa rébellion d'autant plus insoutenable pour la caste. On raconte qu'il portait sa hache nue en permanence, même en temps de paix.
    
- **Personnalité :** Direct, orgueilleux, méprisant envers tout ce qui ralentit la vengeance — y compris la prudence. Il ne niait pas la valeur du [[Glossaire#Le Prix du Sang - Code des Clans Nomades du Dhar'Zulun|Prix du Sang]] : il niait celle des Veilleurs, ces « eunuques de la mémoire » qu'il accusait d'avoir volé aux clans le droit de régler leurs comptes eux-mêmes.
    
- **Motivation principale :** Recouvrer une dette de sang que les Veilleurs avaient, selon lui, mal comptée — un frère tué dont le sang, disait-il, dormait impayé depuis la Grande Lassitude.
    
- **Secrets / Ce qu'il cache :** Rien — c'est tout le drame de Varlag. Il a agi **au grand jour**, déclarant à la face du désert qu'il allait chercher son dû en Faille. Sa transgression n'était pas sournoise, elle était publique et assumée.
    

## Notes & Lore

- Varlag vécut environ **un siècle après la fin de la [[Guerre des Sables]]**, à une époque où les clans avaient presque oublié ce que le désert était avant le Prix du Sang.
    
- Il marcha jusqu'à La [[Faille d'Ocre]] avec une garde de dix-neuf guerriers — non pour piller, mais pour **verser le sang d'un débiteur réfugié** dans la Faille. Le meurtre y était rituellement gratuit ; Varlag pensait y avoir trouvé la faille du code : un endroit où la dette se payait sans en créer une nouvelle.
    
- Aucun Veiller ne leva la main contre lui. C'est **le débiteur lui-même** — un vieil orc sans nom, réfugié là depuis des années — qui sortit de la Faille pour l'affronter, préférant mourir en soldat plutôt que de laisser profaner le lieu. Varlag le tua.
    
- Le tabou fit le reste : la coalition de tous les clans du désert traqua et **effaça le clan de Rukh-Tarr** en une seule saison. Les dix-neuf gardes furent livrés vivants aux lignées créancières ; Varlag périt le dernier, dit-on, en refusant de prononcer le compte de son propre sang.
    
- Sa tente, près de l'entrée de la Faille, est marquée d'une **pierre noire** que nul ne touche. Les Éveilleurs la récitent à chaque Veillée — non pour l'honorer, mais **pour que nul ne l'oublie** : le désert se souvient de ce qui arrive à ceux qui portent le fer en Faille.
    

## Relations & Connexions

- **Alliés :** Sa garde des Dix-Neuf (morts ou livrés) ; quelques lignées discrètes qui murmuraient encore contre les comptes des Veilleurs.
    
- **Ennemis :** La caste des [[Veilleurs d'Ocre|Veilleurs d'Ocre]] (par sa faute, non la leur) ; _tous_ les clans du désert, après la transgression.
    
- **Réseau :** Aucun survivant : sa lignée fut effacée pour l'exemple. Seuls subsistent les murmures — car la rumeur dit que d'autres, quelque part dans les dunes, gardent des comptes que les Veilleurs n'ont jamais prononcés.
    

## Coulisses du MJ

_Cette section se remplit automatiquement si d'autres notes (quêtes, sessions, rumeurs) mentionnent ce PNJ._

### Quêtes liées

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM ""
WHERE type = "quête" AND contains(file.outlinks, this.file.link)
```

### Journal des rencontres

```dataview
LIST
FROM ""
WHERE type = "session" AND contains(file.outlinks, this.file.link)
SORT file.name DESC
```

### Liens Out

`$= dv.fileLink(dv.current().lieu)`  
`$= dv.fileLink(dv.current().faction)`
