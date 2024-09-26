1. Initialisation du dépôt.

```bash
git init correction-tp-1  && cd correction-tp-1
git checkout -b develop
echo "Projet Ecommerce" > README.md
git add .
git commit -m "Initial commit with README.md and develop branch"

cd ..
mkdir server-correction-tp && cd server-correction-tp
git init --bare

git remote add origin file://'C:\Users\Administrateur\Desktop\CDA5\GIT\server-correction-tp'
git push --set-upstream origin develop
```

2. Création des branches de fonctionnalité

```bash
git checkout -b feature/gestion-utilisateurs
git push origin feature/gestion-utilisateurs
git checkout develop
git checkout -b feature/catalogue-produits
git push origin feature/catalogue-produits
git checkout develop
git checkout -b feature/gestion-commandes
git push origin feature/gestion-commandes
git checkout develop
```

3. Commits simulés pour les fonctionnalités

```bash
git checkout feature/gestion-utilisateurs
echo "Strcuture de la gestion des utilisateurs " > users.txt
git add .
git commit -m "Ajout de la structure de gestion des utilisateurs"
echo "Ajout de la fonctionnalité d'inscription " >> users.txt
git commit -am "Ajout de la fonctionnalité d'inscription"
git push 

git checkout feature/catalogue-produits
echo "Strcuture de la gestion des produits " > products.txt
git add .
git commit -m "Ajout de la structure de gestion des produits"
echo "Ajout de la fonctionnalité d'ajout de produit " >> products.txt
git commit -am "Ajout de la fonctionnalité d'ajout de produit"
git push 

git checkout feature/gestion-commandes
echo "Strcuture de la gestion des commandes " > orders.txt
git add .
git commit -m "Ajout de la structure de gestion des commandes"
echo "Ajout de la fonctionnalité d'ajout de commande " >> orders.txt
git commit -am "Ajout de la fonctionnalité d'ajout de commande"
git push 
```

4. Fusion des branches feature dans develop
```bash
git checkout develop
git merge feature/gestion-utilisateurs -m "Fusion de la branche gestion-utilisateurs dans develop"
git push origin develop

git merge feature/catalogue-produits -m "Fusion de la branche catalogue-produits dans develop"
git push origin develop

git merge feature/gestion-commandes -m "Fusion de la branche gestion-commandes dans develop"
git push origin develop
```

5. Préparation de la branche release

```bash
git checkout develop
git checkout -b release/v1.0.0
git push origin release/v1.0.0

git checkout master
git merge release/v1.0.0 -m "Fusion de la release v1.0.0 dans master"
git push origin master

git tag -a v1.0.0 -m "Version 1.0.0 - Première version stable"
git push origin v1.0.0
```

6. Bug critique

```bash
git checkout master
git checkout -b hotfix/critique-affichage

echo "Correction d'un bug d'affichage" > affichage.txt
git add .
git commit -m "Correction du bug critique d'affichge"
git push origin hotfix/critique-affichage

git checkout master
git merge hotfix/critique-affichage -m "Fusion du hotfix/critique-affichage dans master"
git push origin master

git checkout develop
git merge hotfix/critique-affichage -m "Fusion du hotfix/critique-affichage dans develop"
git push origin develop
```