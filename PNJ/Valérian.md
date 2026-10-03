---
type: PNJ
nom: Valérian
statut: Vivant
faction:
fonction: Tenancier de l'[[Auberge des Abysses]]
lieu: "[[Mirenfeld]]"
alignement: N
race: demi elfe
classe:
genre: homme
description:
date_de_création: 2026-06-15
---

# PNJ : Valérian

> [!infobox]+ portrait
> ![[Valérian.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.current().faction` |
> | **Fonction** | `$= dv.current().fonction`
> | **Lieu** | `$= dv.current().lieu` |
> | **Statut** | `$= dv.current().statut` |

## 👤 Description & Psychologie
* **Apparence :** Demi-elfe élancé aux gestes théâtraux. Cheveux argentés, khôl noir intense autour des yeux, bouc impeccable. Porte un grand manteau de velours noir doublé de pourpre et de nombreuses bagues en pacotille.
* **Personnalité :** Excentrique, habillé de soie noire, grandiloquent. C'est un pur businessman du spectacle qui adore provoquer les bien-pensants, mais il s'évanouit à la vue d'une vraie goutte de sang.
* **Motivation principale :** Protéger sa réputation, remplir sa salle et prouver son innocence sans que la garde n'inspecte trop ses affaires.
* **Secrets / Ce qu'il cache :** il fraude un peu les taxes.

## 📝 Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- 

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
