---
type: quête
nom: Meurtres de la Taverne des Abysses
campagne: Chant des Cendres
arc: A Mirenfeld
chapitre: Danse Macabre
world: Elseran
description: Des meurtres ont lieu proche de la [[Taverne des Abysses]]. Vox Ceneris doit trouver les coupables.
statut: En cours
priorité: Basse
date_debut: 2026-06-26
tags:
  - quête
---

# 🎯 Meurtres de la Taverne des Abysses

> [!infobox]
> | | |
> |---|---|
> | **Campagne** | `= this.campagne ` |
> | **Arc** | `= this.arc ` |
> | **Chapitre** | `= this.chapitre ` |
> | **Statut** | `= this.statut ` |
> | **Priorité** | `= this.priorité ` |
> | **Début** | `= this.date_debut ` |

## 📜 **Description**

`= this.description `


## 🎯 **Objectifs**

- [ ]  Parler à [[Valérian]] pour comprendre qu'il est innocent
- [ ]  Etudier les cadavres
- [ ]  Suivre la piste remontant jusqu'à [[Sœur Sophie]]
- [ ]  Neutraliser [[Sœur Sophie]] et ses acolytes

---

## 👥 **PNJ Impliqués**

_(Ce champ est utilisé par la requête dans ton template PNJ existant)_

- [[Grognard]]
- [[Sœur Sophie]]
- [[Valérian]]

---

## 🗺️ **Lieux Associés**

- [[Taverne des Abysses]]

## **Sessions**

```dataview
LIST
FROM "${campagne}/Sessions"
WHERE contains(file.outlinks, this.file.link)
SORT date ASC
```
## 📌 **Récompenses**

- **Expérience** : 250 XP
- **Butin** :
- **Autres** :

