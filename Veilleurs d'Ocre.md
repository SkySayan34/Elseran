---
type: faction
categorie: Caste Sacrée
quartier_general: Géographie/Dhar'Zulun/La Faille d'Ocre
dirigeant: La Voix-du-Compte
influence: Haute
tags:
  - société
---


# 🛡️ Organisation : Les Veilleurs d'Ocre

> [!infobox]+ blason
> ![[Veilleurs d'Orcre.jpg|cover]]
> ###### Fiche d'identité
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **QG Principal** | `$= dv.fileLink(dv.current().quartier_general)` |
> | **Dirigeant** | `$= dv.current().dirigeant` |
> | **Influence** | `$= dv.current().influence` |

## 👁️ Présentation &amp; Philosophie

- **Devise / Dicton :** *« Le sang versé n'est jamais perdu ni gagné — il est dû. »* / *« Seul celui qui n'appartient à aucun clan peut tenir les comptes de tous. »*

- **Doctrine / Objectif :** Les Veilleurs d'Ocre sont la caste sacrée du [[Glossaire#Le Prix du Sang - Code des Clans Nomades du Dhar'Zulun|Prix du Sang]] le code d'honneur commun aux clans orcs du [[Dhar'Zulun]]. Ils ne gouvernent rien et ne commandent personne : ils **tiennent la comptabilité du sang** du désert entier. Leur unique mission : qu'aucune goutte de sang versée ne soit oubliée, et qu'aucune dette ne meure impayée ou impunie. Graver les brands, réciter les dettes, arbitrer les déclarations de guerre et prononcer les quittances — voilà tout leur pouvoir, et il n'en existe pas de plus grand dans le désert.

- **Ressources &amp; Moyens :** Aucune armée, aucun trésor — et c'est leur force. Leur unique ressource est **l'inviolabilité** : tuer un Veilleur est le seul crime qui fait d'un clan entier l'ennemi de tous les autres. Aucun clan, même puissant, n'a jamais survécu à ce tabou. Ils possèdent en outre la **mémoire rituelle** : des générations de comptes récités par cœur à chaque Veillée du Serment, une tradition orale plus fiable que n'importe quelle archive. Leurs instruments : le fer à marquer, l'ocre rouge des rites, et la parole solennelle.

- **Le serment.** On naît Veilleur (par lignée de Veilleurs) ou on y entre par vocation reconnue. Le serment impose la **renonciation au nom de clan.** Il est interdit d'hériter, de commander, de prendre part à un duel ou de verser le sang. Sa dette personnelle est transférée à la caste, qui l'acquitte par son service.

- **Les rangs :**
	- **Les Éveilleurs** — apprentis, souvent enfants ; ils apprennent la récitation et le décompte.
	
	- **Les Tourneurs de Pages** — Veilleurs itinérants, en résidence permanente auprès de chaque clan ; ils récitent les comptes aux Veillées locales et gravent les brands.
	
	- **Les Voix-du-Compte** — la plus haute voix, qui préside la \[\[03-01|Veillée du Serment\]\] annuelle et prononce les quittances. Une seule par génération, sans clan et sans nom d'avant.
	
	- **La Veillée du Serment.** À chaque cycle, tous les Veilleurs du désert se réunissent en lieu neutre pour entendre les récits de l'année, établir officiellement ce que chaque clan doit, prononcer les quittes et les gels. La décision d'un Veilleur ne se conteste pas.

## 📜 Histoire &amp; Secrets

- **Les origines.** Les clans orcs racontent que le Prix du Sang naquit après la \[\[Guerre des Sables\]\], une guerre d'extermination qui faillit éteindre tous les clans du désert : des générations de vengeance sans fin, jusqu'à ce que les belligérants, épuisés, imposent un arbitre à chacun de leurs clans — et que ces arbitres, découvrant qu'ils ne pouvaient être justes que détachés, renoncent ensemble à leurs noms. Les premiers Veilleurs furent ces renégats sacrés.

- **La [[Faille d'Ocre]].** Leur QG est un canyon minéral du [[Dhar'Zulun]] aux parois teintées d'ocre rouge, neutralisé depuis des générations : aucune razzia, aucune guerre déclarée ne peut y pénétrer. Les clans y déposent les orphelines et orphelins destinés à la caste.

## 🧭 Relations Extérieures

- **Alliés :** Aucun — par principe. Ils sont au-dessus des clans, pas à leurs côtés.

- **Rivalités / Ennemis :** Aucun clan ne leur est ennemi. Seuls quelques chefs ou seigneurs de guerre **contestent leur autorité** en silence, et leurs noms sont soigneusement retenus par les Voix-du-Compte. La rumeur dit aussi que certains Veilleurs en résidence chez les Ertuk et chez les Zarka entretiennent, chacun de leur côté, un dialogue discret sur la dette fratricide jamais soldée.

---

## Registre des Membres

### 👥 Membres et Affiliés (PJ &amp; PNJ)

*Cette liste est automatique. Elle utilise la méthode textuelle "blindée" pour trouver tous les PNJ et PJ dont la propriété `faction` contient le nom de cette note.*

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
FROM #PNJ AND #PJ
WHERE contains(list(faction), this.file.name)
SORT file.name ASC
```