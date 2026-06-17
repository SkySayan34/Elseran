<%*
// Un petit prompt Templater pour nommer ta note proprement à la création
let title = tp.file.title;
if (title.startsWith("Untitled") || title === "Template PNJ") {
    title = await tp.system.prompt("Nom du PNJ :");
    await tp.file.rename(title);
}
-%>
---
type: PNJ
nom: <% title %>
statut: Vivant # [Vivant / Mort / Disparu / Inconnu]
faction:
fonction: 
lieu:  
alignement: 
race:
classe:
genre:
description:
date_de_création: <% tp.file.creation_date("YYYY-MM-DD") %>
---

# PNJ : <% title %>

> [!infobox]+ portrait
> ![[image_placeholder.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.current().faction` |
> | **Fonction** | `$= dv.current().fonction`
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
