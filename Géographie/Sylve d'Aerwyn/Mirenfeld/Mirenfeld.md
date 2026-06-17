---
tags:
  - lore/géographie
  - elseran
  - cité
  - sylve
type: lieu
nom: Mirenfeld
categorie: Ville
parent: "[[Frondains]] [[Sylve d'Aerwyn]]"
population: "[[elfes]] [[gnomes]] [[halfelins]] [[humains]]"
factions_presentes: "[[Galavorn]] [[Aeriel]] [[Cercle Druidique]] [[Ordre du Souffle]]"
securite: Haute
cree_le: 2026-06-11
---

# 📍 Lieu : Mirenfeld

```leaflet
id: leaflet-map-mirenfeld
image: [[Mirenfeld  v2 - Copie.png]]
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
> [!infobox]
>
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **Se trouve dans** | `$= dv.current().parent` |
> | **Sécurité** | `$= dv.current().securite` |
> | **Population** | `$= dv.current().population` |

## 🗺️ Description générale
*(Écris ici l'ambiance visuelle, l'architecture, le climat ou la première impression des joueurs en arrivant)*



## 📜 Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

- 

## 🏠 Points d'intérêt (Sous-lieux)
*(Si c'est une ville : les tavernes, temples, boutiques. Si c'est une région : les villages, ruines, etc.)*

### Zone A : Le Versant Sylvestre (Ouest)
Ce versant conserve l'architecture organique et sauvage de la Sylve d'Aerwyn, faisant la part belle au bois vivant, à la pierre de mousse et aux habitations suspendues.

* **5 - [[Écorce-Haute]]** : Le quartier noble de la Sylve. Une architecture aérienne et élégante, bâtie à flanc de canopée dans les branches d'arbres séculaires pour accueillir l'élite sylvestre et les dignitaires druidiques.
* **6 - [[Place des Sèves]]** : Le cœur battant de l'artisanat sylvestre. Un grand marché en plein air spécialisé dans le travail du bois noble, l'herboristerie et la préparation d'onguents magiques.
* **7 - [[Chant des Feuilles]]** : Le quartier des réjouissances et des habitations communes. C'est ici que résonnent les chants, que se trouvent les auberges festives et les places de danse traditionnelles.
* **8 - [[Les Terres de Mirenfeld|Les Terres]]** : Une zone agricole périphérique assurant la subsistance de la cité en accord avec les cycles de la terre et sans exploitation agressive.

---

## 🛠️ Recensement local (Dataview)

### 👥 Habitants et PNJ présents
*Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter.*

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
WHERE contains(list(lieu), this.file.name) and (contains(type, "PNJ") or contains(type, "PJ"))
SORT file.name ASC
```
# Mirenfeld : La Cité du Serment des Racines

> « Ici, la pierre se souvient, et la racine pardonne. »
> — Maxime locale gravée sur le Péristyle des Sages.

Située au cœur des [[Frondains]], dans la majestueuse [[Sylve d'Aerwyn]], **Mirenfeld** est la plus grande cité de la région et le symbole vivant d'une trêve sacrée. Ancien poste avancé militaire de l'[[Empire Vhalarionnien]], la cité fut le théâtre de violents affrontements durant la [[Guerre des Racines]]. Elle a depuis fusionné de manière organique avec le [[Mir'Sylva]], sous l'égide des [[Druide|druides]] de [[Khor'Vélyss]], à la suite du scellement du sacré [[Serment des Racines]]. 

Aujourd'hui, Mirenfeld is une métropole diplomatique et marchande unique sur [[Elseran]], où la pierre taillée impériale s'entrelace de façon indissociable avec le bois vivant et la magie de la forêt.

---

## Cartographie de la Cité



---

## I. Structure Urbaine et Quartiers

, toutes organisées en cercles concentriques autour d'un noyau de pouvoir central.



### Zone B : L'Îlot Central (Le Noyau du Pouvoir)
Organisé en cercles concentriques sur une île rocheuse au milieu de l'[[Anserah]], ce secteur incarne la fusion absolue entre la rigueur impériale et la puissance de la nature sacrée.

