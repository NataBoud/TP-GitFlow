# E-Commerce 

## Structure du Projet

- **master** : Contient la version stable du projet.
- **develop** : Contient les fonctionnalités en cours de développement.
- **feature/** : Branches de développement de fonctionnalités spécifiques.
- **release/** : Branches pour la préparation des versions de release.
- **hotfix/** : Branches pour la correction des bugs critiques détectés en production.

## Workflow GitFlow

1. **Développement des Fonctionnalités :**
   - Créer une branche `feature` à partir de `develop`.
   - Développer la fonctionnalité sur cette branche.
   - Fusionner la branche `feature` dans `develop` une fois terminée.

2. **Préparation d’une Release :**
   - Créer une branche `release` à partir de `develop`.
   - Effectuer des tests et corrections sur cette branche.
   - Fusionner la branche `release` dans `master` et `develop`.

3. **Gestion des Bugs Critiques :**
   - Créer une branche `hotfix` à partir de `master`.
   - Corriger le bug et fusionner la branche dans `master` et `develop`.

## Fonctionnalités Développées

### Gestion des Utilisateurs
- Inscription, connexion, gestion du profil des utilisateurs.

### Catalogue des Produits
- Ajout, modification, suppression des produits disponibles à la vente.

### Gestion des Commandes
- Création, suivi et annulation des commandes.

## Scénarios de Bugs et Conflits

- **Bug Critique d'Affichage :**
  - Détecté et corrigé dans la branche `hotfix/critique-affichage`.

- **Conflit sur `conflit.txt` :**
  - Conflit créé intentionnellement sur deux branches `feature` et résolu manuellement.

## Règles de Contribution

- Utilisez des messages de commit clairs et explicites.
- Documentez les changements majeurs dans le fichier `CHANGELOG.md`.


##### **Rétro-planning**
| Étape                          | Date Prévue     | Date Réelle       |
|--------------------------------|-----------------|-------------------|
| Initialisation du Projet       | 27/09/2024      | 27/09/2024        |
| Développement des Fonctionnalités | 27/09/2024      | 27/09/2024        |
| Fusion des Fonctionnalités     | 27/09/2024      | 27/09/2024        |
| Préparation de la Release      | 27/09/2024      | 27/09/2024        |
| Correction de Bugs Critiques   | 27/09/2024      | 27/09/2024        |
| Résolution des Conflits        | 27/09/2024      | 27/09/2024        |