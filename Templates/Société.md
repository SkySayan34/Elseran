<%*
// Prompt Templater pour nommer la note à la création
let title = tp.file.title;
if (title.startsWith("Sans titre") || title.startsWith("Untitled") || title === "Template Faction") {
    title = await tp.system.prompt("Nom de la société :");
    await tp.file.rename(title);
}

tR += `---
type: faction
categorie: ${await tp.system.prompt("Catégorie :")}
quartier_general:
dirigeant: 
influence:  ${await tp.system.suggester(["Totale","Haute","Modérée","Faible","Secrète"],["Totale","Haute","Modérée","Faible","Secrète"])}
tags : société
---

# 🛡️ Organisation : ${title}
`;
-%>
> [!infobox]+ blason
> ![[carte_placeholder.jpg|cover]]
> ###### Fiche d'identité
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **QG Principal** | `$= dv.fileLink(dv.current().quartier_general)` |
> | **Dirigeant** | `$= dv.fileLink(dv.current().dirigeant)` |
> | **Influence** | `$= dv.current().influence` |


## 👁️ Présentation & Philosophie

* **Devise / Dicton :** 
* **Doctrine / Objectif :** 
* **Ressources & Moyens :** *(Richesse, armée, magie, réseau d'espionnage...)*

- 

## 📜 Histoire & Secrets
*(Les origines de la faction, ses anciens dirigeants, ses rivalités historiques et ce qu'elle cache au grand public)*

- 

## 🧭 Relations Extérieures

* **Alliés :** 
* **Rivalités / Ennemis :** 

---

## Registre des Membres

### 👥 Membres et Affiliés (PJ & PNJ)
*Cette liste est automatique. Elle utilise la méthode textuelle "blindée" pour trouver tous les PNJ et PJ dont la propriété `faction` contient le nom de cette note.*

```dataview
TABLE fonction AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
FROM #PNJ OR #PJ
WHERE contains(faction, this.file.name)
SORT file.name ASC
```
