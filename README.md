**Nom :** Antoine Caron, Luc Lecarpentier, Mathys Poret

**Groupe :** B

**Equipe :** 13

**Année :** 1ere année(2023)

**IUT Le Havre - Cours GIT**

# TP3

## 1-Inviter des collaborateurs dans un dépôt personnel

Pour cela on va dans les options du répertoire github et on va dans collaborateur et on ajoute le compte du collègue.
Les collaborateurs clonent le projet sur leur machine.

## 2-Développement d’un projet java en équipe

Lorsque l'un fait une modification et la push sur github, l'autre doit pull avant de pouvoir modifier le github.

## 3-Gérer des nouvelles fonctionnalités à l’aide des branches

### 3.1) Tester le concept de branche avec un exemple simple

```git checkout -b test``` permet de créer une branche puis de se déplacer sur cette branche. Sur cette branche on va faire des tests sans que cela impact la branche principale.

Sur cette branche, on va créer un fichier test (```touch test.txt```) puis on l'ajoute avec la procédure normale.

Si on retourne sur la branche principale avec ```git checkout main```. Sur cette branche, on ne retrouve aucune trace du test que l'on a effectué.

On fait ensuite une modification du README que lon ajoute à la branche principale. ```git log --graph --oneline --all --decorate --topo-order``` cette commande nous permet de voir l'état des modifications du répertoire git.
On peut observer que le test a été fait uniquement sur la branche dédié et que le test n'as pas eu de modification du README car les branches sont indépendantes. 

### 3.2) Fusionner la branche de test dans la branche principale

## Résumé

- ```git checkout``` : cette commande sert à gérer les branches d'un projet git soit en les créant soit en se déplaçant entre les branches.
- ```git merge``` : cette commande permet de fusionner des branches
