<%*
let title = tp.file.title;
if (title.startsWith("Untitled")  | title === "Template Quête") {
    title = await tp.system.prompt("Nom de la quête :");
    await tp.file.rename(title);
}

const priorite = await tp.system.suggester(["Principale", "Secondaire", "Out"], ["Principale", "Secondaire", "Out"]);
const dateDebut = tp.file.creation_date("YYYY-MM-DD");

tR += `---
type: quête
nom: ${title}
campagne:
arc:
chapitre:
description:
statut: à venir
priorité: ${priorite}
date_debut: ${dateDebut}
tags: #quête
---

# ${title}

> [!infobox]
> | | |
> |---|---|
> | **Campagne** | \`= this.campagne \` |
> | **Arc** | \`= this.arc \` |
> | **Chapitre** | \`= this.chapitre \` |
> | **Statut** | \`= this.statut \` |
> | **Priorité** | \`= this.priorité \` |

## 📜 **Description**


`;
%>

##  **Objectifs**

- [ ]  Objectif principal
- [ ]  Point clé 1
- [ ]  Point clé 2

---

## 👥 **PNJ Impliqués**


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