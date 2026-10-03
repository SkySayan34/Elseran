---
type: PNJ
statut: Vivant
faction: Ordre Impérial de la Lumière
fonction:
lieu: Géographie/Sylve d'Aerwyn/Frondains/Mirenfeld/Anneau des Maîtres/Athenaeum de Myrrha
alignement: LM
race: Humain
classe:
genre: Homme
description: Homme fin et sec de 40 ans, appartenant à l'Ordre Impérial de la Lumière.
tags: PNJ
---

# Ambroise de Valcourt



> [!infobox]+ portrait
> ![[Ambroise de Valcourt.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.fileLink(dv.current().faction)` |
> | **Fonction** | `$= dv.current().fonction` |
> | **Lieu** | `$= dv.fileLink(dv.current().lieu)` |
> | **Statut** | `$= dv.current().statut` |


##  Description & Psychologie

* **Apparence :** Homme sec d'une quarantaine d'années, élégance impériale sobre : pourpre presque effacé, gants gris de chevreau fin, manches boutonnées jusqu'au poignet. Cheveux châtain tirés, barbe taillée à la mode de [[Vhalarion Prime]]. Parfum de qualité sous lequel flotte l'encens. Cicatrice de cire ancienne au poignet gauche, sous le gant.

* **Personnalité :** Zèle froid. Voix basse, courtoisie de marbre. Ne ment jamais frontalement — il omet. Le silence comme arme. Ferveur intime qui transpire par petites fuites : psaume murmuré, tic de frotter son poignet gauche quand on touche un sujet de foi.

* **Motivation principale :** Venger [[Sœur Sophie]] et achever son œuvre — faire de ce procès la mise à mort légale de l'[[Ordre du Souffle]] à [[Mirenfeld]], premier pas de la purification de la cité.

* **Secrets / Ce qu'il cache :** 
	1) Il savait pour les purifications de [[Sœur Sophie]] et les couvrait — preuve qui le détruirait.
	2) La Veillée de Cire : un registre où chaque cierge éteint de sa main nue est une « offense de la cité » qu'il compte rayer un jour.
	3) Il a engagé la Voragine en personne — le contrat existe, détenu par la guilde.

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

- Très proche de [[Sœur Sophie]], complice passif de son activisme de purification. Son deuil l'a radicalisé : la vengeance légale d'abord, l'ombre ensuite.
- **Rôle dans l'intrigue** : Retourne le carnet de Sophie contre les PJ à l'audience ; commanditaire de l'enlèvement de [[Naelwyn]] ; veut des aveux publics → scandale → expulsion de l'[[Ordre du Souffle]] de [[Mirenfeld]].

##  Relations & Connexions
* **Alliés :** 
* **Ennemis :** [[Vox Cineris]] (instrument) ; l'[[Ordre du Souffle]] (cible).
* **Réseau :** Les greffes de la Cour ; les milieux dévots impériaux.

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

### Interprétation :

Voix basse, débit lent, silences longs, accent de la capitale légèrement appuyé. Jamais un geste de trop. Face à l'agression : pas un muscle, un mot de plus bas encore. Face à la flatterie : un sourire de marbre. La menace est dans le calme, jamais dans l'éclat. Quand il est démasqué au procès : pas de rage — un seul aveu de foi, murmuré, qui glace la salle. Tics de table : il frotte son poignet gauche, boutonne sa manche, psalmodie à mi-voix en refermant un dossier.