---
type: PNJ
nom: Eredi Saerel
statut: Vivant
faction: "[[Ordre du Souffle]] ; [[Ordre des Scribes]]"
groupe: Scribe
lieu: "[[Mirenfeld]]"
alignement: LB
race: humain
classe:
genre: homme
description: Vieil érudit de l'[[Ordre du Souffle]] basé à [[Mirenfeld]]
date_de_création: 2026-06-15
---

# PNJ : Eredi Saerel

> [!infobox]+ portrait
> ![[Eredi, de l'odre du souffle.png|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.current().faction` |
> | **Fonction** | `$= dv.current().groupe`
> | **Lieu** | `$= dv.current().lieu` |
> | **Statut** | `$= dv.current().statut` |

## 👤 Description & Psychologie
* **Apparence :** Vieil humain à la longue barbe grise, portant des vêtements amples et sombres, typique des scribes. Il a une chevalière portant le blason de l'[[Ordre des Scribes]] et un pendentif de l'[[Ordre du Souffle]]. Ses yeux sont petits et pétillants de malices, bien qu'entourés de larges cernes se cachant derrière des lunettes ronde.
* **Personnalité :** Rieur, un peu fou, mais très sage.
* **Motivation principale :** Recueillir toutes les infos sur l'Histoire d'Elseran.
* **Secrets / Ce qu'il cache :** Il a par le passé fait un pacte avec un [[Démon]] pour acquérir un livre légendaire.

## 📝 Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- 

## 🔗 Relations & Connexions
* **Alliés :** [[Sorenza]]
* **Ennemis :** 
* **Réseau :** [[Ordre du Souffle]] ; [[Ordre des Scribes]] 

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
