---
type: PNJ
nom: Sorenza
statut: Vivant
faction: "[[Ordre du Souffle]]"
groupe: Tenancière de l'[[Auberge du Chêne Vert]]
lieu: "[[Auberge du Chêne Vert]]"
alignement: NB
race: Tabaxi
classe:
genre: Femme
description: La tenancière provoquante de l'Auberge du Chêne Vert, point de contact de l'Ordre du Souffle de Mirenfeld.
date_de_création: 2026-06-15
---

# PNJ : Sorenza

> [!infobox]+ portrait
> ![[Sorenza la tenanciere du chene vert.png|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.current().faction` |
> | **Lieu** | `$= dv.current().lieu` |
> | **Statut** | `$= dv.current().statut` |

## 👤 Description & Psychologie
* **Apparence :** Une tabaxi léopard, habillée de vêtements larges et simple, le sourire aussi large que son décolleté provocateur, une chevelure noire bouclée, un regard félin comme si elle observait sa proie avant l'assaut. Elle a plein de bijoux grodiloquents 
* **Personnalité :** Provocatrice, parle fort, et rit aussi fort, mais très perspicace.
* **Motivation principale :** Protéger son auberge, et aider l'Ordre du Souffle et ses aventuriers.
* **Secrets / Ce qu'il cache :** est une ancienne aventurière ayant dû tuer son groupe qui était corrompu.

## 📝 Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- 

## 🔗 Relations & Connexions
* **Alliés :** [[Eredi Saerel]]
* **Ennemis :** 
* **Réseau :** [[Ordre du Souffle]]

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
