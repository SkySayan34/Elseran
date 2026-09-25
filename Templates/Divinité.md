<%*
// Prompt Templater pour nommer la note à la création
let title = tp.file.title;
if (title.startsWith("Sans titre") || title.startsWith("Untitled") || title === "Template Divinité") {
    title = await tp.system.prompt("Nom de la divinité :");
    await tp.file.rename(title);
}

tR += `---
type: divinité
rang: ${await tp.system.suggester(["Esprit mineur","Demi-dieu","Dieu mineur","Dieu majeur","Primordial"],["Esprit mineur","Demi-dieu","Dieu mineur","Dieu majeur","Primordial"])}
domaine:
tradition:
alignement: ${await tp.system.suggester(["LB","NB","CB","LN","N","CN","LM","NM","CM"],["LB","NB","CB","LN","N","CN","LM","NM","CM"])}
symbole:
lieu_de_culte:
statut: ${await tp.system.suggester(["Actif","Endormi","Exilé","Mort","Oublié"],["Actif","Endormi","Exilé","Mort","Oublié"])}
tags : divinité
---

# ✨ ${title}

`;

// Insertion de l'infobox APRES le frontmatter et le titre
tR += `
> [!infobox]+ symbole
> ![[carte_placeholder.jpg|cover]]
> ###### Fiche divine
> | | |
> | --- | --- |
> | **Rang** | \`$= dv.current().rang\` |
> | **Domaine** | \`$= dv.current().domaine\` |
> | **Tradition** | \`$= dv.current().tradition\` |
> | **Alignement** | \`$= dv.current().alignement\` |
> | **Statut** | \`$= dv.current().statut\` |
> | **Lieu de culte** | \`$= dv.fileLink(dv.current().lieu_de_culte)\` |

## 🌬️ Présentation & Manifestations
* **Apparence(s) / Avatars :** 
* **Symbole & signes :** 
* **Épithètes & autres noms :** 

## 🌀 Domaine & Pouvoirs
* **Sphère d'influence :** 
* **Ce qu'elle accorde :** *(Bénédictions, dons, faveurs...)*
* **Limites & interdits :** *(Ce qui dépasse sa portée ou relève d'un autre esprit/dieu)*

## 📜 Doctrine & Tabous
* **Ce qu'elle attend de ses fidèles :** 
* **Ce qui l'offense :** 

## 🕯️ Culte & Rites
* **Clergé / Serviteurs :** *(Druides, prêtres, ordres dédiés — lier vers les notes de faction)*
* **Lieux de culte :** 
* **Rites & célébrations :** *(Prières, offrandes, fêtes, périodes sacrées)*

## 🏛️ Histoire & Légendes
*(Mythes de création, faits historiques canon, légendes racontées par ses fidèles)*

- 

## ⚖️ Relations Divines
* **Alliés / Panthéon :** 
* **Rivaux / Ennemis :** 
* **Hiérarchie :** *(Sa place au sein des esprits druidiques ou de son panthéon)*

---

## 🛠️ Coulisses du MJ

### 🛡️ Cultes & factions liés

\`\`\`dataview
LIST
FROM #société 
WHERE contains(file.outlinks, this.file.link)
SORT file.name ASC
\`\`\`

### ⚔️ Quêtes liées

\`\`\`dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM #quête 
WHERE contains(file.outlinks, this.file.link)
\`\`\`

### 📓 Apparitions dans les sessions

\`\`\`dataview
TABLE campagne AS "Campagne"
FROM #session 
WHERE contains(file.outlinks, this.file.link)
SORT file.name DESC
\`\`\`
`;
-%>
