# TP-GitFlow

Étapes du Projet
1. Initialisation du Projet
Création du dépôt Git : Initialisation d'un dépôt Git pour le projet.
Mise en place des branches GitFlow :
Création des branches de base : main (branche de production) et develop (branche de développement principal).
2. Planification des Fonctionnalités

Fonctionnalité 1 : utilisateurs (inscription, connexion, gestion du profil).
Fonctionnalité 2 : produits (ajout, modification, suppression de produits).
Fonctionnalité 3 : commandes (création, suivi, annulation).
3. Simulation du Développement des Fonctionnalités
Pour chaque fonctionnalité, une branche spécifique a été créée à partir de develop :

- branch utilisateurs
- branch produits
- branch commandes

Dans chaque branche, on ajoute des fichiers et commentaires simulant le développement des fonctionnalités avec des commits explicites :

````bash
git commit -m "feat(GitFlow): ✨ Demarrage du projet
"
````

4. Fusion des Fonctionnalités
Une fois chaque fonctionnalité simulée et les commits effectués, on fusionne chaque branche feature dans la branche develop :

Fusion de feature/utilisateurs :
````bash
git checkout develop
git merge utilisateurs

````
5. Préparation d’une Version Finale

- Création de la branche release/1.0.0 pour simuler la préparation de la version finale.

- Sur cette branche, un commit a été ajouté pour simuler des corrections mineures et des ajustements de bugs.
Example : 
````bash
git commit -m "Correction d’un bug mineur dans la gestion des utilisateurs"

````

6. Fusion et Tagging
````bash
git tag v1.0.0
git push origin v1.0.0

````

7. Simulation d’un Bug en Production
Un bug critique a été simulé sur la branche main.

8. Gestion des Conflits
On simule un conflit en modifiant le même fichier sur deux branches différentes :
ici sur main et sur utilisateurs.

9. Rétro-planning et Reporting
Les différentes étapes du projet ont été réalisées selon un planning structuré :

Initialisation du projet et création des branches.
Développement simulé des fonctionnalités et commits explicites.
Fusion des fonctionnalités dans develop.
Préparation et correction de bugs sur la branche release.
Tagging des versions et simulation d’un bug en production.
Résolution de conflits et finalisation du projet.
