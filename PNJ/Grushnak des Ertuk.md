---
type: PNJ
statut: Vivant
faction: Ertuk
fonction: Chef de Clan
lieu: Géographie/Dhar'Zulun/Dhar'Zulun
alignement: LM
race: Orc
classe:
genre: Homme
description: Le Chef du clan des Ertuk, porteur du prix du sang des Zarka.
tags: PNJ
---

# Grushnak des Ertuk



> [!infobox]+ portrait
> ![[Grushnak des Ertuk.jpg|cover]]
> ###### Infos Rapides
> | | |
> | --- | --- |
> | **Faction** | `$= dv.fileLink(dv.current().faction)` |
> | **Fonction** | `$= dv.current().fonction` |
> | **Lieu** | `$= dv.fileLink(dv.current().lieu)` |
> | **Statut** | `$= dv.current().statut` |


##  Description & Psychologie

* **Apparence :** Orc de deux mètres, muscles longs et secs, taillé par des décennies de marches. Peau gris-bronze brûlée par le soleil, mâchoire massive, un croc supérieur ébréché. Œil gauche voilé, laiteux, perdu pendant la guerre fratricide. Bras gauche entièrement couvert de brands rituels — les marques à vif du Prix du Sang. Cheveux noirs tressés de perles d'os et d'un éclat de roche ocre rouge. Longue cape de lin grossier teinte ocre sur une armure de cuir renforcée d'écailles de wyrm du désert à l'épaule droite. Manie « [[Griffe-du-Serment]] », un grand glaive recourbé portant une encoche par membre du clan tombé à la guerre.

* **Personnalité :** Grave, cérémonieux, implacable. Ne crie jamais, pèse chaque parole comme si elle engageait le clan entier. Intègre jusqu'à l'os : le Prix du Sang est une comptabilité sacrée, pas une métaphore. Fait tourner une perle d'os de sa tresse entre ses doigts quand il évalue quelqu'un ; répond souvent par une question. Méprise le mensonge par-dessus tout : un orc qui ment sur son nom est pire qu'un ennemi.

* **Motivation principale :** Acquitter le Prix du Sang et sauver le clan de l'extinction. La guerre fratricide a coûté aux Ertuk les deux tiers de leurs guerriers : Grushnak doit trancher entre vengeance contre les Zarka et survie du clan.

* **Secrets / Ce qu'il cache :**
	- Il a lui-même tué le mentor du PJ déserteur pendant la guerre fratricide, pour empêcher l'anéantissement total du clan — une dette qu'aucun rite ne peut effacer ; si le clan l'apprenait, son autorité s'effondrerait.
	
	- Il cherche le PJ déserteur non pour le tuer mais pour lui demander de revenir — le serment exige qu'un Ertuk vivant paye la dette ; il laissera toujours croire qu'une exécution l'attend tant que la loyauté des PJ n'est pas prouvée.

##  Notes & Lore
*(Raconte ici son histoire, son passif avec les PJ ou son rôle actuel dans l'intrigue)*

Les orcs portent leur nom suivi du nom de clan : un orc sans nom de clan est un déserteur ou un menteur. Le clan des Ertuk vit sous le Prix du Sang — une dette de sang née de la guerre fratricide contre le clan des [[Zarka]], non honorée à ce jour.

Force politique neutre à convaincre. Les PJ doivent l'allier le clan ; le PJ déserteur des Ertuk est considéré comme traître par les siens, ce qui crée une tension immédiate à la première rencontre.

##  Relations & Connexions

* **Alliés :** [[Vashk l'Ombre-de-Sel]], chaman du clan et plus vieil ami de Grushnak (seule voix qui ose le contredire) ; liens de pâture avec les [[caravaniers du Bazzaar-de-la-Poussière]]
* **Ennemis :** Le clan des [[Zarka]] (lignée rivale de la guerre fratricide) ; rancune froide contre les [[Empire Vhalarionnien|pillards impériaux de Vhalarion]]
* **Réseau :** 

##  Coulisses du MJ
*Cette section se remplit automatiquement si d'autres notes (quêtes, sessions, rumeurs) mentionnent ce PNJ.*

### Quêtes liées

```dataview
TABLE description AS "Objectif", statut AS "Statut"
FROM ""
WHERE type = "quête" AND contains(file.outlinks, this.file.link)
```


### Journal des rencontres

```dataview
LIST
FROM "" 
WHERE type = "session" AND contains(file.outlinks, this.file.link)
SORT file.name DESC
```
## Conseils d'interprétation :

**Voix et diction**

- Voix **grave et lente**, très peu de mots. Des pauses longues, comme si chaque phrase était gravée dans la pierre. Ne monte _jamais_ le ton : quand il baisse la voix encore davantage, c'est qu'il est au bord de la violence.
- Vocabulaire simple mais solennel : « Le sable garde ce que le sang verse. » « Tu portes un nom ? Alors tu portes une dette. »
- Accent : appuyé sur les syllabes dures, roulées — comme si l'orc pensait encore en langue des dunes.

**Tics réutilisables**

- La perle d'os qui tourne entre ses doigts quand il évalue quelqu'un (arrête de la faire tourner = décision prise).
- Il répond par une question : « Que vaut ta parole quand ton nom est un mensonge ? »
- Il ne regarde jamais avec son œil valide : il _fixe de l'œil mort_, ce qui met les joueurs mal à l'aise — c'est voulu.
- Il nomme toujours les PJ par leur nom complet, s'ils l'ont donné. Un mensonge sur le nom = rupture immédiate.

**Réactions types**

- **Violence** : il ne dégaine pas en premier — il annonce calmement les conséquences, une fois. « Griffe-du-Serment a encore de la place pour des encoches. »
- **Négociation** : il marchande comme on pèse de l'or — lentement, exigeant une contrepartie qui _coûte_ à l'autre. Jamais de don gratuit : c'est une insulte au Prix du Sang.
- **Flatterie** : inutile, voire irritante. Le seul hommage qu'il respecte est un fait d'armes ou une vérité coûteuse.
- **Mensonge (perçu)** : froideur totale. Le clan a une maxime — « un orc sans nom est un déserteur ou un menteur » — et il la cite en fixant l'oreille du PJ.

**Conseils de RP**

- **Le levier émotionnel clé** : la scène où le PJ déserteur est reconnu. Grushnak ne le traite pas comme un traître à abattre — il le traite comme une **dette non honorée**, avec une lourdeur presque paternelle. Joue la tension : le PJ (et les joueurs) doivent croire à l'exécution jusqu'au dernier moment.
- **Doser les secrets** : ne révèle le meurtre du mentor _jamais_ par Grushnak lui-même en public. Idéal : c'est Vashk le chaman qui le confie en aparté, ou une marque de plus sur son bras que le PJ remarque. Le secret 2 (le retour du déserteur) peut se révéler par un détail : Grushnak fait préparer une tente pour le PJ, pas une fosse.
- **Le rendre mémorable** : ses encoches sur la lame. Encourage les PJ à demander l'histoire d'une encoche — chaque réponse est un fragment de lore des Ertuk, et un excellent outil de exposition.
- **Alliance** : les PJ ne gagnent pas sa confiance par un discours, mais par un **acte qui coûte** — payer une dette à sa place, sauver un Ertuk, ou livrer un Zarka. Il faut que le Prix du Sang bouge.

### Liens out:
`$= dv.fileLink(dv.current().faction)`
`$= dv.fileLink(dv.current().lieu)`
