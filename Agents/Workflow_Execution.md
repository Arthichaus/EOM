# Workflow d'Exécution

## 1) Entrée utilisateur

Deux modes :

- **Mode libre** : description naturelle.
- **Mode template** : fichier rempli via `Templates/Idee_Request_Template.md`.

## 2) Tri initial par l'Orchestrateur

L'orchestrateur classe la demande :

- `DESIGN`
- `CODE`
- `MIXTE`

Puis il détecte les domaines concernés (lore, game design, quêtes, balance, QA docs).

## 3) Appels inter-agents

L'orchestrateur appelle les spécialistes au format `CALL_AGENT`.

### Matrice d'appel recommandée

| Besoin | Agents minimum | Agent final obligatoire |
|---|---|---|
| Lore / Personnages / Fins | Narrative | Documentation QA |
| Système de jeu | Game Design | Documentation QA |
| Quêtes / Actes / Niveau | Quest & Level + Narrative | Documentation QA |
| Équilibrage combat | Combat & Balance + Game Design | Documentation QA |
| Feature mixte complète | Narrative + Game Design + Quest/Level + Combat | Documentation QA |

## 4) Mise à jour documentation

Niveau de rigueur choisi : **Standard**

- Mettre à jour les sections touchées.
- Ajouter un journal synthétique des changements si la modification est majeure.
- Éviter de dupliquer les mêmes informations dans plusieurs documents.

## 5) Politique DESIGN vs CODE

- Si la demande est `DESIGN` : docs uniquement.
- Si `CODE` : code + doc impactée.
- Si `MIXTE` : d'abord design validé, puis code minimal utile.

## 6) Sortie finale

Toujours livrer :

1. Résumé.
2. Décisions prises.
3. Modifications docs (fichiers + sections).
4. Roadmap détaillée (prochaines étapes).
5. Questions en attente (si blocages).
