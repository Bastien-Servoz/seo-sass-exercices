# Journal de bord

## Jour 1

- Date : 21/09/2026
- Ce que j'ai fait : création du dépôt, README, GitHub Pages, exercice-01 en ligne
- Ce qui m'a bloqué : Mauvaise configuration de la clé SSH, j'ai du la supprimer et en refaire une pour faire en sorte que tout fonctionne correctement. Ce que j'ai appris : vérifier avec ssh -T git@github.com que la clé fonctionne avant de cloner ».
- Objectif de la prochaine session : lancer le premier cours de From Scratch

## Jour 2

- Date : 22/09/2026
- Mise en place de la structure `td-html/` pour ranger les TD du cours HTML, un sous-dossier par TD (`td-01/`, `td-02/`, `td-03/`).
- TD 1 : tableau HTML complexe avec fusions de cellules (colspan/rowspan).
- Petite galère de manipulation : le dossier `td-html/td-01/` avait été créé par erreur à l'intérieur de `exercice-01/` au lieu de la racine du dépôt. Corrigé en déplaçant le dossier et en committant le changement.
- Mise à jour du sommaire dans le README avec le lien vers le TD 1.

— TD 2 : structure d'une maquette de site

- Créé `td-html/td-02/index.html`
- Travail sur l'architecture HTML d'une page : organisation en blocs `<div>` avec des classes,
  pensés pour faciliter le stylage CSS à venir
- Vérifié localement (file:///), affichage conforme

— TD 3 : intégration d'une maquette professionnelle

- Créé `td-html/td-03/index.html`
- Intégration d'une maquette plus poussée que le TD 2 : plus de contenu, d'images et de liens
- Vérifié localement (file:///), affichage conforme
- Ajout du dossier `td-html/td-correction/` pour y déposer les corrections du formateur
- Ajout de la correction du TD 3 dans `td-html/td-correction/`

## Jour 3

- Date : 23/09/2026
  Cours CSS (partie 1/2)

- Début du nouveau point de cours, dispensé en 2 parties, dédié au CSS
- Terminé la première partie du cours
- Installation et configuration des extensions/plugins indispensables pour la suite :
  - Extensions VS Code
  - Extensions Chrome

  ### Notions CSS vues aujourd'hui

- **Polices** : import de police externe via `@import url(...)` (Google Fonts) et déclaration de police locale avec `@font-face`
- **Texte** : `text-transform`, `letter-spacing`, `text-align`, tailles en `rem`, `text-shadow`, `font-family`
- **Boîtes** : centrage avec `margin: 0 auto`, bordures (`border`, `border-radius`), ombre de boîte (`box-shadow`), fond en `rgba`
- **Flexbox** : répartition équitable des éléments (`justify-content: space-around`), centrage vertical/horizontal (`justify-content` + `align-items`)
- **Grid** : mise en page en colonnes (`grid-template-columns`), et grille nommée avec `grid-template-areas` (ex : formulaire avec zones `i1`, `i2`, `ta`, `vi`, `bt`)
- **Positionnement** : `position: relative` sur le parent pour contenir un enfant en `position: absolute`, usage de `top`, `right`, `left`, `transform: translateX(-50%)` pour centrer un élément positionné
- **Interactivité** : `cursor: pointer`, `transition`, effet `:hover`
- **Responsive** : media queries (`@media screen and (max-width: ...)`) pour adapter la mise en page (grid → block, flex-direction en colonne) selon la largeur d'écran

- Prochaine étape : partie 2 du cours CSS

## Jour 4

- 24/09/2026
  Cours CSS (partie 2/2)

- Suivi du cours en live, code réalisé en parallèle du formateur avec personnalisation
- À partir de maintenant : intégration des notions en codant en même temps que le cours, sans TP après coup

### Notions CSS vues aujourd'hui

- **Variables CSS** : déclaration de couleurs réutilisables avec `:root` et `var(--nom)`
- **Reset global** : `* { margin: 0; padding: 0; box-sizing: border-box; }`
- **Pseudo-éléments** : `::before` et `::after` pour insérer du contenu décoratif (icône, soulignement animé, texte superposé)
- **Animations** : `@keyframes` et `animation` pour des effets progressifs (ligne qui se dessine, élément qui flotte façon "cheese")
- **Grid** : mise en page en colonnes avec `grid-template-columns`, alignement d'un élément avec `place-self`
- **Formes personnalisées** : `clip-path: polygon(...)` pour créer un losange, `linear-gradient` en fond
- **Effets visuels** : `filter: drop-shadow(...)`, `backdrop-filter: blur(...)` pour flouter l'arrière-plan d'une carte
- **Troncature de texte** : `-webkit-line-clamp` pour limiter un paragraphe à un nombre de lignes avec `...`
- **Personnalisation de sélection** : `::selection` pour changer la couleur du texte sélectionné
- **Checkbox stylisée** : technique `input[type="checkbox"]:checked + label` pour transformer une case à cocher en bouton cliquable stylisé
- **Perspective / 3D** : `perspective` sur le parent + `translateZ` sur l'enfant pour un effet de profondeur au survol
- **Champs de formulaire** : `:focus`, `::placeholder`, transitions sur les bordures
- **Pseudo-classes d'interaction** : `:hover`, `:active`, `:visited`, et combo `button:hover + a` pour afficher un élément au survol d'un autre
- **Visibilité animée** : combinaison `opacity`, `visibility`, `transform: translateY(...)` et `transition` pour une apparition en douceur

- Prochaine étape : Apprentissage GITHUB

## Jour 5

- 25/09/2026
  Cours GitHub

Cours théorique (2x40 min) sur la mise en place de GitHub et les commandes essentielles pour alimenter un dépôt (init, add, commit, push, status, etc.).
Suivi en visionnage, pas de TP associé
Prochain cours : SEO

## Jour 6

-26/09/2026
Cours SEO

### Règles SEO à retenir

**1. Créer du bon contenu**

- 400 mots minimum par page
- Contenu à jour, non répétitif
- Éviter les pages d'intro avant le site
- Éviter les liens type "cliquez ici" / "en savoir plus"
- Privilégier le local (ville, région, quartier) — le robot favorise le contenu local ; utiliser `.fr` si le site cible uniquement la France

**2. HTML "SEO friendly"**

- Voir projet `html-helium`
- Open Graph : https://ogp.me/
- Test Open Graph : https://cards-dev.x.com

**3. Site rapide (performant)**

- Le robot teste le temps de chargement
- Le JS doit être lu en dernier
- Faire apparaître une couleur de fond le plus vite possible
- Privilégier les images depuis le CSS plutôt que la balise `<img>`

**Outils**

- Test SEO : plugin Lighthouse
- Doc officielle : https://developers.google.com/search/docs?hl=fr

### Exercice pratique — `html-helium`

Mise en pratique des principes SEO/perf sur une page (nav, header responsive, section infos/investisseurs), avec media queries pour mobile et tablette

## Jour 7

-27/09/2026
Cours SASS

Introduction à Sass, préprocesseur CSS pour un code plus structuré et maintenable.

- **Organisation** : découpage en plusieurs fichiers `.scss` (variables, mixins, composants...) assemblés via `@import`, pour éviter un fichier CSS monolithique
- **Variables** : centralisation des valeurs réutilisées (couleurs, espacements) pour une maintenance simplifiée
- **Mixins** : blocs de styles réutilisables et paramétrables (`@mixin` / `@include`) pour factoriser les patterns récurrents

Approche plus modulaire, pensée en composants réutilisables plutôt qu'en styles isolés.
