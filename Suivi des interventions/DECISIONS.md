# DECISIONS.md — les choix arrêtés

Une entrée par choix. Format : date · le choix · la raison · ce qu'on a écarté.

## 2026-09-18 · Un seul fichier index.html
Raison : on doit pouvoir l'ouvrir d'un double-clic et l'envoyer par mail.
Écarté : un projet avec plusieurs fichiers et un outil de build — trop lourd pour un prototype.

## 2026-09-18 · Données fictives écrites dans le fichier
Raison : aucune donnée réelle dans l'atelier, et rien à installer.
Écarté : lire un CSV — à reconsidérer si le prototype est repris.

## 2026-09-21 · Ajout de `statut` et `delaiResolutionHeures` au modèle de données
Raison : les indicateurs « délai moyen » et « résolues sous 48h » exigent de savoir
si une intervention est résolue et en combien de temps ; le modèle initial (site,
région, type, technicien, retard) ne le permettait pas.
Écarté : ajouter des dates d'ouverture/résolution plutôt qu'un délai en heures —
plus proche d'un vrai système, mais inutile pour un prototype qui n'affiche que
des agrégats.
