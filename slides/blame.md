## Trouver le coupable!

Pour mieux comprendre   
_...ou mieux punir!_

---

## blame

Pour trouver le dernier commit ayant modifié une ligne en particulier.

```bash
git blame slides/blame.md
```

```text
eb73a701 (Emile Bergeron    2018-05-23 23:29:25 -0400  1) ## Trouver le coupable!
eb73a701 (Emile Bergeron    2018-05-23 23:29:25 -0400  2)
eb73a701 (Emile Bergeron    2018-05-23 23:29:25 -0400  3) Pour mieux comprendre
eb73a701 (Emile Bergeron    2018-05-23 23:29:25 -0400  4) _...ou mieux punir!_
7842b9b8 (Emile Bergeron    2018-05-24 23:15:42 -0400  5)
```

---

## bisect

Pour retrouver le commit qui a brisé le projet.

```bash
git bisect start
git bisect bad
git bisect good HEAD~9
```

```text
Bisecting: 2 revisions left to test after this (roughly 2 steps)
[< ... sha ... >] 3
```
