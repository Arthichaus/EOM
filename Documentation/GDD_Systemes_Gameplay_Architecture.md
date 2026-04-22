# GDD - Systemes Gameplay et Architecture

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

Exemples de zones:

- District central de ChatarraCity
- Districts de ChatarraCity
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

## 4. Anges, Compatibilite et Stabilisation (Detail)

### 4.1 Regles generales

- Tous les humains sont compatibles
- Moins de 10%: humain
- A partir de 10%: Ange
- Taux de base des Anges: 10% a 50%
- Un Ange ne descend pas sous son taux de base
- A 90%: risque d'echec progressif
- A 100% sans module: transformation monstrueuse

### 4.2 Jauge en combat

La jauge n'augmente pas automatiquement chaque tour.

Elle augmente via:

- Competences energetiques
- Degats recus par monstres d'energie
- Zones a forte densite energetique

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

### 5.1 Base commune

- Lvl 1: base de PV faible
- Progression lineaire jusqu'au niveau 50
- Ajustements par role ensuite

### 5.2 DPS

Intentions de design:

- Forte montee offensive avec prise de risque
- Buffs progressifs selon paliers de compatibilite
- Contreparties croissantes a haut taux

Historique de paliers:

- 25%: bonus attaque leger
- 50%: bonus attaque et critique avec contrepartie
- 75%: pic offensif moyen
- 90%: gros pic offensif avec risque eleve
- 100%: etat critique terminal

### 5.3 Tank

Intentions de design:

- Defense et controle de l'aggro
- Resistance accrue aux debuffs
- Outils de protection du groupe

Historique de paliers:

- 25%: bonus defense
- 50%: resistances supplementaires
- 75%: tanking renforce
- 90%: provocation de masse possible
- 100%: etat critique terminal

### 5.4 Support

Intentions de design:

- Choix entre voie debuff et voie soin/protection
- Hausse utilitaire selon les paliers
- Contreparties a haut taux

Historique de paliers:

- 25%: bonus moderes
- 50%: specialisation de role
- 75%: role affirme
- 90%: impact maximal de role avec risque
- 100%: etat critique terminal

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

### 6.3 Modules

Sources d'obtention:

- Exploration
- Quetes
- Boss et semi-boss
- Boutique

Effets possibles:

- Modifier gain de compatibilite
- Modifier paliers
- Modifier stabilisation
- Ajouter bonus/malus de stats
- Ajouter effets speciaux

## 7. Progression et Arbres de Competences

### 7.1 Progression

- XP via combats, quetes, exploration et activites de zone
- Niveau max cible: 50
- Points de competence distribues a la progression

### 7.2 Arbres par role

DPS:

- Voie monocible
- Voie zone

Tank:

- Voie absorbtion
- Voie brute defensive

Support:

- Voie debuff
- Voie soin/buff

Humains:

- Branches liees aux armes energetiques et a la gestion du risque

## 8. Systeme de Combat Detaille

### 8.1 Structure de tour

Tour par tour lisible, sans stat de vitesse globale dominante.

Phases:

1. Planification
2. Resolution
3. Fin de tour (statuts, cooldowns, charges)

### 8.2 Actions

- Attaque
- Competence
- Ultime
- Stabilisation
- Objet
- Fuite

### 8.3 Terrain et rencontre

- Ennemis visibles sur map
- Aggro a vue
- Contact pour transition combat

### 8.4 Fuite, respawn, game over

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

### 9.2 Boss

- Reserve de PV importante
- Interactions possibles avec la jauge de compatibilite
- Pression tactique sur la gestion des ressources

### 9.3 Scaling ennemi

- Niveaux differents par zone
- Courbe de difficulte progressive
- Variations de PV, ATK, DEF selon archetypes

## 10. Architecture Technique (Design cible)

### 10.1 Base technique

- Moteur cible: Godot 4
- Approche data-driven
- Donnees parametreables

### 10.2 Organisation projet

- Scenes
- Zones
- Combat
- UI
- Core
- Data

### 10.3 Managers cibles

- GameManager
- ZoneManager
- CombatManager
- CharacterManager
- QuestManager
- DialogueManager
- GaugeManager

### 10.4 Donnees cibles

- characters
- skills
- equipment
- zones
- factions

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
- Charge solo de production

## 13. Economie Detaillee

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

## 14. Relation avec le Master

Ce document conserve les details systemes.
Le fichier Documentation/Doc_EOM.md reste la source canonique resumee.
