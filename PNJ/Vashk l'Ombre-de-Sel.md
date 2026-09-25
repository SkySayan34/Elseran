---
type: PNJ
statut: Vivant
faction: Veilleurs d'Ocre
fonction: Tourneur de Pages (chez les Ertuk)
lieu: Géographie/Dhar'Zulun/Dhar'Zulun
alignement: LN
race: Orc
classe:
genre: Homme
description: Vénérable Veilleur d'Ocre à la peau blanche de sel, le seul orc vivant à avoir atteint la Mer de l'Est. Témoin du secret de Grushnak.
tags: PNJ
---

# Vashk l'Ombre-de-Sel

> [!infobox]+ portrait
> ![[Vashk l'Ombre de Sel.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.fileLink(dv.current().faction)` |
> | **Fonction** | `$= dv.current().fonction` |
> | **Lieu** | `$= dv.fileLink(dv.current().lieu)` |
> | **Statut** | `$= dv.current().statut` |


##  Description & Psychologie

* **Apparence :** Orc très âgé, desséché comme une racine de sel. Peau blanche d'os éclatant, craquelée de fines gerçures rosées — le sel de la Mer de l'Est l'a marqué à jamais, lui qui était gris-bronze comme les siens. Yeux noirs profonds et humides, le seul point vivant de son visage, qui regardent toujours un peu au-delà de son interlocuteur. Maigre et long, il marche appuyé sur un bâton de bois flotté — du bois de la Mer, sa relique et sa preuve. Robes ocre grossières des Veilleurs ceinturées de corde, chapelet de perles d'os très usées autour du cou. Aucun brand sur la peau : ses dettes sont acquittées par le service de la caste, sa plus grande fierté silencieuse.

* **Personnalité :** Contemplatif, lent, d'une douceur d'ermite — mais désertique : elle ne promet rien, elle donne juste à voir ce qui est. Parle peu, souvent en métaphores de voyage et d'eau (« une dette, c'est une soif ; on ne la fait pas disparaître, on ne choisit que ce qu'on boit »). Écoute plus qu'il ne juge, mais la rigueur de sa caste est en lui comme le sel dans sa peau : jamais il ne faussera un compte. Manies : lisse le bois flotté de son bâton pendant les conversations longues ; ferme les yeux quand on lui ment (il le sait toujours, il ne dit rien) ; répond aux questions pressées par une question plus lente.

* **Motivation principale :** Achever sa vie en laissant deux comptes soldés — la dette fratricide Ertuk–Zarka qu'il voudrait voir apaisée avant sa mort, et celle, secrète, de [[Kyr'Dharûn]] : il veut être celui qui ramène le déserteur, car il reconnaît en lui le chemin qu'il a lui-même manqué de justesse.

* **Secrets / Ce qu'il cache :**
	1. Il est le témoin de la mort du mentor — il a vu Grushnak tuer le mentor en duel cette nuit-là et a gardé le silence : le code du duel était respecté, et la parole d'un Veilleur aurait déchiré le clan. Si ce secret transpirait, son impartialité serait brisée — le Veilleur qui se tait n'est plus un Veilleur — et Grushnak tomberait avec lui.
	
	2. Il a accidentellement tué un membre de son ancien clan dans sa jeunesse et a fui vers l'ouest sans demander le compte : sa traversée légendaire était une fuite, pas un exploit. C'est en revenant qu'il s'est constitué, a fait compter sa dette et l'a acquittée par le service de la caste. Les jeunes croient que l'Ombre-de-Sel est un héros de la marche ; les anciens savent qu'il est d'abord un déserteur repenti.
	
	3. Ce qu'il a vu face à la Mer, il ne l'a jamais dit en entier, même à la Voix-du-Compte : chaque Veilleur qui lui demande reçoit un fragment différent, comme des perles d'un chapelet jamais entièrement déroulé. En réalité, il a reçu un [[Fragment du Chant des Cendres]].

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- Avant d'être Veilleur, Vashk a tenté de s'exiler et traversa seul l'Ouest du Dhar'Zulun — l'exploit le plus dangereux du désert, rare et exceptionnel. Face à la Mer de l'Ouest, il a compris la place de la vie dans le monde, et il est revenu : il a renoncé à son nom de clan, prêté serment, et gravit les rangs jusqu'à Tourneur de Pages. Sa traversée est devenue un enseignement pour la caste : les Éveilleurs apprennent son récit, et certains rêvent de refaire le pèlerinage — presque aucun ne s'y risque. Sa peau blanche de sel en fait une figure visuellement unique du désert : on dit qu'il est « la seule neige du Dhar'Zulun ».

