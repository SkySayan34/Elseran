---
type: PNJ
statut: Mort
faction:
fonction: Chef d'une troupe de braconniers
lieu: Vhalarion/Périphérie de Vhalarion Prime/Drey
alignement: NM
race: Humain
classe:
genre: Homme
description: Un braconnier arrogant et qui n'hésite pas à faire ce qu'il faut pour obtenir ce qu'il désire
date_de_création: 2026-09-06
---

# Garrick l'Ecorcheur

> [!infobox]+ portrait
> ![[Garrick l'Ecorcheur.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `= link(this.faction)` |
> | **Fonction** | `= this.fonction` |
> | **Lieu** | `= link(this.lieu)` |
> | **Statut** | `= this.statut` |


##  Description & Psychologie

* **Apparence :** Un homme d'âge moyen, au regard froid et calculateur. Il mâche un bout de racine amère
* **Personnalité :** Parle d'une voix posé mais tranchante, arrogant face aux aventuriers, opportuniste
* **Motivation principale :** Capturer [[Brak et Grum]] pour honorer son contrat de 600PO avec un seigneur voisin.
* **Secrets / Ce qu'il cache :** 

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- Son groupe et lui sont en chasse de ce monstre depuis quelques semaines, ils le traquent et ont finis par tomber sur son habitat. Ils ont tué la famille du Monstre pour l'appâter mais il s'est enfuit à [[Drey]]

##  Relations & Connexions
* **Alliés :** 
* **Ennemis :** [[Brak et Grum]]
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
