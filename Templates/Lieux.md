<%*
// Prompt Templater pour nommer la note à la création
let title = tp.file.title;
if (title.startsWith("Untitled") || title === "Template Lieu") {
    title = await tp.system.prompt("Nom du Lieu :");
    await tp.file.rename(title);
}
-%>
---
type: lieu
nom: <% title %>
categorie: Ville # [Région / Ville / Quartier / Bâtiment / Donjon / Point d'intérêt]
parent:  # [Lien vers le lieu plus grand, ex: [[Sylve d'Aerwyn]] ou [[Nom de la Région]]]
population: 
factions_presentes: 
securite: # [Haute / Normale / Dangereux / Non civilisé]
cree_le: <% tp.file.creation_date("YYYY-MM-DD") %>
---

# Lieu : <% title %>

> [!infobox]+ carte
> ![[carte_placeholder.jpg|cover]]
> ###### Repères
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **Se trouve dans** | `$= dv.current().parent` |
> | **Sécurité** | `$= dv.current().securite` |
> | **Population** | `$= dv.current().population` |

## 🗺️ Description générale
*(Écris ici l'ambiance visuelle, l'architecture, le climat ou la première impression des joueurs en arrivant)*

- 

## 📜 Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

- 

## 🏠 Points d'intérêt (Sous-lieux)
*(Si c'est une ville : les tavernes, temples, boutiques. Si c'est une région : les villages, ruines, etc.)*

* **Point d'intérêt 1 :** Description rapide.
* **Point d'intérêt 2 :** Description rapide.

---

## 🛠️ Recensement local (Dataview)

### 👥 Habitants et PNJ présents
*Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter.*

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
WHERE contains(list(lieu), this.file.name) and (contains(type, "PNJ") or contains(type, "PJ"))
SORT file.name ASC
```
