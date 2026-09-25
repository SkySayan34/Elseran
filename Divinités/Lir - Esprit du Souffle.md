---
type: divinité
rang: Esprit mineur
domaine: Souffle
tradition: Esprit druidique
alignement: NB
symbole:
lieu_de_culte: Cercle de Lir
statut: Actif
tags: divinité
---

# ✨ Lir - Esprit du Souffle


> [!infobox]+ symbole
> ![[Lir.png|cover]]
> ###### Fiche divine
> | | |
> | --- | --- |
> | **Rang** | `$= dv.current().rang` |
> | **Domaine** | `$= dv.current().domaine` |
> | **Tradition** | `$= dv.current().tradition` |
> | **Alignement** | `$= dv.current().alignement` |
> | **Statut** | `$= dv.current().statut` |
> | **Lieu de culte** | `$= dv.fileLink(dv.current().lieu_de_culte)` |

## 🌬️ Présentation & Manifestations
* **Apparence(s) / Avatars :** Lir se manifeste généralement sous la forme d'un enfant humanoïde fantomatique verdâtre. Il guide les perdus, et rapportent les informations de la [[Sylve d'Aerwyn]] à qui l'écoute.
* **Symbole & signes :** Il est symbolisé par une spirale venteuse bleu/vert, un peu similaire au [[médaillon de l'Ordre du Souffle]].
* **Épithètes & autres noms :** 

## 🌀 Domaine & Pouvoirs
* **Sphère d'influence :**  Il guide les perdus, et rapportent les informations de la [[Sylve d'Aerwyn]] à qui l'écoute.
* **Ce qu'elle accorde :** Résistance à ce qui relève de l'Air.
* **Limites & interdits :** 

## 📜 Doctrine & Tabous

* **Ce qu'elle attend de ses fidèles :** Le respect de la nature et de la vie sous toutes ses formes.
* **Ce qui l'offense :** la violence envers des êtres vivants.

## 🕯️ Culte & Rites

* **Clergé / Serviteurs :** Druides du [[Cercle de Lir]]
* **Lieux de culte :** Dans tous les endroits où se trouve un Druide pouvant faire appel au [[Cercle de Lir]]
* **Rites & célébrations :** [[Les Soufflantes|Les Soufflantes]]

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

```dataview
LIST
FROM #société 
WHERE contains(file.outlinks, this.file.link)
SORT file.name ASC
```

### ⚔️ Quêtes liées

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM #quête
WHERE contains(file.outlinks, this.file.link)
```

### 📓 Apparitions dans les sessions

```dataview
TABLE campagne AS "Campagne"
FROM #session 
WHERE contains(file.outlinks, this.file.link)
SORT file.name DESC
```
