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

---

## init

Crée ou réinitialise un dépôt à l'intérieur d'un dossier.

```shell
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

---

## commit

![git commit comic](resources/git_commit_message_comic.png)

---

## checkout

```shell
# Déplacer HEAD
git checkout [branch | commit_hash]

# Annuler un changement sur un fichier ou un répertoire
git checkout -- directory/
```

---

## diff

```shell
# Voir les différences avec le dernier commit
git diff HEAD

# Différences avec les fichiers dans la "staging area"
git diff --staged
```

---

## log

---

## push

---

## pull

---

## remote

---

## reset

```shell
# Retirer un fichier de l'index
git reset fichier.ext
```

---

## rm

Supprime les fichiers ou répertoires et ajoute les suppressions à l'index.

```shell
git rm "*.txt"

# Supprimer un répertoire
git rm -r dossier/
```

Équivalent de `rm`, mais 

---

## stash
