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

---

## status

---

## add

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

