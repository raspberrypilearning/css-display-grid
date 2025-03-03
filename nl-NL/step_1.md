Om een nauwkeurigere indeling van jouw webpagina te maken, kun je een raster gebruiken!

### Creëer een class (klasse)

Maak een klasse aan binnen je `style.css` bestand - het is het beste om hier een **class** of **id** voor te gebruiken. Als je een tag opmaakt, wordt elke versie van die tag op je pagina een raster.

Stel de eigenschap `display` in op `grid`.

Stel een `height` (hoogte) in. Je kunt hiervoor `vh` gebruiken of een `px`-waarde instellen.

Definieer je **rijen** (de eigenschap `grid-template-rows`) en **kolommen** (de eigenschap `grid-template-columns`).

Je kunt de grootte van jouw rijen op een van de volgende manieren instellen:

- Percentages – je kunt de rijen en kolommen instellen als een `%` van de breedte of hoogte
- Delen - je kunt ze instellen als 'fr' van de breedte of hoogte
- Pixels - je kunt de hoogte instellen als een directe 'px' waarde

Hier zijn enkele voorbeelden:

## --- code ---

language: css
filename: style.css
---------------------------------------------------

// Een klasse
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

// Een ID
\#homepage-grid {
display: grid;
height: 80vh;
grid-template-rows: 2fr 1fr 1fr;
grid-template-columns: 1fr 1fr;
}

\--- /code ---

### Voeg het raster toe aan je HTML

Zodra je je selector hebt gemaakt, voeg je je klasse of id toe aan een **HTML** element.

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
