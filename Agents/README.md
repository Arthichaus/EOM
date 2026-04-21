# Système d'Agents — EchoOfMemory

Ce dossier contient une configuration **simple** d'agents spécialisés pour travailler dans VS Code en mode vibe coding.

## Objectif

Pipeline cible :

1. Tu décris une idée (libre ou via template).
2. L'agent principal analyse la demande.
3. Il délègue aux agents spécialisés nécessaires.
4. Les documents du projet sont mis à jour.
5. Si la demande est design-only, aucun code n'est généré.

## Fichiers principaux

- `00_Principal_Orchestrateur.md`
- `10_Narrative_Lore.md`
- `20_Game_Design.md`
- `30_Quest_Level_Design.md`
- `40_Combat_Balance.md`
- `90_Documentation_QA.md`
- `Workflow_Execution.md`
- `Templates/Idee_Request_Template.md`
- `Templates/Agent_Output_Template.md`

## Règle d'or

Si une information manque, l'agent **pose des questions**. Il n'invente pas.

## Utilisation rapide

1. Ouvre `Templates/Idee_Request_Template.md`.
2. Décris ton besoin.
3. Lance l'agent principal avec le prompt de `00_Principal_Orchestrateur.md`.
4. Laisse l'orchestrateur appeler les agents spécialisés selon la matrice de `Workflow_Execution.md`.