| Cercle | Appellation | Description et Fonction |
| :--- | :--- | :--- |
| **Cercle 1** | **[[Place du Serment]]** | La citadelle de pierre blanche impériale, désormais entièrement fusionnée avec le [[Mir'Sylva]] (l'Arbre-Pilier). C’est ici que siège le glorieux **[[Conseil du Lien]]**. |
| **Cercle 2** | **[[Anneau des Maîtres]]** | Le secteur administratif et économique abritant les sièges des grandes corporations, des guildes et des institutions de la cité. |
| **Cercle 3** | **[[Péristyle des Sages]]** | Le cercle politique supérieur abritant les résidences des hauts dignitaires et la **[[Loge des Hauts-Druides]]** de [[Khor'Vélyss]]. |

### Zone C : Le Versant Cosmopolite (Est)
Affichant une architecture vhalarionnienne classique en marbre blanc et pierre taillée, ce versant accueille les influences, les marchands et les voyageurs de tout le continent d'[[Elseran]].

* **9 - [[Les Terrasses d'Or'Azur]]** : Quartier résidentiel de prestige accueillant l'aristocratie vhalarionnienne, les diplomates étrangers et les plus grandes fortunes marchandes du continent.
* **10 - [[Le Quai des Mondes]]** : D'immenses halles marchandes et des docks fluviaux très actifs. C'est le centre névralgique d'importation des produits exotiques, des métaux et des innovations techniques d'Elseran.
* **11 - [[Croisée des Chemins (Mirenfeld)|Croisée des Chemins]]** : Le quartier des voyageurs et des aventuriers. Un carrefour cosmopolite grouillant d'auberges, de tavernes et de commerces de passage.
* **12 - [[Le Pavé des Ouvriers]]** : Quartier populaire et résidentiel abritant la main-d'œuvre, les artisans étrangers et la classe moyenne de la cité.

### Zones Spécifiques et de Transition
* **4 - [[Le Rempart (Mirenfeld)|Le Rempart]]** : Des quais et des fortifications militaires stratégiques surveillant le cours de l'[[Anserah]] et protégeant l'accès à l'Îlot Central.
* **13 - [[Creux de l'Anserah]]** : Les bas-fonds de la ville, situés sous les pilotis et dans les cavités rocheuses de l'île. Territoire de contrebande, marché noir et guildes de l'ombre.

---

## II. Le Conseil du Lien

Le **[[Conseil du Lien]]** est l'organe gouvernemental suprême de Mirenfeld, établi par le [[Serment des Racines]] pour maintenir l'harmonie entre la Sylve et l'Empire. Il se compose de sept sièges, représentant chacun un pilier de la stabilité régionale.

Plutôt que des votes formels, les décisions du Conseil sont traditionnellement prises par **harmonisation de chants rituels** : si les voix et les esprits s'alignent dans le rythme, la loi est adoptée.

### Les Sept Magistrats du Conseil

| Siège                           | Rôle & Responsabilités                                                                                                                                             | Magistrat                | Description                                                                                                                                                                                            |
| :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Le Haut-Druide d'Aerwyn**     | Chef spirituel du [[Cercle de Nourchêne]] (dont le siège est à [[Khor'Vélyss]]). Gardien du [[Mir'Sylva]] et de la santé spirituelle de la forêt.                  | [[Vahris l'Écorcé]]      | Un vieil homme dont la peau est marquée de runes vivantes. Très respecté, il porte la mémoire du Serment originel et veille scrupuleusement au respect des cycles naturels.                            |
| **La Voix des Galavorn**        | Représentante du clan elfe des Galavorn (les Hauts-Feuillus).                                                                                                      | [[Elenwë de Cime-Haute]] | Fière et austère, elle est partisane d'un isolationnisme strict de la Sylve et se montre extrêmement méfiante envers toute forme d'expansionnisme humain.                                              |
| **La Voix des Aeriël**          | Représentante du clan elfe des Aeriël.                                                                                                                             | [[Sylhira d'Aey'Luin]]   | Calme, éthérée et tournée vers les échanges spirituels et la vie dans la canopée. Elle est réputée pour ses visions prophétiques et guide les voyageurs dans la compréhension des murmures sylvestres. |
| **L'Ambassadrice de Vhalarion** | Représentante diplomatique directe de l'[[Empire Vhalarionnien]].                                                                                                  | [[Dame Iriah d'Orvel]]   | Une humaine rationnelle, ambitieuse et descendante des anciens bâtisseurs impériaux. Elle s'efforce de préserver les intérêts économiques et diplomatiques de l'Empire de pierre.                      |
| **Le Porteur des Marches**      | Grand trésorier et économiste de la cité. Il régule les taxes, supervise les guildes marchandes et gère les finances.                                              | [[Brannos le Large]]     | Un halfelin jovial et affable qui cache, sous sa bonhomie naturelle, un redoutable réseau d'informateurs et d'espions urbains.                                                                         |
| **Le Garde des Ponts**          | Capitaine des [[Veilleurs de Sève]] (la force de sécurité mixte de la cité). Responsable de la garnison, de la défense des ponts et du maintien de l'ordre public. | [[Dhorren Vass]]         | Un vétéran humain loyal mais désabusé, qui a renoncé aux armures métalliques au profit de cuirasses de sève vivante.                                                                                   |
| **Le Scribe du Souffle**        | Historien, archiviste et garant de l'intégrité du [[Serment des Racines]].                                                                                         | [[Nhyrel de Myrrha]]     | Un érudit gnome doté d'une mémoire absolue, chargé de veiller à l'application stricte des lois du pacte et de conserver les archives sacrées.                                                          |

---

## III. Édifices Majeurs et Institutions

### [[L'Institut de l'Entrelacs]] *(Académie Mixte de Mirenfeld)*
* **Localisation** : [[Croisée des Chemins (Mirenfeld)\|Croisée des Chemins]] (11)
* **Description** : Le joyau intellectuel de la cité. Cette académie prestigieuse fusionne les disciplines de l'[[Empire Vhalarionnien]] (magie classique, ingénierie de pierre, droit civil) avec les savoirs ancestraux des [[Druide|druides]] (magie de la nature, herboristerie sacrée, cycles sylvestres). Son architecture unique entrelace de massives colonnes de pierre impériale et des racines vivantes porteuses de sève magique.

### [[L'Auberge du Chêne Vert]]
* **Localisation** : [[Croisée des Chemins (Mirenfeld)\|Croisée des Chemins]] (11)
* **Description** : L'établissement de voyage le plus célèbre d'Aerwyn. Construite autour d'un chêne titanesque dont le tronc traverse tous les étages, cette auberge est le cœur de la mixité culturelle de la ville. On y sert aussi bien les vins fins de Vhalarion que l'hydromel sauvage de la Sylve, au milieu des récits d'aventuriers venus de tout Elseran.

### [[Le Temple de l'Équilibre]]
* **Localisation** : [[Place du Serment]] (1)
* **Description** : Un sanctuaire partagé, situé au pied du [[Mir'Sylva]]. D'un côté s'élève une structure de pierre ordonnée et géométrique dédiée au dieu impérial [[Aureos - Dieu Fondateur de l'Ordre]] (dieu de l'ordre et de la lumière), tandis que de l'autre s'étendent des bosquets sacrés et des racines entrelacées consacrés à la déesse [[Sylméa - Déesse Fondatrice du Lien|Sylméa]] (déesse du Lien et de la Vie).

---

## IV. Les Guildes de l'Anneau des Maîtres *(Zone B - Cercle 2)*

Ces organisations majeures structurent la vie quotidienne, économique et sécuritaire de Mirenfeld :

* **[[La Confrérie du Fer-Sève]]** : Forgerons d'élite ayant développé une méthode unique consistant à utiliser la chaleur de la sève magique pour travailler les métaux, évitant ainsi l'utilisation de charbon polluant au sein de la forêt.
* **[[Le Cartel des Bateliers de l'Anserah]]** : Guilde puissante contrôlant le transit fluvial, le fonctionnement des écluses et les ascenseurs hydrauliques permettant de naviguer sur le fleuve [[Anserah]].
* **[[Le Collège des Chantres d'Écorce]]** : Rassemblement de mages, scribes et traducteurs, gardiens de la mémoire écrite et orale du [[Serment des Racines]].
* **[[La Vigie des Cimes]]** : Corps de rôdeurs, d'éclaireurs et de rangers assurant la sécurité des routes commerciales terrestres et effectuant des patrouilles régulières dans la canopée.
* **[[L'Ordre des Alchimistes du Rosier]]** : Institution médicale combinant la médecine scientifique impériale et l'herboristerie forestière pour produire des remèdes de sève et des potions de soin.
* **[[La Ligue des Bâtisseurs de l'Équilibre]]** : Guilde d'architectes et d'ingénieurs spécialisée dans la conception de structures urbaines capables de fusionner avec le vivant sans entraver la croissance des arbres.

---

## V. Commerces et Boutiques de Référence

### Armurerie & Forge
* **[[La Forge de Fer-Bois]]** *(Zone A - [[Les Terres de Mirenfeld\|Les Terres]])* : Établissement spécialisé dans l'équipement sylvestre. Le bois y est traité par un procédé magique de trempe dans les eaux de l'[[Anserah]], lui conférant une dureté égale à celle de l'acier tout en restant léger et flexible.
* **[[L'Acier de l'Aube]]** *(Zone C - [[Le Pavé des Ouvriers]])* : Forge vhalarionnienne classique proposant des armes et armures en acier de qualité impériale, robustes et finement ornées.

### Alchimie & Soins
* **[[L'Herboristerie « La Sève Éternelle »]]** *(Zone A - [[Place des Sèves]])* : Boutique tenue par des herboristes druidiques, proposant des ingrédients bruts, des baies de soin magiques et des onguents naturels rares.
* **[[Le Creuset de Rosée]]** *(Zone B - [[Anneau des Maîtres]])* : Échoppe officielle de l'Ordre des Alchimistes du Rosier, vendant des potions de soins distillées et de précieux élixirs de sève pure.

### Artisanat & Curiosités
* **[[L'Éclat de Verre]]** *(Zone C - [[Le Quai des Mondes]])* : Maître verrier spécialisé dans le soufflage de fioles luminescentes et la création de bijoux organiques intégrant de la sève fossilisée.
* **[[La Musette du Rôdeur]]** *(Zone A - [[Place des Sèves]])* : Échoppe d'équipement de survie forestier (cordes de vignes tressées, capes caméléons, rations de voyage).
* **[[Le Plumier de l'Anserah]]** *(Zone B - [[Anneau des Maîtres]])* : Papeterie magique vendant du parchemin d'écorce fine et des encres réactives aux fluctuations magiques locales.
* **[[L'Infusion de Morphée]]** *(Zone C - [[Croisée des Chemins (Mirenfeld)\|Croisée des Chemins]])* : Un salon de thé apaisant, idéal pour les voyageurs fatigués cherchant à se détendre près de l'Auberge du Chêne Vert.

---

## VI. Temples et Lieux de Culte

* **[[Le Sanctuaire de Sylméa]]** *(Zone A - [[Chant des Feuilles]] - 7)* : Un space sacré en plein air, délimité par des arbres chantants dont le bruissement des feuilles accompagne les prières. C'est le lieu privilégié pour les mariages sylvestres et les rites de passage saisonniers.
* **[[La Cathédrale d'Auréos]]** *(Zone C - [[Les Terrasses d'Or'Azur]] - 9)* : Un chef-d'œuvre architectural de marbre blanc et de vitraux étincelants, affirmant la présence lumineuse du Panthéon Impérial à l'est de la cité.
* **[[L'Athenaeum de Myrrha]]** *(Zone B - [[Anneau des Maîtres]] - 2)* : Une bibliothèque monumentale et un sanctuaire d'étude abritant les archives historiques de Mirenfeld, d'anciennes cartes d'[[Elseran]] et les écrits diplomatiques liés au pacte.

---

## VII. Les Lieux de l'Ombre et de la Garde

* **[[Le Nid du Corbeau]]** *(Zone Specific - [[Creux de l'Anserah]] - 13)* : Une taverne borgne à moitié immergée sous les structures de la ville. C'est le lieu de rendez-vous de la pègre locale et des contrebandiers où se négocient les contrats secrets à l'insu du Conseil.
* **[[La Vigie du Rempart]]** *(Zone Specific - [[Le Rempart (Mirenfeld)\|Le Rempart]] - 4)* : La caserne principale des [[Veilleurs de Sève]], surplombant les quais militaires pour surveiller le trafic fluvial de l'[[Anserah]] et parer à toute menace d'intrusion.

---

## VIII. Secrets et Factions Souterraines

Bien que Mirenfeld soit officiellement gouvernée par le [[Conseil du Lien]], ses tréfonds abritent des secrets bien gardés :

* **Le Sanctuaire du Souffle Profond** : Dissimulé sous le lit même du fleuve [[Anserah]], ce complexe majestueux de galeries naturelles et de dômes sculptés est le siège continental secret de l'[[Ordre du Souffle (brouillon)]]. C'est là que les moines, les Scribes et les Éveillés écoutent la respiration du monde et cherchent à harmoniser les précieux fragments du *Chant des Cendres*.