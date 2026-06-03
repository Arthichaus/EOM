# GDD — Référentiel Buffs, Malus et États

Auteur: ArthMil

## Page de référence

Cette page centralise les buffs, malus et états utilisés par le système de combat. Elle sert de source de référence pour l'équilibrage, les fiches personnages et les futurs modules d'effets.

---

## Regles de lecture

- Chaque effet doit avoir un nom unique.
- Chaque effet doit preciser s'il est un buff, un malus ou un etat neutre.
- Chaque effet doit indiquer sa duree, sa portee et sa source principale.
- Les effets de vitesse modifient la VIT et donc l'ordre d'action.
- Toute attaque qui inflige des degats peut etre un coup critique. La chance est egale au TC (%).
- En critique, les degats sont multiplies par (1 + DC%). Exemple: DC 100% -> degats doubles.
- Les buffs qui augmentent les degats s'appliquent apres le calcul du critique.
- La Precision est la chance (%) d'appliquer un malus a la cible.
- Valeurs globales par defaut ci-dessous (les fiches perso peuvent remplacer ces valeurs).

---

Régle : les tour des effets/malus/buff son noter sur les personnage/ennemis

## Buffs

| Nom | Effet | Sources | Notes |
|---|---|---|---|
| Buff offensif | Augmente l'atk de la personne possèdant le buff. (La valeur du buff est définie sur le perso) | Angel, Anya, les jumeaux | Augmente le Dps |
| Buff defensif | Augmente la defense sur une valeur de défense fixe.(La valeur du buff est définie sur le perso) | Angel, Grant, Anya, les jumeaux | ! la défense fixe et une valeur fixe, elle fonctionne en méthode de soustraction aux dégats reçus (ex : deff fixe - attaque ennemis) |
| Recuperation | Rend des PV sur une durée de tout définie par le personnage. (La valeur du buff est définie sur le perso) | Freya | Peut se cumuler avec soins directs. Soigne aux début du tour du personnage qui a ce buff |
| Touchez garentie | le personnage est garentie de toucher sa cible lorsqu'il attaque à coup sûr. | Jackson | Contre un certains type d'ennemies |
| Buff TC | Augmente le taux critique du personnage. (La valeur du buff est définie sur le perso) | Jackson, les jumeaux | Augmente le DPS, chaque attaque à une chance de crit |
| Buff DC | Augmente les dégâts critique du personnage. (La valeur du buff est définie sur le perso) | Jackson | Augmente le DPS, elle augmente les dégats si le coup est un critique en fonction du pourcentage de DC ( ex : s'il y a 100% de DC les dégâts son doubler) |
| Ignore Def | Ignore un partie de la def en % de la cible. (La valeur du buff est définie sur le perso) | Jackson | Augmente le DPS, ! la def fixe n'est pas non plus compatibiliser |
| Augmentation de dégâts | Augmente les dégats que va infliger le personnage en %. (La valeur du buff est définie sur le perso) | Ulysse | Augmente le DPS, augmente la valeur finale des dégats infligées de n%, n'agis quand dernier soit après le TC DC |
| Buff de vitesse | Augmente la vitesse du personnage. (La valeur du buff est définie sur le perso) | les jumeaux | Augmente le vitesse, agis immédiatement |
| Immunité | Ne peux plus subir de malus durant n tour ( n definie sur personnage). | Jade | N'agis pas comme un clease, évite juste de recevoire des malus. |

---

## Malus

| Nom | Effet | Sources | Notes |
|---|---|---|---|
| Enflamme | Inflige des degats sur la duree en fonction des PV max.(La valeur du malus est définie sur le perso) | Léora, Freya , Jade | DoT, les dégâts s'inflige lors du tour de personnage qui a ses malus, limite à 5 malus enflammé par cible |
| Empoisonnement | Inflige des degats sur la duree en fonction de l'atk.(La valeur du malus est définie sur le perso) | Jade | DoT, cumulable jusqu'à 10. |
| Fragilisation | Augmente les degats subis de la cible.(La valeur du malus est définie sur le perso) | Léora, Jade | exemple la cible prends 20% de damage suplémentaire. |
| Ralentissement | Reduit la VIT de la cible pour n tour. (La valeur du malus est définie sur le perso) | Léora, Sam, Jade | peut être mis une seule fois sur un ennemie, prends le taux le plus élevé selon le debuff |
| Provocation | Force la cible a viser une cible en priorite. | Grant, Ulysse, Jade | permet aux tank d'agir comme un tank, ne peut que être mis une fois et ne peut pas se cumuler |
| Saignement | Inflige des degats sur la duree 10% de l'attaque. | Mara | peut être cumuler sur 10 stacks |
| Affaiblissement | Reduit l'atk de la cible pour n tour. (La valeur du malus est définie sur le perso) | Léora, Grant, les jumeaux | peut être mis une seule fois sur un ennemie, prends le taux le plus élevé selon le debuff |
| Brisure | Reduit la def % de la cible pour n tour. (La valeur du malus est définie sur le perso) | Léora, les jumeaux, Sam | peut être mis une seule fois sur un ennemie, prends le taux le plus élevé selon le debuff, ne réduit pas la def fixe ! |
| Etourdissement | empêche la cible de jouer pendant n tour(n défini sur le perso) | Grant, Ethan | peut être mis une seule fois sur un ennemie, ne se cumule pas|
| Réduction de dégâts | Reduit les dégâts que va infligé la cible pour n tour. (La valeur du malus est définie sur le perso) | Ulysse | peut être mis une seule fois sur un ennemie, prends le taux le plus élevé selon le debuff |
| Silence | La cible ne peut plus utiliser de compétence ni d'utilme tant que se malus est présent sur elle | Léora, Sam | peut être mis une seule fois sur un ennemie |
| Anti-soin | Empêche la cible de recevoir du soin peut importe la manière | Léora | peut être mis une seule fois sur un ennemie |
---

## Effets de terrain

| Nom | Type | Effets | Source | Note |
|---|---|---|---|---|
| Terrain de flamme infernale | DoT | applique Enflamme à chaque action ennemie pendant 3 tout. | Freya | DoT |
| Terrain de flamme angélique | Soin | soigne les allies de 60% de l'attaque a chaque action pendant 3 tour. | Freya | soigne aux début du tour alliées |
---

## Etats speciaux

| Nom | Type | Effet | Sources | Notes |
|---|---|---|---|---|
| Etat gemme | Etat | Active un effet de gemme sur le personnage, selon la voie choisie l'effets est soit sur l'ennemies soit sur Jade. | Jade | Il peut y avoir plusieurs état de gemme mais seulement d'une seule catégorie, chaque état de gemme à 3 stade soit l'effets sera visible de cet manière "Etat "Ruby" nv1" par exemple et ainsi gâce à cet état le personnage pourra utiliser cet état pour avoir des effets différents : Ruby - Saphir - Amethyste - Onyx - Opale| 
| Contre Ruby | Contre | Posséde 3 stade(../../..), contre-attaque une attaque ennemies avec 25%/50%/75% de chance de contré et applique Enflammé 3 tours(5% PV max)| Jade | s'applique après chaque attaque ennemies|
| Esquive Saphir | Etat | Posséde 3 stade(../../..), esquive l'attaque ennemies 15%/25%/50% de chance de réussite pour chaque attaque | Jade | s'applique après chaque attaque ennemies |
| Contre Amethyste | Contre | Posséde 3 stade(../../..), Contre attaque un attaque ennemies avec 25%/50%/75% de chance de contré et lui applique empoisonnement 3 tours (20% ATK) | Jade | s'applique après chaque attaque ennemies |
| Contre Onyx | Contre | Posséde 3 stade(../../..), contre-attaque avec 25%/50%/75% de chance de contré et inflige 80% ATK + Fragilisation 20% | Jade | s'applique après chaque attaque ennemies |
| Bulles | Etat | Posséde 80% des pv de Sam, elle protége des dégats subit, non cumulable | Sam | réagis comme une protection des dégats subits, une couche de pv supplémentaire |
| Etat repos | Etat | Fait diminuer la jauge de surchauffe de 10% en plus après chaque action | Ulysse | permet de réduire la surchauffe |
| Etat contre | contre | 75% de contrer un attaque ennemies de 25% d'atk et 25% de def(ratio 10% -> 100 degats + valeur fixe), il subit l'attaque mais la réduit en plus de la def (%) de 20%( attque -> def (%) -> reduc 20% -> subit -> contre) | Ulysse | à chaque attaque ennemies |
| Réservoir | Jauge |  il accumule les dégats qu'il subit jusqu'à un max de 10 000(s'il plus sont stocker, tombe KO)(les dégats stocké correspond aux dégats subit après réduction via def) | Ethan | jauge |
| Sacrifice | Etat |  permet de prendre 20% des dégats que subit un alliée et de le prendre à sa place | Ethan | pour stacker la jauge |
| Enchainer | Etat |  l'ennemis ne pour plus qu'attaquée Grant tant qu'il a cet effet sur lui | Grant | une sorte de provoc spéciale |
| Rejoue | Etat |  la cible rejoue un tour après une action | Anya |  |
| Lien | Etat |  n'a pas d'effets particulier mais via une compétence donne des buff, cumulable jusqu'à 10 fois | Anya | 10 -> lien intemporel |
| Lien intemporel | Etat | n'a pas d'effets particulier mais via une compétence donne des buff, etat finale de lien ne peut pas être cumuler, et la cible qui a cet effets ne peut plus recevoir d'effet lien ! | Anya |  |
| Couleur | Etat | Tous ses effets son définie sur le personnage de Léora les différents etat son : Rouge, Bleu, Vert, Violet, Jaune, Cyan, Rouge foncé, Vert foncé, Bleu foncé dure tant qu'il ne sont pas fusionné | Léora | chauqe couleur à un effets |
| Fragmenté | Etat | n'a pas d'effets particulier mais via un ultime peuvent être consomé pour infligé des dégâts, cumule max 20  | Néo |  |
| Stockage d'energie | Jauge |  Jauge d'énergie qui augmente les dégats des tires - Commence avec 50% de sa jauge - Augmente de 20% après chaque actions. | Jackson | degats |
---

## A completer

- Ajouter les valeurs numeriques exactes de chaque effet.
- Ajouter les conversions si tu veux des versions faible / moyenne / forte.
- Ajouter les effets specifiques aux armes et aux gemmes.
- Ajouter les interactions exactes entre buff, malus, cleanse et immunite.