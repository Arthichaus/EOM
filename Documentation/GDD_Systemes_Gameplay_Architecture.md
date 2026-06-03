# GDD - Systemes Gameplay et Architecture

Auteur: ArthMil

Document detaille qui preserve les informations systemes initialement presentes dans le master et les organise par domaines techniques et gameplay.

## 1. Boucle de Gameplay Detaillee

Le joueur alterne entre:

1. Exploration libre
2. Quetes secondaires
3. Quete principale

Structure typique d'une quete principale:
1. Dialogue
2. Exploration
3. Enigmes
4. Combats
5. Revelation
6. Retour QG
7. Deblocage de nouvelles zones

## 2. Enquete et Journal

### 2.1 Types d'indices

- Donnees numeriques
- Temoignages
- Objets physiques
- Traces d'energie

### 2.2 Fonctionnement

- Les enquetes servent aux quetes principales et secondaires.
- Les informations recoltees alimentent le journal.
- Le journal centralise fils narratifs, hypotheses, zones debloquees et personnages.

## 3. Structure du Monde Detaillee

### 3.1 Carte et zones

Carte fixe en zones modulaires connectees, style Pokemon.

Structure des zones:

- Mix ouvert / couloir selon les besoins de pacing.
- Presence de sous-maps et maps internes (batiments).

Types de sous-maps:

- Batiments civils (appartements, commerces, cave)
- Batiments de faction
- Entrepots / hangars
- Egouts / tunnels techniques
- Zones de culte, église improvisé du culte (interieurs)
- Lieux scenario (QG, caches, laboratoires)

- Districts de ChatarraCity
- District central de ChatarraCity
- Quartier industriel
- Bidonvilles
- Zone du culte
- Zones corrompues
- DivusPolice
- Noyau d'energie

### 3.2 Types de corruption de zone

1. Corruption permanente: zones fixes tres dangereuses
2. Corruption temporaire: zones decorrompables

### 3.3 Decorromption

- Debloquee via quete principale
- Activite secondaire majeure
- Necessite un dispositif special
- Structure type: petits combats, mini-boss ou boss, activation du dispositif
- Certaines zones decorrompues ne font plus reapparaitre les monstres

### 3.4 acces aux zones

- Deblocage par quetes principales ou secondaires.
- Deblocage via objets (cles, acces de batiments, sous-maps).
- Deblocage par purification de la corruption.
- Deblocage par reputation de faction (acces a zones de faction).

### 3.5 Points d'interet (minimum)

- Au moins 1 atelier de modules par zone.

### 3.6 Deplacement rapide

- Un seul point de TP par zone.
- Il faut se rendre au point pour se teleporter.

### 3.7 Events de zone pas sur

- Events dynamiques rares (embuscades/encounters).

## 4. Anges, Compatibilite et Stabilisation (Detail)

### 4.1 Regles generales

- Tous les humains sont compatibles
- Moins de 10%: humain
- A partir de 10%: Ange
- Taux de base des Anges: 10% a 50%
- Un Ange ne descend pas sous son taux de base
- A 90%: risque d'echec progressif
- A 100% sans module: transformation monstrueuse

Caps globaux (toutes sources confondues):

- TC max 85% (100% possible)
- DC sans limite
- Precision max 75% (90% possible)
- Ces caps sont globaux et pas forcement atteignables via l'arbre ou les modules.

La COMPAT est la jauge personnelle qui autorise l'Ultime d'un personnage.

- Chaque personnage a son propre seuil de COMPAT pour lancer son Ultime.
- Plus le seuil est eleve, plus l'Ultime doit etre puissant.
- Les competences et les effets peuvent accelerer ou freiner l'acces a ce seuil.

### 4.2 Jauge en combat

La jauge n'augmente pas automatiquement chaque tour.

Elle augmente via:

- Competences energetiques
- Degats recus par monstres d'energie
- Zones a forte densite energetique
- Effets qui modifient la COMPAT ou l'acces a l'Ultime

### 4.3 Stabilisation

Action speciale via module:

- Reduction forte de la jauge (exemple historique: 50%)
- Nombre d'utilisations limite par combat
- Ne descend jamais sous le taux de base

Action de concentration alternative:

- Reduction faible a moyenne (historique: 5% a 20%)
- Utilisation plus flexible
- Ne descend pas sous le taux de base

