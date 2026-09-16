---
type: PNJ
statut: Vivant
faction:
fonction: Antiquaire
lieu: Elseran/Sylve d'Aerwyn/Frondains/Mirenfeld/Quais des Mondes
alignement: N
race: Elfe noir
classe:
genre: Homme
description: Un efle noir proposant de nombreux vestiges et babioles de tout temps. Il est généralement accompagné de son corbeau.
date_de_création: 2026-08-11
---

# Kael'Thir Ombreplume

> [!infobox]+ portrait
> ![[Kael'Thir Ombreplume.png]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `= link(this.faction)` |
> | **Fonction** | `= this.fonction` |
> | **Lieu** | `= link(this.lieu)` |
> | **Statut** | `= this.statut` |


##  Description & Psychologie

* **Apparence :** Elfe noir, portant une vieille armure de cuire et une cape sombre. Ses cheveux sont blancs, il a un regard compatissant et sage comme s'il avait vu le monde depuis ses débuts. Il a toujours son corbeau à portée.
* **Personnalité :** Calme et serein, il a l'air toujours un peu ailleurs.
* **Motivation principale :** Comprendre l'histoire d'Elseran à travers les artefacts qu'il trouve.
* **Secrets / Ce qu'il cache :** Son corbeau est son ancienne compagne qu'il a enfermé dans ce corps afin de l'épargner d'une malédiction qu'une de ces trouvailles lui a infligé.

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- A voyagé en Elseran durant sa jeunesse, et a découvert de nombreuses légendes faisant mentions de l'histoire des Dieux Fondateurs et des cycles se répétant, mais n'y a absolument rien compris.
- A trouvé un objet lui permettant d'avoir une révélation concernant un artefact divin. Cependant le coût fut de donner l'âme de la personne lui étant le plus cher à [[Ren'Morûn]]

##  Relations & Connexions

* **Alliés :** 
* **Ennemis :** 
* **Réseau :** 

##  Coulisses du MJ
*Cette section se remplit automatiquement si d'autres notes (quêtes, sessions, rumeurs) mentionnent ce PNJ.*

### Quêtes liées

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM #quete
WHERE contains(file.outlinks, this.file.link)
```


### Journal des rencontres

```dataview
Table link(campagne) as "Campagne", link(arc) as "Arc", link(chapitre) as "Chapitre"
FROM #session 
WHERE contains(file.outlinks, this.file.link)
SORT file.ctime DESC
```
