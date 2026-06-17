---
tags:
  - pnj
  - mort
  - archidruide
  - druide
groupe:
type: PNJ
lieu:
description: Vieil archidruide du cercle de [[Khor'Vélyss]], à l'origine du [[Serment des Racines]]
race: Elfe sylvestre
genre: homme
classe: druide
nom: Oakhaven
statut: Mort
faction: Cercle de [[Khor'Vélyss]]
alignement: LB
premiere_rencontre: 2026-06-07
---

# PNJ : Oakhaven

> [!infobox]+ portrait
> ![[Oakhaven.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.current().faction` |
> | **Lieu** | `$= dv.current().lieu` |
> | **Statut** | `$= dv.current().statut` |

## 👤 Description & Psychologie
* **Apparence :** 
* **Personnalité :** 
* **Motivation principale :** 
* **Secrets / Ce qu'il cache :** 

## 📝 Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

Oakhaven était un vénérable [[Archidruide]] du Cercle de [[Khor'Vélyss]]. Figure de sagesse et de tempérance au sein de la [[Sylve d'Aerwyn]], il consacra sa longue existence à la préservation de l'Équilibre. 

Parmi ses hauts faits historiques, il fut le principal artisan de la paix à la fin de la [[Guerre des Racines]], agissant comme l'arbitre et le témoin sacré du [[Serment des Racines]]. Ses mémoires et ses paroles prononcées lors de cette nuit historique sont précieusement consignées dans les [[Chroniques Sylvestres]].


## 🔗 Relations & Connexions
* **Alliés :** 
* **Ennemis :** 
* **Réseau :** 

## 🛠️ Coulisses du MJ (Dataview)
*Cette section se remplit automatiquement si d'autres notes (quêtes, sessions, rumeurs) mentionnent ce PNJ.*

### Quêtes liées
```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM #quete or "Suivi de Campagne"
WHERE contains(pnj, this.file.link)
```
### Journal des rencontres
```dataview
LIST
FROM "Sessions" or #session
WHERE contains(file.outlinks, this.file.link)
SORT file.ctime DESC
```
