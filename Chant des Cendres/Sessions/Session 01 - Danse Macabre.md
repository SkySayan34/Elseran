---
type: session
campagne: Chant des Cendres
arc: A Mirenfeld
chapitre: Danse Macabre
lieu: Géographie/Sylve d'Aerwyn/Mirenfeld/Mirenfeld
tags: session
date: Soryn, 37è Souffle de Thalven, cycle 403
---

# Session 01 - Danse Macabre



> [!infobox]
> | | |
> |---|---|
> | **Campagne** | `$= dv.fileLink(dv.current().campagne)` |
> | **Arc** | `$= dv.fileLink(dv.current().arc)` |
> | **Chapitre** |  `$= dv.fileLink(dv.current().chapitre)` |
> | **Lieu** |  `$= dv.fileLink(dv.current().lieu)` |


# Récapitulatif



---

# Préparation de la Session

## Actes ou Scènes

### Scène 1 :

- Rejoindre l'[[Société/Ordre du Souffle]] après avoir discuté avec [[Eredi Saerel]] et [[Sorenza]]. 
1000 PO de récompense et présentation des accès : Scribe [[Eredi Saerel]] et [[Azimuth Sarvolan]] le magicologue. ==> Groupe : Vox Cineris

- **Première Mission** : Enquêter sur des meurtres autour de la [[Taverne des Abysses]].

### Scène 2 : Le Grand Frisson Éphémère

- **Lieu :** _La [[Taverne des Abysses]]_ (Un ancien entrepôt relooké en cabaret macabre : fausses toiles d'araignées, serveurs grimés, fumée épaisse, nobles en costume qui boivent du vin rouge "sang de dryade").
    
- **PNJ impliqués :** [[Grognard]] (à l'entrée), [[Valérian]] (sur scène ou en coulisses).
    
- **Descriptif :** Les PJ doivent entrer (négociation avec Grognard ou paiement de l'entrée sélect). Ils assistent à un "faux sacrifice" théâtral sur scène. L'ambiance est festive mais provocatrice.
    
- **Objectif de la scène :** Interroger Valérian. Il clame son innocence et leur donne accès aux coulisses/sous-sols pour prouver que tous ses monstres sont des acteurs et ses pièges, de la machinerie en bois.

### Scène 3 : L'Horreur Réelle (Le Twist)

- **Lieu :** Les coulisses et les sous-sols de la Taverne des Abysses / Les ruelles adjacentes.
    
- **PNJ impliqués :** Aucun au départ, puis un garde de la ville paniqué.
    
- **Descriptif :** Pendant que les PJ inspectent les trucages en bois de Valérian, un cri retentit dehors. Une nouvelle victime vient d'être jetée dans la ruelle juste derrière le cabaret. Le corps est encore chaud.
    
- **Objectif de la scène :** Examiner le cadavre. Un jet de Religion ou de Médecine (DD 12) révèle que les mutilations ne sont pas des morsures de monstres, mais des incisions rituelles ultra-précises imitant l'ancien rite de "Purification par la Racine" de l'Ordre de Sœur Sophie. Les indices (boue spécifique, morceaux de robe de bure) pointent vers une chapelle abandonnée non loin.

### Scène 4 : La Purification par le Sang (Le Final)

- **Lieu :** Une chapelle désaffectée de l'Ancien Culte ou les sous-sols d'un bâtiment de l'Ordre Impérial.
    
- **PNJ impliqués :** [[Sœur Sophie]] et 4 à 5 fanatiques (statistiques de Bandits/Cultistes). Une victime ligotée (un elfe sylvestre ou un acteur du cabaret).
    
- **Descriptif :** Les PJ déboulent en plein rituel. Sœur Sophie s'apprête à mutiler sa prochaine victime devant un autel improvisé, entourée de braseros. Elle ne cherche pas à nier : pour elle, Mirenfeld doit être nettoyée par le sang pour redevenir "pure".
    
- **Objectif de la scène :** Combat tactique. Il faut neutraliser les fanatiques et Sœur Sophie avant qu'elle ne tue l'otage. La zone peut comporter des risques environnementaux (braseros renversables, paille inflammable).
---

# Résumé de la Session

[[Vox Cineris]] a été envoyé pour leur première mission par l'[[Société/Ordre du Souffle]]. Ils doivent enquêter sur des morts autour de la [[Taverne des Abysses]]. Ils ont pour mission de retrouver les coupables.

En enquêtant sur place, ils rencontrent [[Valérian]], le tenancier de la taverne. Ils décident de l'interroger par des manières douteuses. Ils croisent également le chemin de [[Grognard]] qui garde l'entrée de la taverne et participe au "spectacle".

Le groupe comprend rapidement que Valérian n'y est pour rien, et suivent la piste d'un meurtre frais. Cette piste les mène à une vieille chapelle dans laquelle se trouvent [[Sœur Sophie]] et ses acolytes en plein rituel de sacrifice.

Ils n'hésitent pas une seconde et tuent ces servants de l'[[Ordre Impérial de la Lumière]], stoppant ainsi le rituel de purification sur un demi elfe présent.

Ils ramènent ensuite le demi elfe dans un lieu d'accueil avant de rentrer à [[L'Auberge du Chêne Vert]]. 

^summary

---

# 📜 Journal de Session

```dataview
LIST
FROM #session 
WHERE contains(campagne, this.campagne)
SORT file.name DESC
```

