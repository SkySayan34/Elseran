---
type: quête
nom: Meurtres de la Taverne des Abysses
campagne: Chant des Cendres
arc: A Mirenfeld
chapitre: Danse Macabre
description: Des meurtres ont lieu proche de la [[Taverne des Abysses]]. Vox Ceneris doit trouver les coupables.
statut: Terminé
priorité: Secondaire
tags: quête
---

# Meurtres de la Taverne des Abysses



> [!infobox]
> | | |
> |---|---|
> | **Campagne** |`$= dv.fileLink(dv.current().campagne)` |
> | **Arc** | `$= dv.fileLink(dv.current().arc)` |
> | **Chapitre** | `$= dv.fileLink(dv.current().chapitre)` |
> | **Statut** | `$= dv.current().statut` |
> | **Priorité** | `$= dv.current().priorité` |

## 📜 **Description**

[[Vox Cineris]] a été envoyé pour leur première mission par l'[[Ordre du Souffle]]. Ils doivent enquêter sur des morts autour de la [[Taverne des Abysses]]. Ils ont pour mission de retrouver les coupables.

##  **Objectifs**

- [x]  Parler à [[Valérian]] pour comprendre qu'il est innocent
- [x]  Etudier les cadavres
- [x]  Suivre la piste remontant jusqu'à [[Sœur Sophie]]
- [x]  Neutraliser [[Sœur Sophie]] et ses acolytes

---

## 👥 **PNJ Impliqués**


- [[Grognard]]
- [[Sœur Sophie]]
- [[Valérian]]

---

## 🗺️ **Lieux Associés**

- [[Taverne des Abysses]]

## **Sessions**

```dataview
LIST
FROM #session
WHERE contains(file.outlinks, this.file.link)
SORT date ASC
```

## 📌 **Récompenses**

- **Expérience** : 250 XP
- **Butin** :
- **Autres** :