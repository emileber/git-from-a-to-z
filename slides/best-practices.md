## Les bonnes pratiques de Git

> Commit Often, Perfect Later, Publish Once

---

## Commits fréquents

- Un commit ne coûte rien
- Clarifie l'évolution dans l'historique
- Évite de perdre trop en cas de problème

---

## Message pertinents

Le message du commit doit:

- Décrire ce que le commit ajoute au projet, en terme de feature
- Moins de 80 caractères
- Doit éviter de lister les changements (Git le fait déjà)

```text
* "Adds password reset feature"
* "Fixes flickering on startup"
```

---

## Tenez vous à jour

Avant de commencer à travailler, `git fetch` ou `git pull`

---

## Éviter de changer l'historique partagé

Une fois partagé, un changement à l'historique peut causer des conflits.

Préférez un _revert commit_.

---

## Respectez l'espace de travail de chacun

- Éviter de faire des changements dans la branche de quelqu'un d'autre
- Préférez copier certains changements dans votre branche
- Contribué dans une branche commune (`master`, `develop`, etc.)

---

## Plusieurs projets, plusieurs dépôts

Exemple:
- Le backend dans un dépôt, 
- le frontend dans un autre, 
- les utilitaires dans un dépôt partagé (public même)

_Dépendants des limitations de la technologie du projet._

---

## Gardez le dépôt propre

- Supprimez les vieilles branches
- Faites des rebases (lorsque non-partagé)

---

## Choisissez un standard

Et forcez son application dans l'équipe.

---

## Protégez les branches communes

Il est possible de protéger des branches communes.

Ça évite de commiter par erreur dans celles-ci sans validation au préalable.

---

## Code review

Profitez des outils disponibles pour faire une révision du code avant de l'intégrer dans les branches partagées.

---

## Évitez les fichiers générés

Tout ce qui est généré ou dépendant de l'environnement locale à chacun devrait être ignoré.
