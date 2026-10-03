---
type: PNJ
statut: Vivant
faction: Cercle de Lir
fonction: Apprentie de [[Druan Silme]]
lieu: Géographie/Sylve d'Aerwyn/Mirenfeld/Mirenfeld
alignement: LB
race: Demi-Elfe
classe: Druide
genre: Femme
description: Jeune demi-elfe, apprentie au [[Cercle de Lir]].
tags: PNJ
---

# Naelwyn

> [!infobox]+ portrait
> ![[Naelwyn.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.fileLink(dv.current().faction)` |
> | **Fonction** | `$= dv.current().fonction` |
> | **Lieu** | `$= dv.fileLink(dv.current().lieu)` |
> | **Statut** | `$= dv.current().statut` |


##  Description & Psychologie

* **Apparence :** Jeune demi-elfe d'à peine 20 ans (en équivalent humain), frêle sans être fragile, démarche discrète de celle qui a appris à se faire petite. Traits fins de son père elfe (oreilles pointues, grands yeux ambre-doré) sur un visage encore rond d'adolescence. Cheveux châtain clair mi-longs, mal attachés d'une lanière de cuir avec une fleur séchée piquée dedans. Mains calleuses de travaux de village et d'herboristerie. Vêtements simples de voyage aux teintes de la lisière, un peu trop grands pour elle. Collier-talisman : spirale de [[Lir - Esprit du Souffle|Lir]] taillée dans un galet de l'[[Anserah]], cadeau de Druan, son seul bien précieux. Un petit moineau l'accompagne souvent sans qu'elle l'appelle.

* **Personnalité :** Timide, enjouée, empathique. Parle peu aux inconnus, rougit facilement, mais illumine quand on l'écoute vraiment : rire franc, questions nombreuses. Lit les émotions des autres avant les siennes, parfois à son détriment. Tic : s'excuse même quand elle n'a rien à se reprocher ; trie des herbes ou caresse un animal quand la conversation la dépasse. Phrases simples, souvent interrompues, avec des sauts d'enthousiasme soudains pour une plante, une bête ou une histoire.

* **Motivation principale :** Devenir digne de la confiance de Druan et du Souffle — achever sa formation à [[Khor'Vélyss]], comprendre ce que [[Lir - Esprit du Souffle|Lir]] a vu en elle, et se prouver qu'une fille reniée peut appartenir à quelque chose. Plus simplement : se faire des amis — et les PJ sont sa meilleure chance.

* **Secrets / Ce qu'il cache :** 
	* *La blessure du père :* elle cache à tous que son père elfe l'a reniée et invente des versions vagues (« il est mort », « il est reparti au loin »). Découvrir la vérité est un levier émotionnel fort pour la rapprocher des PJ.
	* *Le poids du destin :* Druan lui a confié ce que [[Lir - Esprit du Souffle|Lir]] a soufflé — qu'elle participerait à rétablir le Souffle lors des perturbations à venir. Elle n'en a parlé à personne, par peur de ne pas être à la hauteur, et cette peur la paralyse parfois au pire moment.

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

Fille d'une villageoise de [[Lethariel]] morte quand elle était petite ; son père, elfe de passage, l'a reniée. Orpheline de fait, elle a grandi à [[Lethariel]] où [[Druan Silme]] l'a prise sous son aile : il avait lu dans le Souffle (par [[Lir - Esprit du Souffle|Lir]]) qu'une apprentie viendrait à lui. Les PJ devaient l'escorter jusqu'aux druides de [[Khor'Vélyss]] à [[Mirenfeld]] pour finaliser sa formation.

**Rôle dans l'intrigue :** Rôle significatif dans les perturbations du Souffle à venir.

##  Relations & Connexions

* **Alliés :** Les PJ ; [[Druan Silme]] (mentor de cœur) ; les villageois de [[Lethariel]] ; [[Sorenza]] (tenancière de l'Auberge du Chêne Vert, [[Ordre du Souffle]]).

* **Ennemis :** Aucun pour le moment.

* **Réseau :** Peu de choses — essentiellement ce qui touche [[Lethariel]] et le petit monde de Druan.

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


### Conseils d'interprétation :

**Voix et diction**

- Voix claire et douce, débit rapide quand elle s'anime, presque inaudible quand elle est intimidée. Elle parle du bout des lèvres aux inconnus, puis de plus en plus librement à mesure qu'elle se sent en sécurité — c'est ton thermomètre de lien avec les PJ : plus elle est bavarde, plus ils gagnent sa confiance.
- Saute du coq à l'âne avec enthousiasme : « Pardon ! Ce n'était pas la question… mais cette plante, là, vous avez vu ? »
- Petites excès de politesse : « pardon », « merci », « désolée » en boucle.

**Tics de langage et gestes réutilisables**

- Joue avec le collier-galet de l'[[Anserah]] quand elle est nerveuse.
- Se penche vers les animaux, jamais l'inverse ; murmure au moineau comme à une confidente.
- Se cache derrière ses mèches quand on la complimente.

**Réactions types**

- Face à la violence : sidérée, se raccroche au premier PJ venu ; mais l'empathie prend le dessus — elle pense d'abord aux blessés, même ennemis.
- Face à la négociation : laisse parler, puis lâche d'une petite voix la remarque qui débloque tout — sa naïveté désarme les interlocuteurs.
- Face à la flatterie : rougit, dénie, mais souvient — un compliment sincère la gagne pour longtemps.
- Face au mensonge : elle le sent plus qu'elle ne le démasque (empathie). Elle ne dit rien, mais son regard s'assombrit — et elle n'oublie pas.

**Conseils de RP**

- Levier émotionnel n°1 — la retrouvaille : pour rattraper le lien avec les PJ, fais de la quête « Retrouver Naelwyn » un moment où elle réalise qu'ils sont venus la chercher : c'est inattendu pour une reniée. Une seule larme discrète vaut mille mots.
- Doser le secret du destin : garde-le pour un moment de vulnérabilité (peur, nuit, blessure) — un PJ compatissant qui la rassure scellera l'amitié. La révéler trop tôt la transformerait en « mission », trop tard en froideur.
- La faire briller en petit : donne-lui une compétence modeste mais décisive (herboristerie, apaiser une bête, déchiffrer un signe druidique) — les joueurs adoptent vite le PNJ qui sauve la situation discrètement.
- Avec [[Sorenza]] : joue le contraste — la tenancière la fait sortir de sa coquille, la protège aussi ; l'Auberge du Chêne Vert peut devenir « son » endroit sûr à [[Mirenfeld]].
- Le moineau : use de lui comme d'un exutoire — elle lui confie ce qu'elle n'ose dire aux PJ ; les joueurs qui écoutent apprendront beaucoup en tendant l'oreille.