### 4.4 Humains et zones corrompues

- Les humains jouables sont equipes de protections adaptees.
- Sans protection, ils sont tres vulnerables en zones corrompues.
- En zone tres corrompue, des effets de poison ou d'erosion peuvent s'appliquer.

### 4.5 Cas du noyau

- Aucun Ange standard ne peut interagir avec la masse du noyau sans atteindre 100% et perdre le controle.
- Neo est l'exception canonique.

## 5. Roles et Scaling Detaille

Les valeurs ci-dessous viennent des notes de design initiales. Elles servent de base de tuning et restent ajustables pendant l'equilibrage.

Mis dans GDD Fiches personnage : plus % plus stats

## 6. Equipements et Modules

### 6.1 Philosophie equipement

- Pas de rarete punitive
- Pas de loot jetable
- Equipements uniques par personnage
- Systeme evolutif (ameliorer plutot que remplacer)

### 6.2 Structure equipement

- Equipement initial niveau 1
- Paliers d'evolution successifs
- Emplacements modules qui augmentent avec les niveaux
- Niveaux 2, 4, 5: +100 PV, +50 ATK, +50 DEF fixe
- Niveaux 3 et 6: +1 slot module (max 3 slots)

### 6.3 Modules

Sources d'obtention:

- Exploration
- Quetes
- Boss et semi-boss
- Boutique

Effets possibles:

- Ajouter bonus/malus de stats
- Ajouter effets speciaux

Regles:

- Les modules sont des items uniques (pas de doublons identiques).
- Pas de rarete.
- Chaque module a un effet specifique.
- Retrait et changement de module: gratuit, mais possible uniquement a certains endroits.
- Lieux de modification: QG ou ateliers de modules (au moins 1 par zone).

### 6.4 Slots et limites

- 1 module par slot.
- Nombre de slots augmente avec les paliers d'equipement.
- Max 3 slots.

### 6.5 Types de modules (structure cible)

- Modules stats (ATK, DEF fixe, PV, VIT, TC, DC, Precision)
- Modules compatibilite (gain, paliers, stabilisation)
- Modules utilitaires (effets speciaux, resistances, immunites)

Regles de stacking:
- Les bonus identiques s'additionnent, sauf mention contraire.
- Les caps globaux s'appliquent a toutes les sources.

Caps globaux:

- TC max 85% (100% possible)
- DC sans limite
- Precision max 75% (90% possible)
- Ces caps sont globaux et pas forcement atteignables via l'arbre ou les modules.

### 6.6 Amelioration d'equipement (structure cible)

- Amelioration par paliers, avec cout en ressources + monnaie.
- Chaque palier ajoute des slots ou renforce les stats de base.
- Ressources obtenues via exploration, quetes, boss.

## 7. Progression et Arbres de Competences

### 7.1 Progression

- L'Xp sera de plus en plus donnée en fonction des zones, des zones seront plus dur et donc le niveaux y sera plus grand et donc plus de gain dont l'xp, à chaque actes les nouvelles zones des actes seront plus difficile et donc donneront un xp adapter pour des lvl 50 par exemple .
- Courbe d'xp : elle double après chaque niveaux soit du Lvl 1 à 2 il faut 50 puis du lvl 2 à 3 - 100 etc...
- Xp moyenne par combat : 1 mob de lvl1-5 -> 15xp et augmente de 5xp après chaque cap de lvl (ex : 6-10 -> 20xp; 11-15 -> 25xp...)
- Xp par quete : a definir plus tard selon la difficulte et le type, et varie selon quand elle est obtenable dans l'histoire (quete de combat - quete d'enquete - quete principale).
- Niveau cible par fin d'actes : Acte 1 - lvl 40-45 | Acte 2 - lvl 90-95 | Acte 3 - lvl 140-145 
- Selon l'acte le niveau cap du niveau max augmente : - Niveau max cible: 50 Acte 1 | 100 Acte 2 | 150 Acte 3
- Points de competence distribues a la progression, soit 1 point tou les niveaux sauf, 3 tout les niveau finissant par 5 (5,15,25...) et 5 tout les niveaux finissant par 0 expecter 0 (10,20,30...)cela reste le même pour chaque actes et les point peuvent se cumuler si on ne les dépense pas.

