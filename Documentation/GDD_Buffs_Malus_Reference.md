# GDD — Référentiel Buffs, Malus et États
## Page de référence

Cette page centralise les buffs, malus et états utilisés par le système de combat. Elle sert de source de référence pour l'équilibrage, les fiches personnages et les futurs modules d'effets.

---

## Regles de lecture

- Chaque effet doit avoir un nom unique.
- Chaque effet doit preciser s'il est un buff, un malus ou un etat neutre.
- Chaque effet doit indiquer sa duree, sa portee et sa source principale.
- Les effets de vitesse modifient la VIT et donc l'ordre d'action.

---

## Buffs

| Nom | Type | Effet | Duree | Sources | Notes |
|---|---|---|---|---|---|
| Buff offensif | Buff | Augmente les degats infliges. | A definir | Angel, modules, competences | Terme generique a decliner selon les sous-types. |
| Buff defensif | Buff | Augmente la resistance ou la defense. | A definir | Angel, Freya, modules | Peut inclure bouclier ou protection. |
| Buff de precision | Buff | Ameliore la PREC et la fiabilite des actions. | A definir | Modules, techniques de soutien | Impacte les attaques et les effets utilitaires. |
| Buff de compatibilite | Buff | Augmente la COMPAT ou facilite l'acces a l'Ultime. | A definir | Modules, progression, soutien | Lie directement au seuil d'ultime du personnage. |
| Hote | Buff | Augmente la VIT et/ou l'ordre de priorite. | A definir | Competences, modules | A utiliser pour les personnages rapides. |
| Buff d'attaque critique | Buff | Augmente les chances ou les degats critiques. | A definir | DPS, modules, synergies | A garder rare pour ne pas exploser l'equilibrage. |
| Buff de soins | Buff | Augmente les soins prodigues ou recus. | A definir | Support, purification | Utile pour les personnages de soutien. |
| Regeneration | Buff | Rend des PV sur la duree. | A definir | Soins, purification, boucliers avances | Peut se cumuler avec soins directs. |
| Bouclier | Buff | Absorbe des degats avant les PV. | A definir | Freya, Sam, modules | S'epaissit ou se renouvelle selon le cas. |
| Immunite aux malus | Buff | Bloque une ou plusieurs categories de malus. | A definir | Purification, protection, Ultimes | Peut etre total ou partiel. |
| Cleanse | Buff | Retire un ou plusieurs malus existants. | A definir | Support, purification, protection | A utiliser comme contre-jeu aux debuffs. |
| Provocation positive | Buff | Force les ennemis a cibler le porteur. | A definir | Tanks | Sert a proteger les allies plus fragiles. |
| Fortification | Buff | Reduit les degats recus pendant une courte duree. | A definir | Tanks, modes defensifs | Plus simple que le bouclier pour la lisibilite. |
| Aura de zone | Buff | Applique un effet de soutien aux allies proches. | A definir | Supports, zones, terrain | Effet passif ou de zone.

---

## Malus

| Nom | Type | Effet | Duree | Sources | Notes |
|---|---|---|---|---|---|
| Enflamme | Malus | Inflige des degats sur la duree. | 3 tours ou plus | Jade, attaques de feu | Exemple deja utilise dans les fiches. |
| Gelure | Malus | Reduit la VIT | 2 tours ou plus | Jade, attaques de glace | Sert directement a l'ordre de tour. |
| Empoisonnement | Malus | Inflige des degats sur la duree. | 3 tours ou plus | Jade, toxines | Effet continu, souvent cumulable. |
| Fragilisation | Malus | Augmente les degats subis. | A definir | Jade, debuffs offensifs | Peut s'empiler par intensite ou duree. |
| Ralentissement | Malus | Reduit la VIT | A definir | Controle, pression, glace | Peut etre different de Gelure selon la severite. | (peut être mis une seule fois sur un ennemie, prends le taux le plus élevé selon le debuff)
| Immobilisation | Malus | Empêche d'agir lorsque son tour arrive | A definir | Controle, entraves | Considérer comme un stun |
| Silence | Malus | Bloque les competences ou certains pouvoirs. | A definir | Debuffs magiques, modules anti-combat | A ajouter si valide par le gameplay. |
| Provocation | Malus | Force la cible a viser une priorite donnee. | A definir | Tanks, protections | Peut aussi etre classe comme contrainte de cible. |
| Brisure | Malus | Reduit l'efficacite de la DEF ou des protections. | A definir | Anti-tank, attaques lourdes | A utiliser comme contre aux tanks. |
| Saignement | Malus | Inflige des degats sur la duree et penalise le tempo. | A definir | Lames, coups critiques, blessures | Variante plus brutale que l'empoisonnement. |
| Fragilite mentale | Malus | Diminue la fiabilite des actions et des effets. | A definir | Controle, pression psychique, souvenirs | Bien adapte a Néo et aux themes mentaux. |
| Anti-soin | Malus | Reduit ou annule les soins recus. | A definir | Debuffs offensifs, corruption | Important pour les combats de longue duree. |
| Drain de compatibilite | Malus | Baisse la COMPAT ou retarde l'acces a l'Ultime. | A definir | Corruption, attaques de noyau | Lie directement au risque de transformation. |
| Marquage | Malus | Rend une cible plus facile a toucher ou suivre. | A definir | Chasseurs, traque, scan | Peut remplacer un simple bonus de precision ennemi. |

---

## Etats speciaux

| Nom | Type | Effet | Duree | Sources | Notes |
|---|---|---|---|---|---|
| Etat neutre | Etat | Aucun effet actif de gemme ou d'etat majeur. | Permanent | Base de combat | Sert de point de depart. |
| Etat gemme | Etat | Active un effet de gemme sur le personnage. | Variable | Jade | Etat central de la logique gemme. |
| Etat critique | Etat | Personnage proche de la rupture ou du seuil de risque. | Variable | COMPAT, transformations | A raccorder a la jauge d'ultime. |
| Etat stabilise | Etat | Reduit le risque de rupture et protege des pics de malus. | Variable | Modules, soins, actions de support | Utile pour les phases de securisation. |
| Etat surcharge | Etat | Augmente fortement l'efficacite mais expose davantage aux contreparties. | Variable | DPS, modes offensifs | Bon levier de risque/recompense. |
| Etat corrompu | Etat | Le personnage subit une pression de corruption ou de deconnexion. | Variable | Boss, noyau, corruption energetique | Peut etre lie a la trame principale. |
| Etat intouchable | Etat | Ignore temporairement certains types d'attaques ou de malus. | Tres court | Ultimes, mecanismes rares | A utiliser avec parcimonie. |

---

## A completer

- Ajouter les valeurs numeriques exactes de chaque effet.
- Ajouter les conversions si tu veux des versions faible / moyenne / forte.
- Ajouter les effets specifiques aux armes et aux gemmes.
- Ajouter les interactions exactes entre buff, malus, cleanse et immunite.