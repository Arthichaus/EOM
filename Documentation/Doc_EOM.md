# Doc EOM - Master Resume

Ce document est le resume global du projet.
Il centralise les informations essentielles sans entrer dans les details de production.
Les GDD specialises sont les complements detailles par domaine.

## Regles Canoniques

1. Nom officiel de la basse-ville: ChatarraCity.
2. Le monde repose sur deux villes superposees: DivusPolice (haute-ville) et ChatarraCity (basse-ville).
3. Il y a exactement 4 Familles majeures: TIATORIUS, ARTISA, COMPUTATIO, ARTIFICIUM.
4. Le jeu comporte 4 fins: 2 mauvaises fins, 1 vraie fin, 1 fin ambigue.
5. L'energie artificielle provient de l'Energie Pure et de l'evenement lie aux 5 Legendes.
6. Les Anges sont immunises a la corruption environnementale.
7. Les humains non proteges sont vulnerables a la corruption environnementale.
8. Atteindre 100% de compatibilite sans module entraine perte de controle et transformation en monstre d'energie.
9. En combat, le module peut forcer un KO a 100% pour eviter la transformation.
10. Aucun Ange ne peut entrer dans la masse du noyau d'energie artificielle sans atteindre 100% et perdre le controle.
11. Neo est l'exception connue: il peut atteindre 100% et rester conscient, puis interagir avec le noyau.
12. Le present document est un master resume. Les GDD specialises sont la reference detaillee par sujet.

## Concept Fondamental

RPG 2D top-down solo, style Pokemon, avec une ambiance futur proche sombre et mature.
Le joueur dirige une equipe de 4 agents qui enquete sur une entite criminelle invisible manipulant les deux villes.
L'enquete et les choix narratifs priment sur la confrontation brute.

## Univers Et Monde

- DivusPolice: ville haute, stable, elite politique et economique.
- ChatarraCity: ville basse, precarite sociale, violence, instabilite energetique.
- Energie artificielle: source de progres industriel, de pouvoirs, et de corruption.
- Corruption: affecte surtout l'environnement et les etres vivants vulnerables, avec des effets graves sur les humains non proteges.

## Factions (Vue Resumee)

- Directoire / Doyens
- Maire
- 4 Familles: TIATORIUS, ARTISA, COMPUTATIO, ARTIFICIUM
- Archanges
- Eternum
- Fallen Angels
- Culte
- Revolutionnaires
- Civils de DivusPolice et de ChatarraCity

Chaque faction influence les quetes, l'acces aux zones, et certains arcs de fin.

## Narration (Vue Resumee)

- Narration lourde: trame principale, antagonistes majeurs, arcs des personnages jouables.
- Narration legere: lore environnemental, notes, archives, histoire des quartiers.
- Themes: corruption, inegalites sociales, manipulation industrielle, pouvoir, perte d'humanite.

## Compatibilite Et Anges

- Tous les humains sont compatibles.
- Moins de 10%: humain (non Ange).
- A partir de 10%: Ange.
- Taux de base des Anges: 10% a 50%.
- Un Ange ne descend jamais sous son taux de base.
- A partir de 90%: risque d'echec progressif en combat.
- A 100% sans module: transformation monstrueuse.

## Neo (Exception Canonique)

Neo possede la capacite Souvenir (lecture, blocage, vol et brisure de souvenirs).
Il peut reproduire de facon affaiblie un pouvoir vole.
Son cas est unique: il peut atteindre 100% tout en restant conscient, ce qui permet son interaction avec le noyau.

## Boucle De Gameplay

1. Exploration
2. Enquete (indices, hypotheses, journal)
3. Quetes secondaires et quetes de factions
4. Quete principale
5. Combat
6. Revelation narrative
7. Retour QG et deblocage de nouvelles zones

## Structure Du Monde

Carte modulaire type Pokemon, transitions zone par zone.

Types de zones:
- Stables
- Corrompues temporaires (decorrompables)
- Corrompues permanentes

La decorromption devient une activite secondaire majeure apres deblocage dans la trame principale.

## Systeme De Combat (Resume)

- Tour par tour lisible, sans statistique de vitesse globale.
- Actions de base: Attaque, Competence, Ultime, Stabilisation, Objet, Fuite.
- Les competences energetiques font monter la compatibilite.
- Stabilisation via modules et actions dediees.
- Boss plus resistants, avec interactions possibles sur la jauge.

## Progression Et Build

- XP via combats, quetes, exploration.
- Arbres de competences par role.
- Equipements uniques et evolutifs (pas de loot jetable).
- Modules a impact systemique (compatibilite, paliers, stabilisation, bonus/malus).

## Personnages

Le roster cible est de 13 personnages jouables (Anges et humains).
Le detail complet des fiches, stats, arcs et voies de progression est maintenu dans le GDD dedie.

## Technique Et Production

- Moteur cible: Godot 4
- Approche data-driven
- Organisation par managers et donnees parametrees
- Roadmap solo-dev en 4 phases: pre-production, vertical slice, production, polish

## Economie

La monnaie s'obtient via affrontements, quetes et exploration.
Elle sert a acheter des ressources, soigner, ameliorer les equipements et ajuster les builds.

## Documents De Reference Detaillee

- Lore fondateur: Documentation/GDD_5Legendes_PremiereGuerre.md
- Antagonistes et fins: Documentation/GDD_Antagonistes_Fins_v2.md
- Factions et Archanges: Documentation/GDD_Factions_Archanges.md
- Fiches personnages: Documentation/GDD_FichesPersonnages.md
- Personnages non jouables: Documentation/GDD_Personnages_NonJouables.md
- Systemes gameplay et architecture: Documentation/GDD_Systemes_Gameplay_Architecture.md

## Maintenance Du Master

Toute nouvelle decision canonique doit d'abord etre resumee ici.
Ensuite, les GDD specialises sont mis a jour avec le niveau de detail adapte.
