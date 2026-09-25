---
type: faction
categorie: Clan du Dhar'Zulun
quartier_general:
dirigeant: Varlag
influence: Faible
tags: société
---
# 🛡️ Organisation : Clan de Rukh-Tarr

> [!infobox]+ blason  
> ![[Rukh-Tarr.jpg|cover]]
> 
> ###### Fiche d'identité
> 
> |   |   |
> |---|---|
> |||
> |**Catégorie**|`$= dv.current().categorie`|
> |**QG Principal**|`$= dv.fileLink(dv.current().quartier_general)`|
> |**Dirigeant**|`$= dv.fileLink(dv.current().dirigeant)`|
> |**Influence**|`$= dv.current().influence`|

## 👁️ Présentation & Philosophie

- **Devise / Dicton :** _« Le compte se règle de main, pas de bouche. »_
    
- **Doctrine / Objectif :** _(inventé — modifiable)_ Clan orc de taille moyenne du [[Dhar'Zulun]], rattaché à la lignée de Rukh — des pasteurs et pillards de dunes profondes, réputés pour leur férocité et leur impatience envers les longues récitailles de comptes. Ils payaient leurs dettes, mais à contrecœur : chez les Rukh-Tarr, on murmurait depuis des générations que les [[Veilleurs d'Ocre]] avaient « volé aux clans le droit de régler leurs comptes eux-mêmes ».
    
- **Ressources & Moyens :** Chevaux de sables, quelques puits secondaires dans les Dunes ; aucune alliance durable — leur arrogance tribale les tenait à l'écart des grandes coalitions.
    

- Le clan vécut environ **un siècle après la [[Guerre des Sables]]**, à une époque où les clans avaient presque oublié ce que le désert était avant le [[Glossaire#Le Prix du Sang - Code des Clans Nomades du Dhar'Zulun|Prix du Sang]].
    

## 📜 Histoire & Secrets

- **L'apogée et la chute.** Le clan connut sa sombre apogée sous [[Varlag]], chef de guerre couvert de brands, « à jour de comptes » — ce qui rendait sa rébellion d'autant plus insoutenable pour la caste. Lorsqu'il estima qu'une dette de sang dormait impayée depuis la Grande Lassitude (un frère tué, mal comptée selon lui), il marcha jusqu'à la [[Faille d'Ocre]] avec sa garde des Dix-Neuf pour verser lui-même le sang d'un débiteur réfugié.
    
- **L'effacement.** Varlag tua le vieil orc sur le seuil de la Faille — un meurtre rituellement « gratuit », donc monstrueux. Le tabou fit le reste : la coalition de **tous** les clans du désert traqua et effaça le clan de Rukh-Tarr en une seule saison. Les Dix-Neuf furent livrés vivants aux lignées créancières ; Varlag périt le dernier, dit-on, en refusant de prononcer le compte de son propre sang. Le nom de Rukh-Tarr n'est plus récité dans aucune Veillée — l'effacement complet, pire que la mort.
    

## 🧭 Relations Extérieures

- **Alliés :** Aucun — c'est ce qui les perdit : lorsqu'est venu le temps de l'effacement, aucun clan ne prit leur défense, pas même par calcul.
    
- **Rivalités / Ennemis :** La caste des [[Veilleurs d'Ocre]] (par la faute de Varlag, non la leur) ; potentiellement toutes les lignées créancières du désert, qui se partagèrent leurs terres et leurs puits après l'effacement.
    

---

## Registre des Membres

### 👥 Membres et Affiliés (PJ & PNJ)

_Cette liste est automatique. Elle utilise la méthode textuelle "blindée" pour trouver tous les PNJ et PJ dont la propriété_ `_faction_` _contient le nom de cette note._

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
FROM #PNJ or #PJ
WHERE contains(list(faction), this.file.name)
SORT file.name ASC
```
