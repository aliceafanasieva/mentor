# Mentor

Begeleid en assisteer eerstejaars in jaar 1. 
De instructie vind je in: [INSTRUCTIONS](https://github.com/fdnd-task/mentor/blob/main/docs/INSTRUCTIONS.md)



## 1-10-2025

Vandaag in de les heb ik Kate en Khouloud begeleidt.

### Voorbereiding

In de les van eerstejaars: workshop Breakpoints & Media queries, inloop 9:00, start 9:30 (les gegeven door Krijn).

**Responsive design** - past de layout aan op basis van beschikbare ruimte.

**Breakpoint** = punt waarop de layout/styles veranderen.

**Mobile-first** - start met basisstijl voor kleinste view en voeg stijlen toe met min-width (aanrader).

**Desktop-first** - begin groot en schakel uit met max-width (minder schaalbaar).

### Media query syntaxis

```
/* Mobile-first */
@media (min-width: 48rem) /* ~768px als 1rem = 16px */

/* Desktop-first */
@media (max-width: 48rem) {}

/* Range */
@media (width >= 48rem) and (width < 64rem) /* “tussen 48rem en 64rem” */

```

### Veelgebruikte media features

- width / height (van viewport)

- orientation: portrait | landscape

- hover / pointer: detecteer muis/aanraakprecisie

- prefers-reduced-motion: respecteer animatievoorkeuren van de gebruiker

- prefers-color-scheme: dark/light colorscheme (gebruikersinstellingen)

### Mobile-first voorbeeld

```
.card-grid { display: grid; grid-template-columns: 1fr; gap: 1rem; }

@media (min-width: 48rem) {
  .card-grid { grid-template-columns: 1fr 1fr; }
}

@media (width >= 64rem) {
  .card-grid { grid-template-columns: repeat(3, 1fr); }
}
```

### Gebruiken van clamp() voor typografie

```
:root {
  /* schaal tussen 16px en 20px afhankelijk van viewport */
  font-size: clamp(1rem, 0.9rem + 0.5vw, 1.25rem);
}
h1 { font-size: clamp(1.75rem, 1.2rem + 2vw, 3rem); }
```


### Toegankelijkheid

```
@media (prefers-reduced-motion: reduce) {
  * { animation: none; transition: none; }
}
@media (prefers-color-scheme: dark) {
  :root { color-scheme: dark; }
  body { background: #111; color: #eee; }
}
```


### Werkcollege notities

1. Breakpoints

Basisregels:

1. Een _minimale_ grootte van 16px.
2. Een _optimale_ regellengte van 10-12 woorden.
3. Een regelafstand van 1.4

Opdracht 

**Vuistregels mediaqueries:**
1. We gebruiken het Mobile First principe, te zien aan de min-width media query.
2. We gebruiken CSS Nesting voor media queries, waardoor we de body selector niet hoeven te herhalen.

### Issues

Ik heb aan Khouloud tip gegeven in vorm van issue, dat ging over de opdrachtgever website. 

<img width="703" height="522" alt="image" src="https://github.com/user-attachments/assets/13c79fb2-b820-4b4c-950d-4166a1a53635" />


## 8-10-2025


