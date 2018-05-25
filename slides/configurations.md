## Configurations

Plusieurs fichiers de configuration Git

Local ou global

---

## Ignorer des fichiers

Le fichier `.gitignore` (local et global)

```text
node_modules
bower_components
dist
*.log
.sass-cache
/index.html
/css/theme.css

.idea
.DS_Store
```

Des fichier `.gitignore` pré-configuré pour des technos: https://gitignore.io/

---

## Paramètres

```bash
cat ~/.gitconfig
```

```text
[core]
	autocrlf = false
	eol = lf
[push]
	default = simple
```

---

## Alias

- Dans le `.gitconfig`
- équivaut à une nouvelle commande `git mon-alias`

```text
[alias]
    # list aliases
    la = !git config -l | grep alias | cut -c 7-
    branch-name = rev-parse --abbrev-ref HEAD
    cam = commit -am
    cm = commit -m
    pub = !git push -u origin $(git branch-name)
    unpub = !git push origin :$(git branch-name)
```

Tous mes alias personnels [github.com/emileber/dot-files](https://github.com/emileber/dot-files/blob/master/.gitconfig)

---

## Attributs

Modifier le comportement de git pour certains fichiers