- Miroir et destinée possible de Kyr'Dharûn — le déserteur qui est revenu et a trouvé sa place. C'est par lui que le PJ peut apprendre le secret de [[Grushnak des Ertuk]] (s'il gagne sa confiance), comprendre la portée de sa dette, et trouver la voie du retour sans exécution. Il veille aussi discrètement sur la maison de Kyr'Dharûn, la famille endettée.



##  Relations & Connexions

* **Alliés :** La Voix-du-Compte et la caste des [[Veilleurs d'Ocre]] (vénéré comme le marcheur de la Mer) ; [[Grushnak des Ertuk]], par un silence partagé plutôt que par amitié ; dans l'ombre, la maison de [[Kyr'Dharûn]], qu'il protège sans le dire.

* **Ennemis :** Les partisans du mentor mort — l'aile dure du clan Ertuk qui estime que la dette doit être payée par la lignée de Kyr'Dharûn, qui conteste le gel de la dette prononcé par les Veilleurs, et donc conteste Vashk lui-même.

* **Réseau :** Tous les Veilleurs du désert (réseau rituel de la caste) ; la mémoire des comptes de toutes les Veillées auxquelles il a assisté ; les rares clans de l'Ouest profond qu'il a croisés lors de sa traversée — dont il ne parle jamais.

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
### Conseils d'interprétation en partie

**Voix et diction** : voix basse, lente, éraillée par le sable — comme le vent dans la Faille. Débit très lent, avec de vraies pauses de silence qu'il ne comble jamais. Vocabulaire concret du désert (eau, soif, sel, pas, dune) même pour les sujets abstraits. Il ne s'excuse jamais de son rythme : c'est le désert qui parle à sa vitesse. Accent rauque, sec ; il laisse les phrases finir avant de reprendre.

**Tics de langage et gestes** : lisse le bois flotté de son bâton pendant les conversations sérieuses (plus la question est grave, plus il lisse lentement) ; répond aux questions pressées par une question plus lente ; compte sur ses perles d'os en écoutant un récit ; dit « la Mer » avec une micro-pause avant, toujours ; appelle les PJ par des surnoms de choses (« petit vent », « pierre qui roule »), jamais par leur nom — sauf Kyr'Dharûn, dont il évite soigneusement de prononcer le nom.

**Réactions types** :

- _Face à la violence_ : il ne s'interpose pas, il s'assied. Calme plat désarmant : « Le sang criera plus tard. Il crie toujours plus tard. » Il compte les coups — littéralement.
- _Face à la négociation_ : très bon juge, mais il ne négocie jamais un compte ; il propose toujours une troisième voie en don.
- _Face à la flatterie_ : ferme les yeux, sourit doucement, ne répond pas — c'est sa façon de dire qu'il a vu le mensonge.
- _Face au mensonge_ : les yeux fermés, il laisse finir, puis pose LA question lente qui éventre le mensonge sans l'accuser jamais.

**Conseils de RP** :

- **Le levier émotionnel, c'est le miroir** : dès qu'il parle à Kyr'Dharûn, chaque phrase a deux sens — il raconte sa propre fuite en parlant de celle du PJ. Ne le faites jamais dire explicitement « je suis comme toi » : les joueurs doivent le comprendre au 3e ou 4e échange, c'est un moment de table en or.
- **Doser les secrets** : le meurtre accidentel de jeunesse peut tomber assez vite (c'est presque une leçon qu'il donne) ; la traversée-fuite ensuite ; le secret de Grushnak **jamais directement** — il ne le livrera qu'en dernier recours, et seulement à Kyr'Dharûn, et probablement sous forme de métaphore à déchiffrer. Le trio Grushnak/Vashk/Kyr'Dharûn vaut une fin d'arc.
- **Le rendre mémorable** : c'est le seul personnage du désert qui a vu la mer — chaque fois qu'un joueur le doute, il sort un détail impossible (le goût, le son, l'immobilité vivante de l'eau) et se tait. Le mystère de « ce qu'il a vu face à la Mer » doit rester entrouvert même à la fin de la campagne.
- **Conflit jouable** : l'aile dure du clan le déteste — utilisez-le comme pression temporelle. Si les PJ tardent, Vashk vieillit, et l'aile dure gagne du terrain sur le gel de la dette.

### Liens Out
`$= dv.fileLink(dv.current().lieu)`
`$= dv.fileLink(dv.current().faction)`

