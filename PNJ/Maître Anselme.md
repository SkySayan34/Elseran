---
type: PNJ
statut: Vivant
faction: Mestre de village de l'Empire
fonction: Bourgmestre de Drey
lieu: Vhalarion/Périphérie de Vhalarion Prime/Drey
alignement: LB
race: Humain
classe:
genre: Homme
description:
date_de_création: 2026-09-04
---

# Maître Anselme

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

* **Apparence :** Homme longue barbe poivre et sel, lunettes en demi-lune, traits du visage fatigués.
* **Personnalité :** Voix anxieuse, se frotte nerveusement les mains, sent la bière aigre et le cuir mouillé.
* **Motivation principale :** Veut sécuriser le village au plus vite avant l'arrivée du percepteur impérial. Offre 250 po pour la tête du monstre.
* **Secrets / Ce qu'il cache :** 

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- 

##  Relations & Connexions
* **Alliés :** 
* **Ennemis :** 
* **Réseau :** 

##  Coulisses du MJ
*Cette section se remplit automatiquement si d'autres notes (quêtes, sessions, rumeurs) mentionnent ce PNJ.*

### Quêtes liées

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM #quête
WHERE contains(file.outlinks, this.file.link)
```


### Journal des rencontres

```dataview
LIST
FROM "" 
WHERE type = "session" AND contains(file.outlinks, this.file.link)
SORT file.name DESC
```
