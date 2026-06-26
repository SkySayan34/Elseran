---
tags:
  - lore/géographie
  - elseran
  - region
  - sylve
type: lieu
nom: Sylve d'Aerwyn
categorie: Région
parent: "[[Elseran]]"
population: "[[elfes]] [[gnomes]] [[halfelins]] [[humains]]"
factions_presentes: "[[Galavorn]] [[Aeriel]] [[Cercle Druidique]] [[Ordre du Souffle]]"
securite:
cree_le: 2026-05-23
---

# 📍 Lieu : Sylve d'Aerwyn

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

- **Titres :** Le Souffle Vert, la Mémoire Sylvestre
- **Position :** Nord-Ouest d'[[Elseran]]. Sa frontière est marquée au sud par le fleuve sacré [[Anserah]], et à l'est par la haute chaîne des [[Monts d'Elseran|Hauts de Vhalûr]].
- **Climat :** Tempéré et humide, caractérisé par des brumes permanentes et des pluies calmes. La forêt s'autorégule naturellement (absence totale d'incendies naturels ou de sécheresses).
- **Capitale :** [[Géographie/Sylve d'Aerwyn/Mirenfeld/Mirenfeld]], la cité née du [[Serment des Racines]].

## 📜 Histoire & Lore
*(Le passé de ce lieu, les événements marquants ou les secrets géographiques)*

-  La forêt fut le théâtre de la violente [[Guerre des Racines]] qui opposa ses peuples à l'[[Empire Vhalarionnien]]. Ce conflit prit fin grâce au sacré [[Serment des Racines]], un traité magique scellé par les druides de [[Khor'Vélyss]].
>[!notice] Lois de la Nature
>- **Le Tabou du Feu :** On ne brûle jamais le bois vivant sous peine d'un flétrissement spirituel immédiat.
>- **L'Écho du Souffle :** La magie [[Druide|druidique]] et bardique y est grandement amplifiée, à l'inverse de la *nécromancie* et de la magie du *feu* qui y s'avèrent bien plus instables.

## 🏠 Points d'intérêt (Sous-lieux)
*(Si c'est une ville : les tavernes, temples, boutiques. Si c'est une région : les villages, ruines, etc.)*

* **Les [[Frondains]] :** Une forêt mixte, lumineuse et fertile. C'est la région la plus accessible et habitée de la Sylve, traversée par d'anciennes routes de pierre.
	- *Points d'intérêt :* [[Géographie/Sylve d'Aerwyn/Mirenfeld/Mirenfeld]] ; [[Nourchêne]] ; [[Aey'Luin]]
- **Les [[Hauts-Feuillus]] :** Zone de relief élevé (falaises, collines et cascades) dominée par des arbres géants aux feuilles dorées.
	- *Points d'intérêt :* [[Cîmes-Hautes]] ; [[Anelthir]]
- **Le [[Cœur Voilé]] :** Une forêt ultra-dense, noyée sous des brumes épaisses où la magie ancienne est omniprésente, semblable à une jungle mystique.
	- *Points d'intérêt :* [[Khor'Vélyss]] ; [[Arbre de la Première Parole]]
- **La [[Lisière Morte]] :** Forêt grise et silencieuse, composée d'arbres morts, d'où toute vie semble s'être retirée.
	- *Points d'intérêt :* [[Branègme]]

---

## 🛠️ Recensement local (Dataview)

### 👥 Habitants et PNJ présents
*Cette liste affiche automatiquement tous les PNJ qui ont ce lieu précis indiqué dans leurs propriétés Frontmatter.*

```dataview
TABLE groupe AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
WHERE contains(list(lieu), this.file.name) and (contains(type, "PNJ") or contains(type, "PJ"))
SORT file.name ASC
```
