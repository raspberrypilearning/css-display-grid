Pour réaliser une mise en page plus précise sur ta page web, tu peux utiliser une grille !

### Créer une classe

Crée une classe dans ton fichier `style.css` : il est préférable d'utiliser une **classe** ou un **id** pour cela. Si tu stylises une balise, chaque version de cette balise sur ta page sera une grille.

Définis la propriété `display` sur `grid`.

Définir un `height` (hauteur). Tu peux utiliser `vh` pour cela, ou définir une valeur `px`.

Définis tes **lignes** (la propriété `grid-template-rows`) et **colonnes** (le `grid-template-columns`).

Tu peux définir la taille de tes lignes de l'une de ces manières :

- Pourcentages : tu peux définir les lignes et les colonnes comme un `%` de la largeur ou de la hauteur
- Fractions : tu peux les définir comme un `fr` de la largeur ou de la hauteur
- Pixels : tu peux définir la hauteur comme une valeur `px` directe

Voici quelques exemples :

## --- code ---

language: css
filename: style.css
---------------------------------------------------

// Une classe
.fact-holder {
display: grid;
height: 50vh;
grid-template-rows: 50% 50%;
grid-template-columns: 50% 50%;
}

\--- /code ---

## --- code ---

language: css
filename: style.css
---------------------------------------------------

// Un ID
\#homepage-grid {
display: grid;
height: 80vh;
grid-template-rows: 2fr 1fr 1fr;
grid-template-columns: 1fr 1fr;
}

\--- /code ---

### Ajouter la grille à ton HTML

Une fois ton sélecteur créé, ajoute ta classe ou ton ID à un élément **HTML**.

## --- code ---

## language: html

<section class="fact-holder">

</section>

\--- /code ---

## --- code ---

## language: html

<div id="homepage-grid">

</div>

\--- /code ---