### 7.2 Arbres par role

Chaque personnage a son arbre qui a une base identique:

- Boules reliees entre elles
- Couleurs: Vert (PV), Bleu (DEF fixe), Rouge (ATK), Violet (Precision), Jaune (modif passif/competence)
- Exemples jaunes: +chance de malus, +% degats, nouvel effet, +nb de tours de buff
- Cases avec contour special: buffs plus importants (ex: +5% a +10% ATK max, +200 a +250 DEF fixe max, +200 a +500 PV max, +5% a +10% DC max, +5% a +10% TC max, +5% a +10% soin subi, +5% a +10% Precision)

De plus l'arbre sera de plus en plus grand aux fils des actes.

- Chaque arbre dispose de 225 nodes des l'acte 1. La progression vient des points de competence debloques par niveau.
- Cout des nodes: node simple 2 points, node speciale 5 points (case de base augmentee et violet), node passif/competence 10 points.

## 8. Systeme de Combat Detaille

### 8.1 Structure de tour

Tour par tour lisible, avec une VIT individuelle qui fixe l'ordre d'action.

Regle de base:

- La VIT la plus elevee agit en premier.
- Les bonus/malus de vitesse modifient l'ordre au debut de chaque tour.
- A VIT egale, priorite aleatoire.

Phases:

1. Planification
2. Resolution
3. Fin de tour (statuts, cooldowns, charges)

### 8.2 Actions

- Attaque
- Competence
- Ultime
- Stabilisation (pour ange)
- Objet
- Fuite

### 8.3 Calcul des degats (structure cible)

- Chaque competence/attaque definit son propre ratio dans la fiche du personnage/ennemi.
- La formule exacte est portee par la competence (ex: %ATK, %DEF fixe, degats bruts).
- Ordre general: base du skill -> critique -> buffs/malus de degats.

Formules types (exemples):

- Attaque: degats = ATK * %
- Attaque hybride: degats = (ATK * %) + (DEF fixe * %)
- Degats bruts: degats = %ATK ou %PV manquants (ignore DEF)
- Degats en zone: degats = (ATK * %) sur plusieurs cibles

Regle degats bruts:

- Les degats bruts transpercent tout, sauf les shields (ex: shield de Sam).

Note: pas de resistance aux malus. Seule la Precision determine l'application.

### 8.4 Critique (regle)

- Chance de critique = TC (%).
- Si critique: degats = X + (X * DC/100).

### 8.5 Buffs/Malus et stacks (regles)

- Un personnage peut avoir plusieurs effets en meme temps (pas de limite globale).
- Pour un meme effet: la regle de stack est definie par l'effet lui-meme.
- Certains effets sont uniques (une seule application possible).
- Les stacks sont des cumuls d'un meme effet, pas des effets differents.

### 8.5.1 Shields (regles)

- Un shield a des "PV" qui absorbent des degats.
- Si les degats depassent les PV du shield, le surplus touche les PV.
- Les shields ne se cumulent pas: seul le plus fort reste.

### 8.5.2 Timing des effets

- DoT: debut du tour de la cible.
- Buffs/malus: effet immediat a l'application.
- Durees: decrement a la fin du tour de la cible.

### 8.5.3 Cleanse

- Pas de cleanse pour l'instant.

### 8.5.4 Provocation et Silence

- Provocation force la cible a attaquer celui qui a applique le malus.
- Silence bloque competences et ultimes.

### 8.5.5 Rez

- Rez avec %PV variable selon l'item.

### 8.5.6 Fuite

- Possible contre mobs simples, impossible contre mini-boss ou boss.
- Reussite en % selon situation.

### 8.5.7 IA ennemie (priorites)

- Priorise la cible la plus facile a tuer.
- Cherche la cible sur laquelle elle inflige le plus de degats.
- Si une cible est a portee de KO, elle est priorisee.

### 8.6 Terrain et rencontre

- Ennemis visibles sur map
- Aggro a vue
- Contact pour transition combat

### 8.7 Fuite, respawn, game over

- Fuite possible selon situation
- Respawn present hors exceptions de zones traitees
- En cas de game over: retour QG avec penalite economique partielle

## 9. Ennemis et Ecosysteme Hostile

### 9.1 Types d'ennemis

