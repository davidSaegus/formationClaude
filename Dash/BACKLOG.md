# BACKLOG.md — les idées, triées

Une ligne par idée, avec son critère de réussite : on doit pouvoir dire « c'est fait »
en regardant la page, sans lire le code. Une seule idée à la fois.

## En cours
- (rien)

## Priorité 1 — l'effet immédiat

- [ ] **B2 · Mettre les retards en évidence**
  Plus de 10 jours en rouge, de 5 à 10 en orange, en dessous en gris.
  *Fini quand :* Pylône Nord-12 ressort en rouge, Pylône Sud-08 reste discret.

- [ ] **B3 · Trier par retard décroissant**
  *Fini quand :* la première ligne du tableau est la plus en retard, sans avoir à chercher.

## Priorité 2 — rendre la page interactive

- [ ] **B5 · Filtre par type, cumulable avec la région**
  *Fini quand :* Bretagne + Préventif donne exactement 2 lignes.

- [ ] **B6 · Recherche libre sur le site ou le technicien**
  *Fini quand :* taper « benali » ne laisse que ses deux interventions.

- [ ] **B7 · Détail d'une intervention au clic**
  Un panneau à droite avec toutes les informations de la ligne.
  *Fini quand :* un clic ouvre le panneau, un deuxième clic ou Échap le referme.

## Priorité 3 — des données qui tiennent la route

- [ ] **B8 · Dates d'ouverture et d'échéance, retard calculé**
  Le retard n'est plus écrit en dur : il se déduit de l'échéance et de la date du jour.
  *Fini quand :* changer une échéance change le retard affiché.

- [ ] **B9 · Passer à 40 interventions fictives sur 7 régions**
  *Fini quand :* le tableau se remplit et les filtres restent lisibles.

- [ ] **B10 · Compteur « X interventions affichées sur Y »**
  *Fini quand :* le compteur suit les filtres.

## Priorité 4 — présentation

- [ ] **B11 · Habillage aux couleurs TDF**
  Corail #FF401B en accent, en-tête sobre, typographie lisible en projection.
  *Fini quand :* la page est présentable en comité sans commentaire.

- [ ] **B12 · Version mobile pour le technicien**
  Sous 700 px, une carte par intervention plutôt qu'un tableau.
  *Fini quand :* la page reste lisible en réduisant la fenêtre.

- [ ] **B13 · Mode comité**
  Un bouton qui masque les filtres et agrandit les indicateurs.
  *Fini quand :* un clic suffit pour passer en mode projection.

- [ ] **B14 · Export de la sélection courante en CSV**
  *Fini quand :* le fichier téléchargé contient exactement les lignes affichées.

## Idées à trier (pas encore arbitrées)

- Évolution sur 12 semaines, préventif contre correctif
- Regroupement par technicien, avec la charge de chacun
- Carte de France cliquable à la place du menu régions
- Impression propre sur une page A4

## Fait

- [x] Page de départ : tableau brut des interventions, produite avec Claude Design
- [x] **B1 · Les 4 indicateurs en haut de page**
- [x] **B4 · Filtre par région**
