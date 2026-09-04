---
type: PJ
statut: Vivant
faction: Culte du Néant
fonction: Commandant en chef
lieu: Géographie/Elseran/Thal'Myrrun/Vhalren
alignement: N
race: Demi-Orc
classe: Occultiste
genre: Homme
description: Commandant en chef du Culte du Néant dédié à Dhargam, il dirige la sous-branche cherchant à détruire la matière.
date_de_création: 2026-08-11
---

# Disa Pear

> [!infobox]+ portrait
> ![[carte_placeholder.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `= link(this.faction)` |
> | **Fonction** | `= this.fonction` |
> | **Lieu** | `= link(this.lieu)` |
> | **Statut** | `= this.statut` |


##  Description & Psychologie

* **Apparence :** 
* **Personnalité :** 
* **Motivation principale :** 
* **Secrets / Ce qu'il cache :** 

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- ancien membre du clan [[Ertuk]] dans le [[Dhar'Zulun]]. Il est devenu chasseur de trésor, a voyagé un peu partout et a fini par rejoindre le [[Culte du Néant]] car il a compris que le monde atteignait sa fin et qu'il fallait l'aider à se réinitialiser.

##  Relations & Connexions
* **Alliés :** 
* **Ennemis :** 
* **Réseau :** 

##  Coulisses du MJ
*Cette section se remplit automatiquement si d'autres notes (quêtes, sessions, rumeurs) mentionnent ce PNJ.*

### Quêtes liées

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM "Chant des Cendres/Quêtes"
WHERE contains(file.outlinks, this.file.link)
```


### Journal des rencontres

```dataview
TABLE 
FROM #session 
WHERE contains(file.outlinks, this.file.link)
SORT file.ctime DESC
```
