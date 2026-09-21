# ETAT.md — où on en est

*Dernière mise à jour : 2026-09-21*

## Ce qui marche
- `index.html` s'ouvre dans un navigateur et affiche le tableau des 5 interventions
  fictives : site, région, type, technicien, jours de retard.
- Les 4 indicateurs de tête (B1) : ouvertes, en retard (> 7 j), retard moyen,
  part de correctif — calculés par `calculerIndicateurs(liste)`.
- Le filtre par région (B4) : un menu déroulant (régions + « Toutes ») qui
  recalcule indicateurs et tableau ensemble via `actualiser()`.

## Ce qui ne marche pas encore
- Aucun tri, pas de mise en évidence visuelle des retards.

## En cours
- Rien.

## Prochaine étape
- B2 (mise en évidence des retards) ou B3 (tri décroissant).

## Pour reprendre, me redonner cette phrase
« Lis CLAUDE.md, ETAT.md et BACKLOG.md, puis résume-moi où on en est et ce qui est prioritaire. »
