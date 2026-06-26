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

## 👥 **Personnages Principaux**

```dataview
TABLE nom AS "Nom", faction AS "Faction", lieu AS "Localisation"
FROM #PNJ OR "PNJ"
WHERE contains(campaign, "Chant des Cendres")
SORT file.name ASC
LIMIT 10
```

## 🗺️ **Lieux Clés**

```dataview
TABLE nom AS "Nom", categorie AS "Type", parent AS "Région"
FROM #lieu OR "Géographie"
WHERE contains(campaign, "Chant des Cendres")
SORT file.name ASC
LIMIT 10
```

## 🏛️ **Factions en Jeu**

```dataview
TABLE nom AS "Nom", type_société AS "Type", dirigeant AS "Dirigeant"
FROM #société OR "Société"
WHERE contains(campaign, "Chant des Cendres")
SORT file.name ASC
```

## 📅 **Sessions Récentes**

```dataview
TABLE date AS "Date", game_date AS "Date In-Game", location AS "Lieu"
FROM "Chant des Cendres/Sessions"
WHERE type = "session"
SORT date DESC
LIMIT 5
```

