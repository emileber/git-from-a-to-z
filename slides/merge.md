## Les stratégies de fusion (merge)

Dépendants des objectifs et situation.

```text
A <- B         [master]
^
 \
  C <- D       [feature]
```

---

## Merge commit

Crée un nouveau commit qui a comme parent `master` et `feature`.

```bash
git checkout master
git merge feature
```

```text
A <- B <- E    [master]
^         ^
 \       /
  C <- D       [feature]
```

_Historique 100% intact_

---

## Rebase merging

Prend tous les commits de `feature` et les applique par dessus `master`.

```bash
git checkout feature
git rebase master
```

```text
A <- B <- C <- D    [master | feature]      
```

_Garde l'historique, mais recrée les commits._

---

![merge vs rebase](resources/git-merge-and-rebase.png)

---

## Squash merging

Crée un nouveau commit (E) qui contient tous les commits de la branch `feature`.

```bash
git checkout master
git merge --squash feature
git commit
```

```text
A <- B <- E (C+D)  [master]
^         
 \       
  C <- D           [feature]
```

_Perd l'historique de `feature`, mais très concis comme historique partagé._
