## Les opérations de base


- Naviguer dans un dépôt
- Enregistrer ses changements
- Annuler des changements
- Voir l'historique de changements
- Partager ses changements
- etc.

---

## Exercice pratique

[**try.github.io**](https://try.github.io/levels/1/challenges/9)

Voir l'aide d'une commande git

```bash
git [command] --help
```

---

## init

Crée ou réinitialise un dépôt à l'intérieur d'un dossier.

```bash
# Créez un dossier et naviguez à l'intérieur
mkdir mon-projet && cd "$_"

# Nous sommes prêt à initialiser un nouveau dépôt git
git init
```

Un dossier `.git/` est créé à l'intérieur du répertoire du projet.

---

## status

Montre l'état de la zone de travail.

![git status](resources/status.png)

---

## add

Ajoute des _changements_ à la zone d'index

```bash
# Ajouter tous les changements
git add .

# Ajout intéractif
git add -i
```
Permet d'ajouter seulement des sections d'un fichier modifié

---

## commit

Enregistre les changements actuellement dans l'index

```bash
# Commit avec un message
git commit -m "Message du commit"
```

![git commit comic](resources/git_commit_message_comic.png)

---

## checkout

Changer de branche (bouger le `HEAD`)  
**ou** restaurer un fichier modifié

```bash
# Déplacer HEAD
git checkout [branch | commit_hash]

# Annuler un changement sur un fichier ou un répertoire
git checkout -- directory/
```

---

## diff

Voir les différences entre les zones et des commits

```bash
# Voir les différences avec le dernier commit
git diff HEAD

# Différences avec les fichiers dans la "staging area"
git diff --staged
```

---

## log

Affiche l'historique de commit

```bash
git log

# Voir un graphique plus complet et clair
git log --graph --oneline
```

![git graph oneline](resources/git-graph-oneline.png)

---

## push

---

## pull

---

## remote

---

## reset

```bash
# Retirer un fichier de l'index
git reset fichier.ext
```

---

## rm

Supprime les fichiers ou répertoires et ajoute les suppressions à l'index.

```bash
git rm "*.txt"

# Supprimer un répertoire
git rm -r dossier/
```

Équivalent de `rm`, mais 

---

## stash
