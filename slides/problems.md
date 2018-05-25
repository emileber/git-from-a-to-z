## Réécrire l'histoire

Avec Git, c'est possible!

---

## Modifier un message de commit

```bash
git commit --amend
```

---

## Corriger un oubli

Une faute d'ortographe? Un fichier oublié?

```text
git rebase -i commit_hash

# Soyez très vigilant avec la commande suivante
git push --force
```

---

## Annuler complètement le travail

- Commit sur la mauvaise branche?
- Branches locale et distante différentes?

```bash
git reset --hard commit_ou_branche

# Soyez très vigilant avec la commande suivante
git push --force
```
