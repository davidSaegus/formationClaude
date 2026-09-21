# ETAT.md — où on en est

*Dernière mise à jour : 2026-09-21*

## Ce qui marche
- **B0 fait** : `index.html` (297 lignes) reprend à la main la maquette Claude Design
  (dont l'export d'origine était illisible — bundle JS compressé). En-tête, filtres
  (région, type d'équipement, période), 4 indicateurs, charge par région, graphique
  12 semaines (préventif/correctif), tableau des 10 interventions les plus en retard,
  panneau de détail au clic. 15 interventions fictives sur 7 régions.
- Filtres et panneau de détail fonctionnels (un seul écouteur par délégation, un seul
  `afficher()` qui reconstruit l'écran à chaque interaction).

## Ce qui ne marche pas encore
- Les indicateurs « délai moyen » et « résolution < 48h » sont des valeurs fictives
  codées en dur par région, pas de vrais agrégats sur les lignes affichées — piège
  identifié dans B1, à corriger.
- Pas encore d'alerte d'engagement contractuel (B2), de charge par technicien (B3),
  ni de replanification active (B4).

## En cours
- Rien.

## Prochaine étape
- **B1 — les 4 indicateurs en tête de page**, avec le piège connu à vérifier :
  choisir une région et s'assurer que les indicateurs se recalculent vraiment.

## Pour reprendre, me redonner cette phrase
« Lis CLAUDE.md, ETAT.md et BACKLOG.md, puis résume-moi où on en est et ce qui est prioritaire. »
