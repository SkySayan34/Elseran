---
type: faction
categorie: Guilde
quartier_general: Auberge du Chêne Doré
dirigeant: Zéphirae Anemoi
influence: Haute
tags: société
---

# 🛡️ Organisation : Ordre du Souffle
> [!infobox]+ blason
> ![[Ordre du Souffle.png|cover]]
> ###### Fiche d'identité
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **QG Principal** | `$= dv.fileLink(dv.current().quartier_general)` |
> | **Dirigeant** | `$= dv.fileLink(dv.current().dirigeant)` |
> | **Influence** | `$= dv.current().influence` |


## 👁️ Présentation & Philosophie

* **Devise / Dicton :** Le vent souffle dehors, et qu'il nous emporte tous
* **Doctrine / Objectif :** Conserver la paix et l'Harmonie en Elseran

L'**Ordre du Souffle** est une fraternité spirituelle, philosophique et humanitaire majeure d'[[Elseran]].

Aux yeux du peuple et des autorités profanes, ses membres ne sont que d'humbles voyageurs qui prêtent main forte aux démunis. Ils sont profondément aimés pour leur dévouement désintéressé et leur neutralité politique absolue.

### Les Trois Piliers du Souffle

L'action et la foi de l'Ordre reposent sur trois préceptes fondamentaux :
* **Réparer :** Guérir les corps meurtris, apaiser les esprits tourmentés et soigner la terre elle-même là où la magie ou la guerre l'ont déchirée.
* **Préserver :** Sauver de l'oubli la mémoire du monde, ses ruines anciennes, ses langues disparues (comme le *Vharun*) et les souvenirs des mourants.
* **Relier :** Tisser des liens d'empathie et de compréhension mutuelle entre les peuples d'Elseran pour étouffer les germes de la discorde.

## Différents grades :


- **Les Cinq :** L'autorité de l'Ordre. Cinq figure anonymes qui détiennent la doctrine et guident la fraternité. Chacun porte un masque représentant la région qu'il gère.
- **Voiles :** Les voiles sont les aventuriers de l'Ordre. Ce sont ceux qui sont envoyés sur le terrain pour les missions basiques.
- **Voiles de l'Ombre :** Ceux-ci sont la partie immergée de l'Ordre. Leur identité reste secrète, ils participent aux missions top secrètes, diplomatie, manipulation, tout ce que l'Ordre ne peut pas se permettre de révéler, ce sont eux les instigateurs de ce genre de missions.
- **Scribes :** Les gardiens du savoir, ils collectent, transcrivent et étudient l'Histoire d'Elseran. Tout se savoir est contenu dans le [[Codex du Souffle]].
- **Magicologues :** Ce sont les scientifiques magiques. Ils se chargent d'étudier et d'assister les voiles dans leur équipement.

## 📜 Histoire & Secrets
*(Les origines de la faction, ses anciens dirigeants, ses rivalités historiques et ce qu'elle cache au grand public)*

- Grande Guilde créée par un groupe d'aventurier il y a longtemps. L'un des aventuriers était le dirigeant actuel : [[Zéphirae Anemoi]].
- Le chef est au courant de l'existence de fragments du Chant, mais n'en comprend pas le sens
- Guilde répartie dans Elseran sous la forme d'Auberge du Chêne "".

Sous cette façade de charité publique se cache une organisation mystique d'une envergure colossale. Les haut-gradés de l'Ordre se consacrent en secret à une tâche titanesque : **retrouver, préserver et harmoniser les Fragments du Chant des Cendres** — les vestiges d'un pouvoir divin originel dont la résonance sacrée est indispensable pour maintenir la cohésion d'un monde qu'ils sentent vaciller.

## 🧭 Relations Extérieures

* **Alliés :** 
* **Rivalités / Ennemis :** 

---

## Registre des Membres

### 👥 Membres et Affiliés (PJ & PNJ)
*Cette liste est automatique. Elle utilise la méthode textuelle "blindée" pour trouver tous les PNJ et PJ dont la propriété `faction` contient le nom de cette note.*

```dataview
TABLE fonction AS "Groupe / Rôle", faction AS "Faction", statut AS "Statut"
FROM #PNJ OR #PJ
WHERE contains(faction, this.file.name)
SORT file.name ASC
```

