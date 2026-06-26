<%*
let title = tp.file.title;
if (title.startsWith("Untitled")  | title === "Template Session") {
    let sessionNumber = await tp.system.prompt("Numéro de la session :");
    let sessionName = await tp.system.prompt("Titre de la session :");
    title = `Session ${sessionNumber} - ${sessionName}`;
    await tp.file.rename(title);
}

const campagne = await tp.system.suggester(["Chant des Cendres", "Contes en Elseran"], ["Chant des Cendres", "Contes en Elseran"]);
const arc = await tp.system.prompt("Arc associé :");
const chapitre = await tp.system.prompt("Chapitre associé :");
const dateReelle = tp.file.creation_date("YYYY-MM-DD");
const location = await tp.system.prompt("Lieu principal :");


tR += `---
type: session
world: Elseran
campagne: ${campagne}
arc: ${arc}
chapitre: ${chapitre}
date: ${dateReelle}
game_date: ${dateInGame}
location: ${location}
tags: #session
---

# ${title}

> [!infobox]
> | | |
> |---|---|
> | **Campagne** | \`= this.campagne \` |
> | **Arc** | \`= this.arc \` |
> | **Chapitre** | \`= this.chapitre \` |
> | **Date** | \`= this.date \` |
> | **Lieu** | \`= this.location \` |
`;
%>

## 📌 Résumé de la Session

^summary

---

## 🏠 Administration

- [ ]

---

## 🔄 Récapitulatif

![[<%*  
const files = app.vault.getMarkdownFiles()  
.filter(f => f.path.includes(`${campagne}/Sessions`) && f.basename !== title)  
.sort((a, b) => b.basename.localeCompare(a.basename));  
files.length > 0 ? files[0].basename : "Session Précédente"  
%>#^summary]]

---

## ✨ Accroche Forte

---

## 🎭 Scènes

- [ ] 

---

## 🔍 Secrets et Indices

- [ ] 

---

## 💰 Butin

- [ ] 

---

## 📜 Journal de Session

- 

