---
type: PNJ
statut: Vivant
faction: Conseil du Lien
fonction: Scribe du Souffle
lieu: Géographie/Sylve d'Aerwyn/Frondains/Mirenfeld/Anneau des Maîtres/Athenaeum de Myrrha
alignement: LN
race: Gnome
classe:
genre: Homme
description: Vieux Gnome trapu, siégeant au conseil du Lien, scribe du souffle.
tags: PNJ
---

# Nhyrel de Myrrha



> [!infobox]+ portrait
> ![[Nhyrel de Myrrha.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.fileLink(dv.current().faction)` |
> | **Fonction** | `$= dv.current().fonction` |
> | **Lieu** | `$= dv.fileLink(dv.current().lieu)` |
> | **Statut** | `$= dv.current().statut` |


##  Description & Psychologie

* **Apparence :** Gnome trapu d'un siècle, barbe grise fourchue soigneusement peignée, moustache cirée, petits yeux noirs perçants. Robe de laine grise à galon d'or du Conseil, chaîne de sceaux du Serment à la ceinture, doigts tachés d'encre ancienne.

* **Personnalité :** Sobre, cérémonieux, précis à l'excès. Répète mot pour mot la phrase qu'on vient de lui adresser avant de répondre. Cite des références d'archives datées. Courtois mais impitoyable avec l'imprécision. Jamais de colère : au pire, un silence et une référence supplémentaire.

* **Motivation principale :** Que la mémoire de la cité ne dépende jamais d'un seul homme — achever l'archive parfaite de l'Athenaeum et appliquer le Serment à la lettre.

* **Secrets / Ce qu'il cache :** 
	1) Il sent une dissonance dans les échos d'Ambroise depuis des mois, mais n'en a parlé à personne : accuser un assesseur impérial sans preuve le rendrait suspect de partialité sylvestre.
	2) Sa mémoire commence, pour la première fois, à lui faire défaut — des brèves défaillances qu'il cache avec terreur.

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

-Son dicton populaire de « mémoire absolue » n'est qu'une excellente mémoire, fruit d'une vie d'archives. Il tire son nom de Myrrha, déesse fondatrice du savoir et de la magie. Rôle dans l'intrigue : Préside le procès de [[Vox Cineris]] (16h, Athenaeum). Sa mémoire ne peut pas détecter les omissions — les PJ lui apportent la pièce manquante. Après l'exposition du complot, il les remercie et les met en relation avec Brannos le Large.


##  Relations & Connexions
* **Alliés :** Collège des Chantres d'Écorce ; Loge des Hauts-Druides.
* **Ennemis :** Aucun déclaré — Ambroise l'exploite à son insu.
* **Réseau :** Archivistes de l'Athenaeum, scribes de la Cour des Échos.

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

### Interprétation:

Voix posée, débit lent et régulier, comme une lecture publique. Il ne discute jamais : il cite. Ses silences sont des citations qu'il ne prononce pas. Face à la violence : un constat neutre, puis « Cela sera archivé ». Face au mensonge : aucune réaction visible — mais les PJ devraient sentir que tout se note. Levier émotionnel : s'ils l'observent bien, ils peuvent le surprendre en train de **vérifier ses propres registres** — l'homme-écho qui n'ose plus se fier à son écho.