- Bandits
- Factions hostiles
- Anges hostiles
- Humains modifies
- Monstres corrompus

Familles d'ennemis:

- Bandits(auront plusieurs nom différents) (principalement ChatarraCity, camps)
- Agents d'Eternum (quetes principales)
- Monstres corrompus (proches zones corrompues, parfois ailleurs)
- Anges hostiles (bandits ou adversaires)
- Autres factions (ajout plus tard)

Chaque famille aura un type de chaque archetypes possibles avec un mini-boss et boss.

Archetypes possibles:

- Brute
- Assassin
- Tank
- Support
- Controle
- Sniper
- Mage

Contres par archetype:

- Brute -> focus / ralentissement
- Assassin -> shield / provocation
- Tank -> perforation de defense / malus degats subis / degats bruts
- Support -> focus prioritaire
- Controle -> immunite / precision (cleanse si ajoute plus tard)
- Sniper -> vitesse / engage rapide
- Mage -> silence


### 9.2 Boss

- Reserve de PV importante
- Interactions possibles avec la jauge de compatibilite
- Pression tactique sur la gestion des ressources

Regles:

- Les stats des mobs, mini-boss et boss sont definies a l'avance sur leur fiche.
- Certains boss ont deux phases.

Mini-boss de camps:

- Un mini-boss par camp/zone.
- Battu une seule fois (unique).
- Les autres mobs restent farmables.

### 9.3 Scaling ennemi

- Niveaux differents par zone
- Courbe de difficulte progressive
- Variations de PV, ATK, DEF selon archetypes

Regles de scaling:

- Les memes ennemis peuvent avoir des niveaux differents dans une meme zone.
- Les stats augmentent avec le niveau (par tranche de 5 niveaux).

Progression des zones (logique):

- Carte semi-ouverte avec zones accessibles des le debut.
- Certaines zones sont trop difficiles et demandent un retour plus tard.
- D'autres zones sont verrouillees par quete ou action.
- Debut du jeu: orphelinat -> exterieur de l'orphelinat -> centre de ChatarraCity.
- Tuto integre via les zones (montrer sans texte, laisser le joueur comprendre).

Grille niveaux par zones (acte 1):

- Orphelinat: lv0 (pas de combats)
- Centre de ChatarraCity: lv1-5
- Sud du centre (zone decheterie / QG Fallen Angels): lv1-5
- Exterieure Est du centre: lv5-10
- Est centre Chatarra: lv10-15
- Exterieure Nord Est du centre: lv15-20
- Exterieure Sud Est du centre: lv15-20
- Banlieue ChatarraCity: lv20-25
- Bidonville: lv20-25
- Exterieure Nord du centre: lv25-30
- Zone Nord Ouest: lv30-35
- Frontiere ChatarraCity / DivusPolice: lv35-40

Zones corrompues:

- Les ennemis y sont plus dangereux que ceux du meme niveau.
- Plus de mobs que d'habitude.
- Une fois la zone nettoyee, les mobs ne reapparaissent plus.

Loot:

- Argent toujours.
- Objets parfois (taux 20%).
- Objets de quete si requis par une quete.

IA par archetype:

- Assassin -> focus supports.
- Brute -> frappe tout.
- Tank -> essaie de provoquer.
- Support -> soigne en priorite ses allies.
- Controle -> applique des malus en priorite sur ceux qui n'en ont pas.
- Sniper -> focus DPS.
- Mage -> attaque libre.

## 10. Architecture Technique (Design cible)

### 10.0 Base technique

- Moteur cible: Godot 4
- Approche data-driven
- Donnees parametreables

### 10.1 Organisation projet

- Scenes
	- boot
	- world
	- combat
	- ui
	- dialogues
	- items
	- modules
	- factions
	- economy

- Core
	- managers
	- systems
	- services
- Data
	- characters
	- skills
	- status
	- enemies
	- zones
	- quests
	- dialogues
	- items
	- modules
	- factions
	- economy

### 10.2 Managers cibles

- GameManager (cycle global, sauvegarde, etats du jeu)
- ZoneManager (chargement zone, transitions, encounters)
- CombatManager (tour, actions, resolution, etats)
- CharacterManager (party, stats, progression, build)
- QuestManager (quetes, objectifs, journal, progression)
- DialogueManager (dialogues, choix, flags)
- GaugeManager (COMPAT, jauges annexes)
- InventoryManager (items, modules, equipements)
- EconomyManager (monnaie, couts, boutiques)

