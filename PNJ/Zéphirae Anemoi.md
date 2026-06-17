---
type: PNJ
nom: Zéphirae Anemoi
statut: Vivant
groupe: Chef de Guilde
lieu: "[[[Vhalarion Prime]] ; [[Vhalarion]]]"
faction: "[[Ordre du Souffle]]"
alignement: LN
date_de_création: 2026-06-13
---

# PNJ : Zéphirae Anemoi

> [!infobox]+ portrait
> ![[image_placeholder.jpg|cover]]
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
