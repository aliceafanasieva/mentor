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

#### Opdracht

Ik ging ook meedoen met opdracht:

https://github.com/fdnd-task/the-client-website/blob/main/docs/breakpoints-en-media-queries.md#opdracht

Mijn code:

https://github.com/aliceafanasieva/i-love-web/blob/main/leesbare-teksten.html

Screenshots:

<img width="783" height="834" alt="image" src="https://github.com/user-attachments/assets/97b4269a-d357-4408-a42b-a74d209a94c4" />

<img width="783" height="834" alt="image" src="https://github.com/user-attachments/assets/e0f4a828-8c2b-4927-b3eb-43839a7aff1c" />

<img width="783" height="609" alt="image" src="https://github.com/user-attachments/assets/4359c320-80b3-41bd-a41e-07c023540945" />


### Issues

Ik heb aan Khouloud tip gegeven in vorm van issue, dat ging over de opdrachtgever website. 

<img width="703" height="522" alt="image" src="https://github.com/user-attachments/assets/13c79fb2-b820-4b4c-950d-4166a1a53635" />


## 8-10-2025

#### Planning

### Sprintreview en Readme voorbereiden voor donderdag

1. Wat wil je donderdag laten zien en wat is daar nog voor nodig?
2. Bereid de Sprint Review voor met studenten uit je squad, die dezelfde opdracht hebben
3. Maaak een nette proffessionele Readme

## 15-10-2025

### WCAG Audit feedback

Ik heb de presentaties over WCAG audit van eerstejaars studenten gereviewed en issues geschreven met tips en tops:

- Kurollos: [https://github.com/Kurollos/all-human-accessible-website/issues/10](https://github.com/Kurollos/all-human-accessible-website/issues/10#issuecomment-3405064442)

- Mathijs: [https://github.com/MathijsN/all-human-accessible-website/issues/9](https://github.com/MathijsN/all-human-accessible-website/issues/9#issuecomment-3405026724)

- Tom: [https://github.com/TZGaming/all-human-accessible-website/issues/11](https://github.com/TZGaming/all-human-accessible-website/issues/11#issuecomment-3405093988)

<img width="960" height="702" alt="image" src="https://github.com/user-attachments/assets/5177432a-4b9f-437d-9976-e62f2f7666cb" />

<img width="910" height="832" alt="image" src="https://github.com/user-attachments/assets/53a8547d-eb46-46cd-a957-10c4ae044a75" />

# 14-11-2025

### Code/design review Look and Feel - Styleguide

Vandaag ben ik mentor van groep eerstejaars bij project AD-Connect.

Samen met mijn groepje heb ik feedback gegeven aan de code van styleguide van [BCK](https://github.com/toasterbath0758/look-and-feel-styleguide-BCK/issues/9) en [EFM (Kate en Keileigh)](https://github.com/Kayleighhhhh/look-and-feel-styleguide/issues/8).

Ik heb ook zelfstandig code/design review geschreven in een issue voor het groepje EFM: https://github.com/Kurollos/look-and-feel-styleguide/issues/6

Ik heb aantal dingen geleerd van eerstejaars, zoals gebruik maken van Markdown [alerts](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#alerts) of css letterlijk citeren. 