Note: pour un solo dev, 7-9 managers suffisent. On peut commencer avec ceux-ci et en fusionner si besoin.

### 10.3 Donnees cibles

- characters
- skills
- status
- enemies
- equipment
- zones
- quests
- dialogues
- items
- modules
- factions
- economy

### 10.4 Flux principal (cycle gameplay)

1. Exploration de zone
2. Rencontre (ennemis visibles / declencheur)
3. Combat (actions, effets, recompenses)
4. Loot et progression (XP, monnaie, modules)
5. Journal et quetes (mise a jour indices/hypotheses)
6. Deblocage zone ou retour QG

### 10.5 Journal et Enquete (structure cible)

Types de quetes:

1. Quetes simples
	- Objectif simple (combat, collecte, livraison, decorromption)
	- Avancement rapide
	- Recompense selon la difficulte de la quete

2. Quetes d'enquete
	- Indices trouves via exploration, enigmes ou dialogues
	- Hypotheses reliees aux indices mis dans le journal
	- Revelation lorsque le bon ensemble d'indices est reuni
	- Deduction basee sur les indices, avec possibilite d'aide

Structure du journal:

- Onglets: Quetes, Indices, Hypotheses, Personnages, Zones
- Indice: source, lieu, date, lien vers une hypothese
- Hypothese: conditions de validation (liste d'indices requis), chaque enquête aura sa page avec ses indices.
- Avancement dans l'histoire principale

Format d'un indice (fiche courte):

- Nom
- Description courte
- Source (PNJ, objet, zone, combat, document)
- Lieu
- Date/chapitre
- Lien vers hypothese(s)
- Importance (normal / important)

Regles d'enquete:

- Les hypotheses demandent un ensemble precis d'indices (pas un simple compte).
- Les indices sont ajoutes automatiquement dans le journal .
- Progression libre: l'ordre des etapes peut varier tant que les indices requis sont reunis.
- Pas d'echec definitif d'enquete.
- Aide optionnelle: indique les indices importants a trouver.

Forme de l'aide:

- Lorsqu'on active l'aide, les indices importants sont mis en surbrillance dans le journal.

Regles d'accessibilite:

- Tout est visible dans le journal (rien de cache)
- Les elements manquants sont clairs (indices requis qui ne sont pas trouves)
- L'interface reste lisible pour un joueur non expert

Exemple d'enquete (court):

- Quete: "Disparitions dans le quatier"
- Objectif: identifier la cause des disparitions
- Indices importants:
	- Rapport d'ouvrier: bruits metalliques la nuit (PNJ)
	- Trace d'energie: residu instable pres des conduits (zone)
	- Document interne: maintenance annulee depuis 2 semaines (document)
- Hypothese: activite illegale dans les conduits
- Revelation: acces a une zone cachee + combat de mini-boss

### 10.6 Interface globale (structure cible)

Menu principal (hub): Journal

Sous-interfaces accessibles depuis le journal:

- Inventaire
- Equipe (arbres des personnages + capacites)
- Infos (quetes, personnages, enquete, objets, documents)
- Carte (débloquer en progressant dans la zone)
- Options
- Quitter le jeu

Interface combat (infos essentielles):

- PV et COMPAT (jauges speciales si besoin) ennemis comme alliée
- Buffs/malus/effets actifs + cooldowns
- Ordre d'action
- Liste des competences + selection
- Statistiques ally/enemy en combat (avec effets)
- Boutons: Fuite, Concentration (anges)

HUD exploration:

- Pas de mini-map
- Pings visibles sur la carte quand elle est ouverte
- Aide dans les options pour indiquer une destination (fleche sur batiment cible)

Feedback visuel/sonore:

- Feedback visuel et sonore pour crit, malus applique, aide active, zone corrompue autre mais pas idée

## 11. Roadmap Solo Dev

### 11.1 Pre-production

- Consolidation GDD
- Prototype combat
- Base architecture

### 11.2 Vertical slice

- Une zone complete
- Trois personnages
- Un boss
- Enquete jouable de bout en bout

### 11.3 Production

- Integration des zones
- Arbres de competences
- Systeme complet

### 11.4 Polish

- Equilibrage
- UX/UI
- Corrections bugs

## 12. Risques Projet

- Scope creep
- Surcharge systemique
- Complexite de tuning
- Complexite de tuning
- Charge solo de production

## 13. Quetes secondaires, factions et affinite

Factions concernees:

- Revolutionnaires
- Culte (a confirmer)
- Peuple du bidonvilles
- Peuple de ChatarraCity
- Fallen Angels
- Archanges (acte 3)

Affinite:

- L'affinite ne baisse pas, elle ne fait que monter.
- Jauge de 0 a 1000.
- Seuils: 0-200 hostile, 200-400 neutre, 400-600 allie, 600-800 amis, 800-1000 membre honoraire.

Gagner de l'affinite:

- Quetes secondaires
- Quetes de faction (chasse de monstres, fedex)
- Donations

Valeurs de gain:

- Grosse quete en 2 parties: 100 points par partie.
- Quetes de faction: 8 quetes a faire, 50 points chacune.
- Donations: jusqu'a 400 points au total (10000 "monnaie").

Recompenses d'affinite:

- Deblocage de zones
- Prix reduits
- Quetes exclusives
- Acces a certaines fins
- Deblocage de personnage (selon faction)
- Objets/modules/documents donnes

Types de quetes secondaires:

- Chaines de quetes (histoire secondaire)
- Quetes isolees (histoire courte en 1 quete)
- Quetes de faction (chasse / fedex)
- Quetes speciales (vagues d'ennemis)

## 14. Economie Detaillee

### 13.1 Monnaie

- Monnaie principale unique (nom a definir).
- Gagnee via affrontements, quetes, exploration.

### 13.2 Boutiques et services

- Achat de modules et materiaux d'amelioration.
- Soins et remise en forme a la base.
- Ajustement de build (retirer/remplacer des modules).
- Pour soigner entierement toute l'equipe, il faut se rendre dans un lieu dedie (nom a definir) ou utiliser des ressources achetees pour soigner.
- Achat de documents (infos, lore, indices).
- Achat d'items importants (cles, acces de zone, items de quete).
- Amelioration d'equipement (paliers).

### 13.3 Scaling des couts

- Les prix augmentent a chaque acte.
- Les couts restent proportionnels au niveau cible de la zone.

### 13.4 Recompenses (structure cible)

- Combat: monnaie + ressources, varie selon niveau et type d'ennemi.
- Quete simple: monnaie + ressources + module possible.
- Quete d'enquete: monnaie + ressources + module possible.
- Quete principale: monnaie + progression narrative + acces a nouvelles zones + module possible.

### 13.5 Depenses prioritaires

- Evolution d'equipement (palier).
- Principalement pour l'Achat de modules ou ressources rares.
- Pour découvir des zones

### 13.6 Table de prix (fixes par acte)

Acte 1:
- Soin individuel: 100
- Soin de groupe: 250
- Ressource de rez: 350


Acte 2:
- Soin individuel: 200
- Soin de groupe: 500
- Ressource de rez: 700


Acte 3:
- Soin individuel: 400
- Soin de groupe: 1000
- Ressource de rez: 1400


### 13.7 Prix (tout le reste)

Acte 1:
- Module standard: 450
- Document (info/indice): 250
- Item important (cle/zone/quete): 600
- Amelioration equipement (palier): 800
- Ajustement de build (changement modules au lieu dedie): 0 (gratuit)

Acte 2:
- Module standard: 1000
- Document (info/indice): 500
- Item important (cle/zone/quete): 1200
- Amelioration equipement (palier): 1700
- Ajustement de build (changement modules au lieu dedie): 0 (gratuit)

Acte 3:
- Module standard: 1900
- Document (info/indice): 900
- Item important (cle/zone/quete): 2200
- Amelioration equipement (palier): 3500
- Ajustement de build (changement modules au lieu dedie): 0 (gratuit)

Sources de revenus:

- Affrontements
- Quetes
- Exploration

Depenses principales:

- Modules
- Ressources
- Soins
- Amelioration des equipements
- Ajustement de build

## 15. Relation avec le Master

Ce document conserve les details systemes.
Le fichier Documentation/Doc_EOM.md reste la source canonique resumee.
