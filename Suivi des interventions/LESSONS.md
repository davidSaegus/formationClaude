# LESSONS.md — les erreurs devenues des règles

Une entrée par erreur rencontrée. Format : le symptôme · la cause · la règle à retenir.

## Exemple (à remplacer par les vôtres)
- **Symptôme** : le compteur « en retard » ne changeait pas quand on filtrait par région.
- **Cause** : les indicateurs étaient calculés une seule fois au chargement de la page.
- **Règle** : tout indicateur se recalcule à partir des données filtrées, jamais des données brutes.
