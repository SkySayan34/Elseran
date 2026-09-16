<%*
// Un petit prompt Templater pour nommer ta note proprement à la création
let title = tp.file.title;
if (title.startsWith("Sans titre") || title.startsWith("Untitled") || title === "Template PNJ") {
    title = await tp.system.prompt("Nom du PNJ :");
    await tp.file.rename(title);
}

tR += `---
type: PNJ
statut: ${await tp.system.suggester(["Vivant","Mort","Disparu","Inconnu"],["Vivant","Mort","Disparu","Inconnu"])}
faction:
fonction:
lieu:
alignement: ${await tp.system.suggester(["LB","NB","CB","LN","N","CN","LM","NM","CM"],["LB","NB","CB","LN","N","CN","LM","NM","CM"])}
race: ${await tp.system.prompt("Quelle Race ?")}
classe: ${await tp.system.prompt("Quelle Classe ?")}
genre: ${await tp.system.suggester(["Homme","Femme","Non-Binaire"],["Homme","Femme","Non-Binaire"])}
description:
tags : PNJ
---

# ${title}


`;
-%>

> [!infobox]+ portrait
> ![[carte_placeholder.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.fileLink(dv.current().faction)` |
> | **Fonction** | `$= dv.current().fonction` |
> | **Lieu** | `$= dv.fileLink(dv.current().lieu)` |
> | **Statut** | `$= dv.current().statut` |


##  Description & Psychologie

* **Apparence :** 
* **Personnalité :** 
* **Motivation principale :** 
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
