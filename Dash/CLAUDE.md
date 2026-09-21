# CLAUDE.md — projet « Suivi des interventions » (prototype)

Prototype d'une page web de suivi des interventions de maintenance.
Données fictives, créées pour l'atelier. Aucune donnée réelle ici.

## Les fichiers du projet, et quand les lire

- `PRODUIT.md` — ce qu'on construit et pour qui. À lire si le besoin est flou.
- `BACKLOG.md` — les idées, triées. La source des tâches.
- `ETAT.md` — où on en est. **À lire en premier, à chaque session.**
- `DECISIONS.md` — les choix arrêtés et leur raison. À lire avant de proposer un choix technique.
- `LESSONS.md` — les erreurs déjà rencontrées. **À relire avant de modifier le code.**
- `index.html` — le prototype. Un seul fichier, HTML + CSS + JS à l'intérieur.

## Au début de chaque session

1. Lire `ETAT.md`, puis `BACKLOG.md`.
2. Résumer en 5 lignes : ce qui marche, ce qui est en cours, ce qui est prioritaire.
3. Attendre que je choisisse l'item à traiter.

## Pendant le travail

- Une seule fonctionnalité à la fois, prise dans le backlog.
- Toujours proposer le plan avant de modifier quoi que ce soit, et attendre mon accord.
- Ne jamais écraser un fichier sans le dire : annoncer ce qui change, et pourquoi.
- Le prototype reste dans un seul `index.html`, sans dépendance externe.
- Écrire en français : textes de l'interface, commentaires, et tout ce qui est écrit dans les `.md`.

## À la fin de chaque étape

- Une erreur rencontrée puis corrigée → une ligne dans `LESSONS.md` (le symptôme, la cause, la règle).
- Un choix qui engage la suite → une entrée datée dans `DECISIONS.md` (le choix, la raison, l'alternative écartée).
- Une idée qui surgit en chemin → une ligne dans `BACKLOG.md`, sans la traiter tout de suite.

## À la fin de la session

Mettre à jour `ETAT.md` : ce qui marche, ce qui est en cours, la prochaine étape,
et la phrase exacte à me redonner pour reprendre.

## Jamais

- Inventer un chiffre : si une donnée manque, écrire `[à compléter]`.
- Installer une bibliothèque ou un outil sans me demander.
- Traiter plusieurs items du backlog dans la même étape.
