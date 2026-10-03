---
type: campagne
nom: Chant des Cendres
world: Elseran
description: "La campagne principale se déroulant dans l'univers d'Elseran."
date_debut: 2026-06-26
statut: En cours
---

# 🌍 Chant des Cendres

> [!infobox]
> ###### **Informations Générales**
> | | |
> | --- | --- |
> | **Monde** | Elseran |
> | **Statut** | En cours |
> | **Début** | 2026-06-26 |

---

## 📖 **Arcs Narratifs**

```dataview
TABLE description AS "Description", statut AS "Statut", date_debut AS "Début"
FROM "Chant des Cendres/Arcs"
WHERE type = "arc"
SORT date_debut ASC
```


## **Quêtes en cours**

```dataview
TABLE description AS "Description", arc AS "Arc", statut AS "Statut", priorité AS "Priorité"
FROM #quête
WHERE contains(campagne, this.file.name) and statut != "Terminé" 
```

## 📅 **Sessions Récentes**

```dataview
TABLE date AS "Date", location AS "Lieu"
FROM "Chant des Cendres/Sessions"
WHERE type = "session"
SORT date DESC
LIMIT 5
```

