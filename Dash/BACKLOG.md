# BACKLOG.md — tableau de bord « Interventions terrain »

Une ligne = une demande métier. Chaque item porte **la phrase à taper** dans Claude Code
et **son critère de réussite visible** : on valide en regardant l'écran, jamais en lisant le code.

Règle du jeu : un seul item à la fois, le plan d'abord, le résultat ensuite.

---

## En cours
- (rien)

---

## Priorité 1 — rendre le tableau de bord lisible en 10 secondes

---

## Priorité 2 — répondre aux questions du responsable d'exploitation

### B3 · Charge par technicien
> « Ajoute un bloc « Charge par technicien » sous la charge par région : une barre par
> technicien, avec le nombre d'interventions en cours et le nombre hors engagement. »

**Fini quand :** on voit d'un coup d'œil qui est le plus chargé, et les barres suivent les filtres.

### B4 · Replanifier une intervention
> « Rends le bouton Replanifier actif dans le panneau de détail : il décale l'échéance de
> 7 jours, recalcule le retard, referme le panneau, affiche une confirmation et met à jour
> tout l'écran. »

**Fini quand :** après replanification de Pylône Nord-12, l'alerte passe de 2 à 1, le retard
moyen de 6,5 à 5,9 jours, et la ligne sort du haut du tableau.

---

## Priorité 3 — si le temps le permet

### B5 · Filtre par période
> « Ajoute un filtre Période : 7 derniers jours, 30 derniers jours, tout. »

**Fini quand :** le filtre se combine avec les autres, et tout l'écran suit.

### B6 · Vue comité
> « Ajoute un bouton « Vue comité » qui masque les filtres, agrandit les indicateurs et
> ne garde que les cinq interventions les plus en retard. »

**Fini quand :** un clic suffit pour projeter l'écran en réunion.

### B7 · Export de la sélection
> « Ajoute un bouton qui exporte en CSV exactement les lignes affichées. »

**Fini quand :** le fichier téléchargé correspond aux filtres en cours.

### B8 · Motifs de retard
> « Ajoute un petit classement des motifs de retard les plus fréquents sur la sélection
> courante. »

**Fini quand :** on peut dire quelle cause pèse le plus, et ça change avec les filtres.

### B9 · Vue mobile du technicien
> « Sous 700 pixels de large, remplace le tableau par une carte par intervention. »

**Fini quand :** la page reste lisible en réduisant la fenêtre.

---

## Idées à trier (déposées, pas arbitrées)

- Évolution sur 12 semaines, préventif contre correctif
- Carte de France cliquable à la place du menu des régions
- Historique des replanifications par intervention
- Impression propre sur une page A4
- Jeu de 40 interventions au lieu de 12

---

## Fait

- [x] **Maquette initiale** — tableau de bord produit avec Claude Design, exporté en HTML
- [x] **B0 · Reprendre la maquette dans un fichier propre** — `index.html` réécrit à la main
  (297 lignes), même mise en page, mêmes couleurs, mêmes données (15 interventions, 7 régions),
  filtres et panneau de détail fonctionnels
- [x] **B1 · Quatre indicateurs en tête de page** — ouvertes, en retard (>7j), retard moyen,
  part de correctif, recalculés sur les lignes filtrées (piège corrigé, voir `LESSONS.md`)
- [x] **B2 · Alerte engagement contractuel** — bandeau + colonne Engagement (Hors SLA/À
  risque/Dans les temps), seuils 10j / 7-10j documentés dans `DECISIONS.md`
