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

utilisateurs
produits
commandes

Dans chaque branche, on ajoute des fichiers et commentaires simulant le développement des fonctionnalités avec des commits explicites :

````bash
git commit -m "feat(GitFlow): ✨ Demarrage du projet
"
````

4. Fusion des Fonctionnalités
Une fois chaque fonctionnalité simulée et les commits effectués, nous avons fusionné chaque branche feature dans la branche develop :

Fusion de feature/utilisateurs :
````bash
git checkout develop
git merge utilisateurs

````
5. Préparation d’une Version Finale

6. Fusion et Tagging