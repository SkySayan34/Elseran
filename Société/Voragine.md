---
type: faction
nom: La Voragine
categorie: Guilde
quartier_general: Géographie/Sylve d'Aerwyn/Frondains/Mirenfeld/Subracine/QG des Voragine
dirigeant: Morgath
alignement: NM
influence: Faible
tags: société
---

# 🛡️ Organisation : La Voragine

> [!infobox]+ blason
> ![[Voragine.jpg]]
> ###### Fiche d'identité
> | | |
> | --- | --- |
> | **Catégorie** | `$= dv.current().categorie` |
> | **QG Principal** | `$= dv.fileLink(dv.current().quartier_general)` |
> | **Dirigeant** | `$= dv.fileLink(dv.current().dirigeant)` |
> | **Influence** | `$= dv.current().influence` |

## 👁️ Présentation & Philosophie

* **Devise / Dicton :** *« Ce que le fleuve avale nous revient. »*
* **Doctrine / Objectif :** Une guilde de voleurs professionnels du [[Creux de l'Anserah]] — cambriolages, enlèvements sur contrat, tractations et livraisons discrètes. Sa règle de fer n'est ni l'or ni le sang : c'est la **neutralité commerciale absolue** envers toutes les familles de la pègre. La Voragine ne prend jamais parti, ne noie jamais personne (« le fleuve décide, pas nous »), et **tient parole à la lettre** — ce qu'elle promet, elle l'exécute, et elle exige la même précision de ses clients.
* **Ressources & Moyens :**
	- **La Serre** : le QG vitré de [[Subracine]], ancienne serre-bassin impériale engloutie lors de la construction des quais, suspendue au-dessus des profondeurs de l'[[Anserah]] et des racines du [[Mir'Sylva]] ;
	- Une flotte de **barques sans lanterne** et des relais chez les bateliers des quais ;
	- L'accord de longue date avec **l'[[Éclat de Verre]]** : tout le verre de la Serre est soufflé là-bas, en sous-main ;
	- Son vrai trésor : **une archive de contrats et de dettes** — chaque client, chaque faveur, chaque secret y est consigné.

## 📜 Histoire & Secrets
*(Les origines de la faction, ses anciens dirigeants, ses rivalités historiques et ce qu'elle cache au grand public)*

- **Le noyé fondateur** : [[Morgath]], halfelin des rives laissé pour mort par son équipage dans l'Anserah, en est remonté. Il a revendiqué l'ancienne serre engloutie et fait vitrer la Serre de neuf. La Voragine est née de ce qu'il croit être une dette : le fleuve l'a rendu, il lui doit tout.
- **Les Fonds** : ainsi nomme-t-on ses membres — *ceux du fond*, et l'argent qu'on y coule. On y entre par le « retour du fleuve », une épreuve d'initiation que Morgath ne commente jamais.
- **Secrets :**
	- *Le contrat* : la guilde détient le **contrat signé d'[[Ambroise de Valcourt]]** pour l'enlèvement de [[Naelwyn]] — la preuve qui peut briser un membre de la [[Cour des Échos]] ;
	- *La rive les a tous rendus* : l'équipage qui a abandonné Morgath enfant a disparu un à un. La Voragine ne le sait pas. Personne ne le sait ;
	- *L'archive* : l'étendue des dettes consignées dépasse ce que quiconque imagine — un levier dormante sur la moitié du Creux.

## 🧭 Relations Extérieures

* **Alliés :** Aucun — des partenaires et des clients, jamais d'alliés. La neutralité est le produit qu'elle vend.
* **Rivalités / Ennemis :** Les familles de la pègre qui voudraient l'absorber (tensions larvées à préciser une fois le filler « Fantômes de Mirenfeld » intégré) ; méfiance réciproque avec le Cartel des Bateliers de l'Anserah, dont la Voragine contourne les écluses.

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