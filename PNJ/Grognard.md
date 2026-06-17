---
type: PNJ
nom: Grognard
statut: Vivant
faction:
fonction: videur de la [[Taverne des Abysses]]
lieu: "[[Mirenfeld]]"
alignement: N
race: Goliath
classe:
genre: homme
description:
date_de_création: 2026-06-15
---

# PNJ : Grognard

> [!infobox]+ portrait
> ![[Grognard.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.current().faction` |
> | **Fonction** | `$= dv.current().fonction`
> | **Lieu** | `$= dv.current().lieu` |
> | **Statut** | `$= dv.current().statut` |

## 👤 Description & Psychologie
* **Apparence :** - Colosse chauve aux épaules démesurées. Visage carré marqué par une longue cicatrice sur la joue, air profondément ennuyé. Porte un gilet de cuir noir clouté révélant des **bras massifs et tatoués**.
* **Personnalité :** Peu bavard, professionnel, mais secrètement fan des pièces de théâtre du cabaret.
* **Motivation principale :** Éviter les bagarres et filtrer les clients à l'entrée.
* **Secrets / Ce qu'il cache :** il joue parfois la "Goule n°3" sur scène.

## 📝 Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- 

## 🔗 Relations & Connexions
* **Alliés :** [[Valérian]]
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
