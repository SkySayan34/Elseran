---
type: quête
nom: Retrouver Naelwyn
campagne: Chant des Cendres
arc: A Mirenfeld
chapitre: Plaider Coupable
description: Naelwyn a été capturée par une guilde pour faire chanter Vox Ceneris. Arriveront-ils à la sauver avant leur procès?
statut: à venir
priorité: Secondaire
tags: quête
---

# Retrouver Naelwyn



> [!infobox]
> | | |
> |---|---|
> | **Campagne** |`$= dv.fileLink(dv.current().campagne)` |
> | **Arc** | `$= dv.fileLink(dv.current().arc)` |
> | **Chapitre** | `$= dv.fileLink(dv.current().chapitre)` |
> | **Statut** | `$= dv.current().statut` |
> | **Priorité** | `$= dv.current().priorité` |

## 📜 **Description**

`$= dv.current().description`

##  **Objectifs**

- [ ]  Interroger l'enfant qui leur donne la lettre
- [ ]  Suivre le moineau de Naelwyn
- [ ]  Interroger les témoins (bateliers)
- [ ]  Se renseigner auprès du Nid du Corbeau.
- [ ]  Retrouver la guilde Voragine
- [ ]  Battre Morgath et récupérer Naelwyn
- [ ]  Bonus : Convaincre Morgath de plaider en leur faveur pour le procès.

---

## 👥 **PNJ Impliqués**


- [[Naelwyn]]
- [[Morgath]]

---

## 🗺️ **Lieux Associés**

- [[QG des Voragine]]
- [[Auberge du Chêne Vert]]

## **Sessions**

```dataview
LIST
FROM #session
WHERE contains(file.outlinks, this.file.link)
SORT date ASC
```

## 📌 **Récompenses**

- **Expérience** : 
- **Butin** :
- **Autres** :