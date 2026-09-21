# DECISIONS.md — les choix arrêtés

Une entrée par choix. Format : date · le choix · la raison · ce qu'on a écarté.

## 2026-09-18 · Un seul fichier index.html
Raison : on doit pouvoir l'ouvrir d'un double-clic et l'envoyer par mail.
Écarté : un projet avec plusieurs fichiers et un outil de build — trop lourd pour un prototype.

## 2026-09-18 · Données fictives écrites dans le fichier
Raison : aucune donnée réelle dans l'atelier, et rien à installer.
Écarté : lire un CSV — à reconsidérer si le prototype est repris.

## 2026-09-21 · B0 : reprise fidèle de la maquette, y compris ses approximations
Raison : la maquette calcule certains indicateurs (délai moyen, résolution < 48h) par
des valeurs fictives codées en dur par région, pas par un vrai agrégat sur les lignes
affichées. B0 demandait « même mise en page, mêmes couleurs, mêmes données » — donc ces
raccourcis ont été repris tels quels plutôt que corrigés.
Écarté : recalculer proprement ces indicateurs dès B0 — reporté à B1, qui porte
explicitement ce risque (« les indicateurs restent souvent figés »).

## 2026-09-21 · B2 : seuils de l'engagement contractuel
Raison : le backlog fixe le SLA à 10 jours après échéance, mais ne précise pas le seuil
« à risque », et son exemple (« Pylône Nord-12 », « 2 interventions hors engagement »)
correspond à un autre jeu de données que le nôtre. Seuils retenus, validés par
l'utilisateur : Hors SLA si retard > 10 j, À risque si 7-10 j, Dans les temps sinon —
cohérent avec le seuil « en retard » déjà utilisé par B1 (> 7 j). Sur nos données réelles,
cela donne 4 interventions hors engagement, pas 2.
Écarté : caler le seuil pour retomber sur « 2 » comme le backlog — aurait inventé un
chiffre sans rapport avec la règle énoncée (10 jours).

## 2026-09-21 · Gabarit HTML compact pour tenir sous 300 lignes
Raison : le critère de B0 impose moins de 300 lignes lisibles ; certains blocs répétitifs
(faits du panneau de détail, historique, légendes) sont générés par une boucle sur un
tableau de paires plutôt qu'écrits ligne par ligne.
Écarté : garder une balise HTML explicite par élément — plus lisible ligne à ligne, mais
dépassait largement les 300 lignes pour ce niveau de détail visuel.
