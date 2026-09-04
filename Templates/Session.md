<%*
let title = tp.file.title;
if (title.startsWith("Sans titre") || title.startsWith("Untitled")  | title === "Template Session") {
    let sessionNumber = await tp.system.prompt("Numéro de la session :");
    let sessionName = await tp.system.prompt("Titre de la session :");
    title = `Session ${sessionNumber} - ${sessionName}`;
    await tp.file.rename(title);
}

const campagne = await tp.system.prompt("Campagne ? : ")
const dateReelle = tp.file.creation_date("YYYY-MM-DD");

tR += `---
type: session
campagne: ${campagne}
arc:
chapitre:
date: ${dateReelle}
location:
---

# ${title}

> [!infobox]
> | | |
> |---|---|
> | **Campagne** | \`= link(this.campagne) \` |
> | **Arc** | \`= link(this.arc) \` |
> | **Chapitre** | \`= link(this.chapitre) \` |
> | **Date** | \`= this.date \` |
> | **Lieu** | \`= link(this.location) \` |
`;
%>

# Récapitulatif

<%*
// 1. Récupère toutes les sessions de la campagne
const allSessions = app.vault.getMarkdownFiles()
  .filter(f => f.path.includes(`${campagne}/Sessions`))
  .sort((a, b) => {
    const numA = parseInt(a.basename.split(" - ")[0].replace("Session ", ""));
    const numB = parseInt(b.basename.split(" - ")[0].replace("Session ", ""));
    return numA - numB; // Tri croissant (1, 2, 3...)
  });

// 2. Trouve l'index de la session actuelle
const currentIndex = allSessions.findIndex(f => f.basename === title);

// 3. Détermine la session précédente (ou "Session Précédente" si inexistante)
const previousSession = currentIndex > 0 ? allSessions[currentIndex - 1] : null;

// 4. Génère le lien vers la section #^summary de la session précédente
if (previousSession) {
  tR += `![[${previousSession.basename}#^summary]]`;
} else {
  tR += "";
}
%>

---

# Préparation de la Session

## Actes ou Scènes

### Description

### Choses à Faire

---

# Résumé de la Session



^summary

---

## 📜 Journal de Session

```dataview
LIST
FROM "${campagne}/Sessions"
SORT file.name DESC
```

