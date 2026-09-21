# LESSONS.md — les erreurs devenues des règles

Une entrée par erreur rencontrée. Format : le symptôme · la cause · la règle à retenir.

## Exemple (à remplacer par les vôtres)
- **Symptôme** : le compteur « en retard » ne changeait pas quand on filtrait par région.
- **Cause** : les indicateurs étaient calculés une seule fois au chargement de la page.
- **Règle** : tout indicateur se recalcule à partir des données filtrées, jamais des données brutes.

## B1 · Les indicateurs de la maquette ne recalculaient pas vraiment
- **Symptôme** : filtrer par région changeait bien les 4 chiffres en tête de page, mais
  vers des valeurs qui ne correspondaient à aucun calcul sur les lignes affichées.
- **Cause** : la maquette d'origine (B0) utilisait une approximation par région
  (`part` de la région × un total global) et deux valeurs codées en dur par région
  (délai moyen, résolution < 48h) — pas un agrégat sur les interventions filtrées.
- **Règle** : un indicateur se calcule sur la liste déjà filtrée (région + type), avant
  toute troncature d'affichage (ex. le top 10 du tableau) — jamais sur un total global
  mis à l'échelle, et jamais sur une valeur pré-écrite par cas.
