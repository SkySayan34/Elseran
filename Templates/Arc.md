<%*
let title = tp.file.title;
if (title.startsWith("Untitled")  | title === "Template Arc") {
    title = await tp.system.prompt("Nom de l'arc :");
    await tp.file.rename(title);
}

const description = await tp.system.prompt("Description courte :");
const statut = await tp.system.suggester(["En cours", "Terminé", "À venir"], ["En cours", "Terminé", "À venir"]);
const dateDebut = tp.file.creation_date("YYYY-MM-DD");
const campagne = await tp.system.suggester(["Chant des Cendres", "Contes en Elseran"], ["Chant des Cendres", "Contes en Elseran"]);

tR += `---
type: arc
nom: ${title}
campagne: ${campagne}
world: Elseran
description: "${description}"
statut: ${statut}
date_debut: ${dateDebut}
---

# 🌌 ${title}

> [!infobox]
> | | |
> |---|---|
> | **Campagne** | \`= this.campagne \` |
> | **Statut** | \`= this.statut \` |
> | **Début** | \`= this.date_debut \` |

## 📜 **Résumé**

\`= this.description \`
`;
%>

## Chapitres

```dataview
TABLE description AS "Description", statut AS "Statut", date_debut AS "Début"
FROM "Chant des Cendres/Chapitres"
WHERE contains(arc, this.file.name)
SORT date_debut ASC
```

## Quêtes Associées

```dataview
TABLE description AS "Objectif", statut AS "Statut", priorité AS "Priorité"
FROM "Chant des Cendres/Quêtes"
WHERE contains(arc, this.file.name)
SORT priorité DESC, date_debut ASC
```

## PNJ impliqués

```dataview
TABLE nom AS "Nom", faction AS "Faction", fonction AS "Rôle"
FROM #PNJ OR "PNJ"
WHERE contains(file.outlinks, this.file.link) OR contains(quêtes, this.file.name)
SORT file.name ASC
```

## Lieux Principaux

```dataview
LIST
FROM #lieu OR "Géographie"
WHERE contains(file.outlinks, this.file.link)
SORT file.name ASC
```

