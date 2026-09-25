---
type: chapitre
nom: Danse Macabre
arc: A Mirenfeld
campagne: Chant des Cendres
description: Des meurtres ont lieu proche de la [[Taverne des Abysses]]. Vox Ceneris doit trouver les coupables.
statut: Terminé
tags: chapitre
---

# 📖 Danse Macabre


> [!infobox]
> | | |
> |---|---|
> | **Arc** | `$= dv.fileLink(dv.current().arc)` |
> | **Campagne** | `$= dv.fileLink(dv.current().campagne)` |
> | **Statut** | `$= dv.current().arc` |


## 📜 **Résumé**

[[Vox Cineris]] a été envoyé pour leur première mission par l'[[Société/Ordre du Souffle]]. Ils doivent enquêter sur des morts autour de la [[Taverne des Abysses]]. Ils ont pour mission de retrouver les coupables.

En enquêtant sur place, ils rencontrent [[Valérian]], le tenancier de la taverne. Ils décident de l'interroger par des manières douteuses. Ils croisent également le chemin de [[Grognard]] qui garde l'entrée de la taverne et participe au "spectacle".

Le groupe comprend rapidement que Valérian n'y est pour rien, et suivent la piste d'un meurtre frais. Cette piste les mène à une vieille chapelle dans laquelle se trouvent [[Sœur Sophie]] et ses acolytes en plein rituel de sacrifice.

Ils n'hésitent pas une seconde et tuent ces servants de l'[[Ordre Impérial de la Lumière]], stoppant ainsi le rituel de purification sur un demi elfe présent.

Ils ramènent ensuite le demi elfe dans un lieu d'accueil avant de rentrer à [[L'Auberge du Chêne Vert]]. 


## Sessions

```dataview
LIST
FROM #session 
WHERE contains(campagne, this.file.name)
SORT file.name DESC
```

## Quêtes

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM #quête
WHERE contains(chapitre, this.file.name)
SORT priorité DESC, date_debut ASC
```

