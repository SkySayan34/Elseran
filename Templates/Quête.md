<%*
let title = tp.file.title;
if (title.startsWith("Untitled")  | title === "Template Quête") {
    title = await tp.system.prompt("Nom de la quête :");
    await tp.file.rename(title);
}

const description = await tp.system.prompt("Description courte :");
const statut = await tp.system.suggester(["En cours", "Terminé", "Échoué", "À venir"], ["En cours", "Terminé", "Échoué", "À venir"]);
const priorite = await tp.system.suggester(["Haute", "Moyenne", "Basse"], ["Haute", "Moyenne", "Basse"]);
const dateDebut = tp.file.creation_date("YYYY-MM-DD");
const campagne = await tp.system.suggester(["Chant des Cendres", "Contes en Elseran"], ["Chant des Cendres", "Contes en Elseran"]);
const arc = await tp.system.prompt("Arc associé (optionnel) :");
const chapitre = await tp.system.prompt("Chapitre associé (optionnel) :");

tR += `---
type: quête
nom: ${title}
campagne: ${campagne}
arc: ${arc}
chapitre: ${chapitre}
world: Elseran
description: "${description}"
statut: ${statut}
priorité: ${priorite}
date_debut: ${dateDebut}
---

# 🎯 ${title}

> [!infobox]
> | | |
> |---|---|
> | **Campagne** | \`= this.campagne \` |
> | **Arc** | \`= this.arc \` |
> | **Chapitre** | \`= this.chapitre \` |
> | **Statut** | \`= this.statut \` |
> | **Priorité** | \`= this.priorité \` |
> | **Début** | \`= this.date_debut \` |

## 📜 **Description**

\`= this.description \`
`;
%>

## 🎯 **Objectifs**

- [ ]  Objectif principal
- [ ]  Objectif secondaire
- [ ]  Objectif optionnel

---

## 👥 **PNJ Impliqués**

_(Ce champ est utilisé par la requête dans ton template PNJ existant)_

- 

---

## 🗺️ **Lieux Associés**

- 

## **Sessions**

```dataview
LIST
FROM "${campagne}/Sessions"
WHERE contains(file.outlinks, this.file.link)
SORT date ASC
```
## 📌 **Récompenses**

- **Expérience** :
- **Butin** :
- **Autres** :

