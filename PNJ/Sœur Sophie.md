---
type: PNJ
nom: Sœur Sophie
statut: Vivant
faction: "[[Ordre Impérial de la Lumière]]"
fonction: Soeur
lieu: "[[Géographie/Sylve d'Aerwyn/Mirenfeld/Mirenfeld]]"
alignement: LM
race: humaine
classe: clerc
genre: Femme
description:
date_de_création: 2026-06-15
---

# PNJ : Sœur Sophie

> [!infobox]+ portrait
> ![[Soeur Sophie.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.current().faction` |
> | **Fonction** | `$= dv.current().fonction`
> | **Lieu** | `$= dv.current().lieu` |
> | **Statut** | `$= dv.current().statut` |

## 👤 Description & Psychologie
* **Apparence :** Une femme humaine d'une trentaine d'années, à la posture incroyablement droite, presque rigide. Elle dégage une aura de sévérité glaciale et de dignité impériale. Elle porte une robe de bure immaculée de l'Ordre Impérial, lourde et sans fioritures, serrée à la taille par une corde de chanvre. À son cou pend un lourd médaillon de bronze représentant le symbole de son culte. Ses mains sont calleuses, et ses ongles sont coupés ras, souvent rougis par le froid ou le frottement de ses chapelets.

* **Personnalité :** Charismatique, austère, regard fiévreux. Elle parle avec une voix théâtrale qui captive les foules. Elle méprise profondément le métissage culturel de Mirenfeld.
* **Motivation principale :** Purger la ville de sa "décadence".
* **Secrets / Ce qu'il cache :**  Elle orchestre les meurtres et mutile les corps pour faire accuser l'[[Auberge des Abysses]] et forcer le [[Conseil du Lien à le fermer.

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
