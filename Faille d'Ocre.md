---
type: lieu
nom: Faille d'Ocre
categorie: location_precise
lieu_parent: Dhar'Zulun
securite: Haute
tags: lieu
---

# La Faille d'Ocre

> [!infobox]+ carte  
> ![[Faille d'Ocre.jpg|cover]]
> 
> ###### Repères
> 
> |   |   |
> |---|---|
> |||
> |**Catégorie**|`$= dv.current().categorie`|
> |**Se trouve dans**|`$= dv.fileLink(dv.current().lieu_parent)`|
> |**Sécurité**|`$= dv.current().securite`|

```leaflet
id: leaflet-map-La Faille d'Ocre
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

## Description générale

_(Écris ici l'ambiance visuelle, l'architecture, le climat ou la première impression des joueurs en arrivant)_

- Un canyon minéral enfoui au cœur des dunes profondes du [[Dhar'Zulun]], invisible à plus d'une journée de marche : il ne se révèle qu'en dernière minute, quand le sable cède brutalement sous l'horizon et que le vent, s'engouffrant dans la faille, chante d'une note grave et continue — les clans disent que c'est la Faille qui _récite_.
    
- Les parois, hautes de plusieurs dizaines de mètres, sont zébrées de strates d'un **ocre rouge éclatant**, veinées d'os et de sel blanc. À certaines heures du jour, le soleil cogne contre la roche et tout le canyon brûle d'une lumière de braise — le "bain de sang" des Veilleurs.
    
- Pas de murailles, pas de porte, pas de garnison : la seule chose qui protège la Faille est le **tabou**. Un étranger qui y entre armé offense tous les clans du désert d'un coup ; un clan qui y porterait le fer signerait son arrêt de mort rituel.
    
- Des **encoches** identiques à celles du blason des Veilleurs sont gravées sur toute la longueur des parois d'entrée — une par dette prononcée depuis la fondation de la caste, disent-ils ; la roche est presque saturée.
    
- Au sol : des tentes de lin grossier délavé, des cercles de pierres pour les rites, et de longues cordes de perles d'os tendues entre les parois — chaque perle un nom, chaque corde une lignée de comptes. On y vit la nuit, comme partout dans le désert ; à midi, seuls les Éveilleurs s'exercent à la récitation à l'ombre des strates.
    

## Histoire & Lore

_(Le passé de ce lieu, les événements marquants ou les secrets géographiques)_

- **La fondation.** À l'issue de la [[Guerre des Sables]], quand les belligérants, épuisés, imposèrent des arbitres à chaque clan, ces premiers Veilleurs cherchèrent un lieu neutre pour tenir leurs comptes — un endroit qui ne fût à personne. Le canyon était le site d'un ancien champ de bataille où chaque clan avait versé du sang ; cette terre, disent-ils, n'appartenait donc _plus à personne_ — elle fut déclarée Faille, littéralement « la déchirure entre les clans ».
    
- **La seconde blessure.** Selon la mémoire rituelle des Voix-du-Compte, un seul clan a jamais osé porter le fer jusqu'ici : un chef de guerre nommé **Varlag**, venu réclamer une dette de sa main. Son clan ne s'est jamais remis de l'offense — la Faille fut le début et la fin de sa lignée, effacée par la coalition de tous les autres clans. L'emplacement exact de sa tente, près de l'entrée, est marqué d'une pierre noire : nul ne la touche, et les Éveilleurs la récitent chaque Veillée, pour que nul ne l'oublie.
    
- **Le silence de la Faille.** Aucune razzia, aucune guerre déclarée ne peut y pénétrer ; aucune dette ne peut y être contractée ni soldée. C'est le seul lieu du désert où l'on peut tuer quelqu'un sans créer de dette du Prix du Sang — ce qui est précisément pour quoi personne ne l'a jamais fait : un meurtre en Faille est rituellement _gratuit_, donc monstrueux.
    
- **Les orphelins du désert.** Les clans y déposent les orphelines et orphelins destinés à la caste, souvent à l'entrée, dans des nacelles de toile suspendues — les Veilleurs les récupèrent à la tombée du jour, sans jamais demander d'où ils viennent : l'enfant entré en Faille n'a plus de lignée, plus de nom, plus de dette.
    
- **Un lieu habité, non un sanctuaire.** La Faille n'est pas un temple vide : c'est une cité troglodyte miniature creusée dans les parois nord, avec la Grande Strate (la salle des Veillées du Serment), les cellules des Voix-du-Compte, et les écoles de récitation des Éveilleurs, où les enfants apprennent à réciter des milliers de comptes en les chantant sur des airs de marche.
    

## Points d'intérêt (Sous-lieux)

_(Si c'est une ville : les tavernes, temples, boutiques. Si c'est une région : les villages, ruines, etc.)_

```dataview
LIST
FROM #lieu
WHERE contains(lieu_parent, this.file.name)
```

---

## Habitants et PNJ présents

_Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter._

```dataview
TABLE faction AS "Faction", description AS "Description"
FROM #PNJ
WHERE contains(list(lieu), this.file.name)
SORT file.name ASC
```

## Impact du jeu sur le lieu

_(Raconter les éventuels changement qu'ont apportés les joueurs sur le lieu)_