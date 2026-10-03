---
type: PNJ
statut: Vivant
faction: Conseil du Lien
fonction: Porteur des Marches
lieu: Géographie/Sylve d'Aerwyn/Frondains/Mirenfeld/Place du Serment
alignement: LB
race: Halfelin
classe:
genre: Homme
description:
tags: PNJ
---

# Brannos le Large



> [!infobox]+ portrait
> ![[Brannos le Large.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.fileLink(dv.current().faction)` |
> | **Fonction** | `$= dv.current().fonction` |
> | **Lieu** | `$= dv.fileLink(dv.current().lieu)` |
> | **Statut** | `$= dv.current().statut` |


##  Description & Psychologie

* **Apparence :** Halfelin rond comme une barrique, double menton souriant, gilet brodé aux couleurs des guildes, une bague « de marchand » par guilde. Petits yeux brillants qui voient tout, mains potelées à la poigne étonnante.

* **Personnalité :** Jovial, affable, rire gras, anecdotes sans fin. Ne dit jamais non : il dit « voyons voir ». Mais sous la bonhomie, il compte tout — chaque faveur est une dette future, et son carnet mental ne perd jamais une ligne.

* **Motivation principale :** Que le commerce coule et que l'harmonie de [[Mirenfeld]] dure — c'est bon pour les affaires. Sa position au Conseil avant tout.

* **Secrets / Ce qu'il cache :** 
	1) Il est l'intermédiaire secret de [[Zéphirae Anemoi]] pour l'acquisition des armes des anciens cycles (dont celle trouvée dans le [[Dhar'Zulun]]).
	2) Son réseau d'informateurs est plus étendu que quiconque ne l'imagine — même l'[[Ordre du Souffle]] serait surpris. Et il mentira sciemment aux PJ : « une acquisition pour le Conseil du Lien ».

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- Seul au Conseil à connaître le vol de l'arme. Il manœuvre la peine de service (échec du procès) ou l'entretien (réussite), et scelle l'accord par traité magique. 
- **Rôle dans l'intrigue** : La porte vers la piste de l'arme antique et du donjon du Culte du Néant — par la force en cas de condamnation, par gratitude en cas de blanchiment. Dans les deux cas, sa version officielle est un mensonge.

##  Relations & Connexions
* **Alliés :** Conseil du Lien ; guildes marchandes ; Cartel des Bateliers de l'[[Anserah]].
* **Ennemis :** Les contrebandiers (en public).
* **Réseau :** Informateurs urbains, du Creux de l'[[Anserah]] à [[Écorce-Haute]] ; secrètement, [[Zéphirae Anemoi]].

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

### Interprétation :

Voix chaude et forte, débit joyeux, interjections de marchand (« or pur ! », « sur ma bourse ! »). Il compte sur ses doigts pendant qu'on lui parle. Face à la violence : déçu par le manque de flair (« casse un pot, et tu n'auras plus de marché du tout »). Face au mensonge : il le sait déjà — et le laisse dire, ça agrandit la dette. La bonhomie est le masque : ne jamais le faire jouer en flagrant délit de méchanceté, seulement en flagrant délit de comptabilité.