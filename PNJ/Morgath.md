---
type: PNJ
statut: Vivant
faction: Voragine
fonction: Chef de Guilde
lieu: Géographie/Sylve d'Aerwyn/Frondains/Mirenfeld/Subracine/QG des Voragine
alignement: NM
race: Halfelin
classe:
genre: Homme
description: Halfelin chef de guilde de voleur dans subracines (mirenfeld)
tags: PNJ
---

# Morgath



> [!infobox]+ portrait
> ![[Morgath.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.fileLink(dv.current().faction)` |
> | **Fonction** | `$= dv.current().fonction` |
> | **Lieu** | `$= dv.fileLink(dv.current().lieu)` |
> | **Statut** | `$= dv.current().statut` |


##  Description & Psychologie

* **Apparence :** Halfelin des rives, petit et sec comme un galet, peau burlée par l'eau. Cheveux noirs plaqués en arrière, yeux gris-vert d'eau profonde. Habits sombres de coupe précise, bottes courtes cirées, chevalière de verre noir jamais retirée. Sourire rare, et effrayant.

* **Personnalité :** Taciturne, flegme de noyé. Parle du fleuve comme d'une personne : « l'[[Anserah]] a décidé ». Code des Fonds : ce que le fleuve avale lui revient — mais il ne noie personne lui-même : « le fleuve décide, pas moi ». Tient parole à la lettre. Marchand âpre, jamais cruel gratuitement.

* **Motivation principale :** Faire prospérer la Voragine en conservant sa neutralité entre les familles. En profondeur : il se croit redevable à l'[[Anserah]] — le fleuve l'a rendu, il lui doit quelque chose qu'il ne comprend pas encore.

* **Secrets / Ce qu'il cache :** 
	1) Enfant, son équipage l'a laissé pour mort — il a retrouvé chaque visage un à un, et « l'[[Anserah]] les a tous rendus à la rive ». 
	2) Il détient le contrat signé d'Ambroise, et il a reconnu un homme de loi de la Cour.

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- Laissé pour mort dans l'[[Anserah]], remonté du fond. Il a fait de la Voragine une guilde de voleurs professionnels, neutre et commerciale envers toutes les familles de la pègre. Le verre de son QG vient en sous-main de l'Éclat de Verre. 
- **Rôle dans l'intrigue** : Tient [[Naelwyn]] contre contrat. Viendra témoigner au procès, contrat en main, si les PJ le convainquent — leur performance décide de tout.

##  Relations & Connexions
* **Alliés :** [[Voragine]]
* **Ennemis :** Les familles qui voudraient absorber sa guilde.
* **Réseau :** Bateliers de l'[[Anserah]] ; l'Éclat de Verre ; contacts du Nid du Corbeau.

##  Coulisses du MJ
*Cette section se remplit automatiquement si d'autres notes (quêtes, sessions, rumeurs) mentionnent ce PNJ.*

### Quêtes liées

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM ""
WHERE type = "quête" AND contains(file.outlinks, this.file.link)
```


### Journal des rencontres

```dataview
LIST
FROM "" 
WHERE type = "session" AND contains(file.outlinks, this.file.link)
SORT file.name DESC
```

### Interprétation

Voix grave et plate, phrases très courtes, silences qui durent. Il regarde « à travers » ses interlocuteurs, vers l'eau. Face à la menace : « Le fleuve décide. Essayez. » Face à la négociation : très bon, mais il échange en services et en paroles tenues, rarement en or. Face à la flatterie : le prix monte. Levier émotionnel : si un PJ parle au nom du fleuve ou du Souffle, Morgath **écoute vraiment** — sa dette envers l'Anserah est sa seule porte sensible. Son formalisme à la lettre est exploitable : une promesse exactement formulée, il l'honore.