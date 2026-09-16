---
type: PNJ
statut: Vivant
faction:
fonction:
lieu: Vhalarion/Périphérie de Vhalarion Prime/Drey
alignement: CN
race: Ettin
classe:
genre: Homme
description: Un Ettin (descendant géant bicéphale) pourchassé par des braconniers
date_de_création: 2026-09-06
---

# Brak et Grum

> [!infobox]+ portrait
> ![[Brak et Grum.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `= link(this.faction)` |
> | **Fonction** | `= this.fonction` |
> | **Lieu** | `= link(this.lieu)` |
> | **Statut** | `= this.statut` |


##  Description & Psychologie

* **Apparence :** Monstre de 3m de haut à deux têtes. Celle de gauche a les dents du bas qui ressortent, et les sourcils toujours froncés, tandis que celle de droite a un léger strabisme et a le regard suppliant.
* **Personnalité :** Grum est agressif, méfiant, Brak est plaintif, suppliant et s'exprime comme un enfant.
* **Motivation principale :** Trouver un refuge vers Khor'Thélûn.
* **Secrets / Ce qu'il cache :** 

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- 

##  Relations & Connexions
* **Alliés :** 
* **Ennemis :** [[Garrick l'Ecorcheur]]
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
