# ETAT.md — où on en est

*Dernière mise à jour : 2026-09-21*

## Ce qui marche
- **B0 fait** : `index.html` (~300 lignes) reprend à la main la maquette Claude Design
  (dont l'export d'origine était illisible — bundle JS compressé). En-tête, filtres
  (région, type d'équipement, période), charge par région, graphique 12 semaines
  (préventif/correctif), tableau des 10 interventions les plus en retard, panneau de
  détail au clic. 15 interventions fictives sur 7 régions.
- **B1 fait** : les 4 indicateurs de tête (ouvertes, en retard > 7 j, retard moyen,
  part de correctif) se calculent sur les lignes réellement filtrées (région + type),
  avant la troncature à 10 lignes du tableau — vérifié en filtrant par région.
- **B2 fait** : bandeau d'alerte (« N interventions hors engagement ») et colonne
  Engagement dans le tableau (Hors SLA > 10j / À risque 7-10j / Dans les temps),
  recalculés sur les lignes filtrées. 4 interventions hors engagement au total.
- Filtres et panneau de détail fonctionnels (un seul écouteur par délégation, un seul
  `afficher()` qui reconstruit l'écran à chaque interaction).

## Ce qui ne marche pas encore
- Pas encore de charge par technicien (B3), ni de replanification active (B4).
- Le graphique 12 semaines reste sur des séries fictives approximées par région
  (pas de vraies dates par semaine dans les données).

## En cours
- Rien.

## Prochaine étape
- **B3 — charge par technicien** (bloc de barres sous la charge par région).

## Pour reprendre, me redonner cette phrase
« Lis CLAUDE.md, ETAT.md et BACKLOG.md, puis résume-moi où on en est et ce qui est prioritaire. »
