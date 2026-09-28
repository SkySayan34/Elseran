---
type: PNJ
statut: Vivant
faction: Cercle de Lir
fonction: Haut Druide du Cercle de Lir, Protecteur du Sud (garant des courants méridionaux du Souffle)
lieu: Géographie/Sylve d'Aerwyn/Frondains/Lethariel
alignement: LB
race: Elfe Galavorn
classe: Druide
genre: Homme
description: Vieil elfe vouté, haut druide du cercle de Lir
tags: PNJ
---

# Druan Silme



> [!infobox]+ portrait
> ![[Druan Silme.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.fileLink(dv.current().faction)` |
> | **Fonction** | `$= dv.current().fonction` |
> | **Lieu** | `$= dv.fileLink(dv.current().lieu)` |
> | **Statut** | `$= dv.current().statut` |


##  Description & Psychologie

* **Apparence :** Elfe sylvestre d'environ 300 ans, grand mais légèrement voûté « comme un arbre qui a poussé vers le fleuve ». Tresse longue d'argent-cuivré nouée d'un anneau de bois vivant qui n'a jamais cessé de pousser. Yeux vert d'eau très clairs, qui semblent toujours écouter autre chose. Vêtements simples en fibres tressées aux teintes de lisière, manteau de plumes et d'écorce, aucun métal. Bâton-racine noueux surmonté d'une spirale venteuse gravée, symbole de Lir. Une brise légère semble toujours l'accompagner.

* **Personnalité :** Attentif, patient, praticien du sacré : il entretient le Souffle comme un jardinier entretient un verger, sans nostalgie ni ambition. Peu bavard mais d'une chaleur tranquille et volontaire. Manie les métaphores de souffle et de courant. Tic : pose une main à plat sur le sol, un arbre ou une épaule quand il réfléchit, comme pour prendre le pouls du monde.

* **Motivation principale :** Assurer la libre circulation des courants méridionaux du Souffle, entretenir le Cercle de Lir, veiller sur Lethariel et l'Anserah. Depuis le rituel : comprendre ce qu'était l'Ombre d'Anserah — et si elle pourrait revenir.

* **Secrets / Ce qu'il cache :** Depuis le rituel, il sent que le Souffle au bord de l'Anserah « porte une odeur » qu'il ne reconnaît pas. Il craint que l'Ombre combattue par les PJ n'ait été qu'un symptôme d'un mal plus profond, mais n'en parle à personne pour ne pas alarmer Lethariel ni inquiéter son cercle.

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

Formé par des druides de Khor'Vélyss (n'a jamais rencontré Oakhaven, qui lui est antérieur). Le Cercle de Lir est faible en nombre, mais l'esprit Lir y reste présent et actif ; Druan ne cherche pas à agrandir le cercle, seulement à l'entretenir. A formé un temps Naelwyn, jeune demi-elfe partie à Mirenfeld avec les PJ pour finaliser sa formation auprès des druides de Khor'Vélyss.

**Rôle dans l'intrigue :** Poste d'écoute du Sud. A accueilli les PJ en intro de campagne et a mené avec eux le rituel qui a révélé l'Ombre d'Anserah — qu'ils ont combattue et qui a disparu. Point de contact naturel pour tout ce qui touche au Souffle, à la Sylve et à la frontière du Dhar'Zulun.


##  Relations & Connexions

* **Alliés :** Les habitants de Lethariel ; les druides de Khor'Vélyss. (Lir n'est pas un allié au sens strict : esprit qui assiste le cercle qui lui est dédié.)
* **Ennemis :** Aucun réel ennemi pour le moment. (Le Tourmenteur est totalement inconnu de tous à ce stade et n'entre pas dans ses relations.)
* **Réseau :** Les animaux et esprits de la Sylve, les villageois de Lethariel et les voyageurs passant par le village.

##  Coulisses du MJ
*Cette section se remplit automatiquement si d'autres notes (quêtes, sessions, rumeurs) mentionnent ce PNJ.*

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

### Conseils d'interprétation 

**Voix et diction**

- Voix posse, grave et lente — il ne se presse jamais, même en crisis (sauf si le Souffle lui-même est menacé : alors il devient soudain net et rapide, contraste marquant).
- Légère scansion chantante, comme s'il marquait le rythme du vent entre ses phrases. Il laisse des silences que les joueurs rempliront naturellement — leurs confidences tomberont dedans.
- Vocabulaire concret, paysan presque : il ne dit pas « la magie est instable » mais « le courant tourne mal ».

**Tics de langage et gestes réutilisables**

- Mains à plat sur le sol / un arbre / une épaule quand il réfléchit ou rassure.
- Termine souvent ses conseils par une métaphore de souffle : « Laisse ça prendre le vent », « Ça sent l'orage derrière la brise ».
- Ferme les yeux une à deux secondes avant de répondre à une question importante — il « écoute » d'abord.

**Réactions types**

- Face à la violence : ne s'interpose presque jamais physiquement ; il déçoit calmement (brise qui éteint, racine qui accroche). Déçu plutôt que fâché : « Le fer hurle toujours plus fort que la forêt n'écoute. »
- Face à la négociation : très bon marchand, mais ne marchande jamais en or — il échange en services, en respect de la Sylve, en promesses tenues.
- Face à la flatterie : la fait glisser comme l'eau sur une feuille : « La brise flatte aussi les feuilles ; elle les emporte quand même. »
- Face au mensonge : il ne le dénonce presque jamais frontalement. Il sourit, note, et la Sylve se souviendra. Les joueurs devraient sentir que mentir à Druan est possible, mais jamais gratuit.

**Conseils de RP**

- Le rendre mémorable : son « aura de brise permanente » — décris à chaque apparition un micro-détail de vent (flammes qui dansent, feuille qui tourbillonne, poussière qui se soulève) : les joueurs l'identifieront vite.
- Levier émotionnel : son attachement paternel discret à Naelwyn — si les joueurs lui donnent des nouvelles d'elle, il laisse percer une émotion rare et touchante.
- Doser le secret : distille-le en trois temps — (1) indices indirects : il renifle l'air, froncement de sourcil au bord du fleuve ; (2) si les PJ reviennent vers lui après l'intro, il finit par admettre : « Depuis le rituel, le Souffle porte une odeur que je ne connais pas » ; (3) c'est lui qui devrait venir les trouver quand l'odeur s'aggravera — le MJ garde la main sur le timing.
- En combat : il protège, entrave, soigne — jamais ne tue. Sa colère, rare, c'est la tempête contenue.