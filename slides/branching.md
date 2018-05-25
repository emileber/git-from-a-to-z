## Les branches et étiquettes

Pour pouvoir travailler en parallèle

---

## Les branches

Nom symbolique représentant une ligne de développement.

Les nouveaux commits sont ajoutés dessus et le pointeur s'ajuste.

```bash
# Créer une branche
git branch ma_branche

# Créer et naviguer sur la branche
git checkout -b ma_nouvelle_branche

# Voir les branches
git branch

# Supprimer une branche
git branch -D ma_vieille_branche

# Supprimer une branche distante (le : avant le nom de la branche)
git push origin :ma_vieille_branche_distante
```

---

## Les étiquettes (tags)

Nom symbolique d'une révision spécifique.

Pointe toujours le même commit.

```text
x--x--x--x--x # une branche
    \ 
     --y----y # une autre branche
       1.1
        ^
        |
        # un tag qui pointe un commit
```

_Utile pour identifier une version._

---

## Les étiquettes légères

_Lightweight tags_

Seulement le nom du tag attaché sur un commit.

```bash
git tag v1.0.2
```

---

## Les étiquettes annotées

En plus du nom, possibilité d'inclure un commentaire et les informations de l'auteur de l'étiquette.

```bash
git tag -a v1.0.2 -m "[RELEASE] blah blah"
```
