#  Git Learning – Exercices 1, 2 et 3

Ce dépôt contient trois exercices pratiques pour apprendre Git et GitHub entièrement via le **terminal** :  
création de branches, commits, merges, gestion des conflits et pull requests.

---

##  Exercice 1 – Création du projet et premières commandes Git

###  Objectif
Découvrir les bases : initialisation du projet, commits, création de branche et fusion.

###  Commandes utilisées

- `git init`  
  Initialise un nouveau dépôt Git dans le dossier courant.

- `git status`  
  Affiche l’état des fichiers : modifiés, ajoutés, non suivis…

- `git add .`  
  Ajoute tous les fichiers modifiés dans la zone de préparation (stage).

- `git commit -m "message"`  
  Enregistre officiellement les changements dans l’historique Git.

- `git branch nom_branche`  
  Crée une nouvelle branche.

- `git checkout nom_branche`  
  Permet de changer de branche.

- `git merge nom_branche`  
  Fusionne une autre branche dans celle où l’on se trouve.

###  Résultat de l’exercice
- Création du dossier `learning1`
- Ajout d’un fichier (ex: `notes.txt`)
- Création de la branche `develop`
- Travail dans `develop`
- Fusion des modifications dans `main`

---
## Exercice 2 – Travail sur plusieurs branches sans conflit

### Objectif
Comprendre comment plusieurs branches peuvent travailler en parallèle sans provoquer de conflits.

###  Commandes utilisées

- `git branch`  
  Liste les branches existantes.

- `git switch nom` / `git checkout nom`  
  Change de branche.

- `git log --oneline --graph`  
  Affiche l’historique sous forme graphique.

- `git merge`  
  Fusionne deux branches.

### Résultat de l’exercice
- Création du dossier `learning2`
- Création de deux branches : `featureA` et `featureB`
- Modification du même fichier mais dans des **zones différentes**
- Fusion dans `main` **sans conflit**

---

##  Exercice 3 – Gestion des conflits lors du merge

###  Objectif
Provoquer et résoudre un conflit Git.

###  Quand un conflit apparaît ?
Lorsqu'une **même ligne** d’un fichier est modifiée différemment dans deux branches.

### Exemple de conflit affiché par Git :

```text
<<<<<<< HEAD
ligne dans la branche actuelle
=======
ligne dans l’autre branche
>>>>>>> feature
