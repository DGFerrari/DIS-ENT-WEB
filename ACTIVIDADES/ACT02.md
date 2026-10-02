# DAW.0615.DIS.INT.WEB.Act2

## Activitat 2: Landing Page Restaurant
### Estilització amb CSS

Has de crear la landing page d'un restaurant que necessita presència digital per captar nous clients. La pàgina ha de transmetre la identitat i l'essència del restaurant a través dels colors, tipografia i estil visual.

### Tipus de restaurants disponibles (trieu-ne un)

1. 🍕 Pizzeria artesanal italiana
   - Ambient: tradicional, familiar, càlid
   - Colors suggerits: vermells, verds, crema, marró
2. 🍣 Restaurant de sushi modern
   - Ambient: minimalista, elegant, zen
   - Colors suggerits: negre, blanc, vermell, daurats
3. 🍔 Hamburgueseria gourmet
   - Ambient: modern, urbà, desenfadat
   - Colors suggerits: vermells, negres, mostassa, marrons
4. 🌱 Restaurant vegetarià/vegà
   - Ambient: natural, fresc, saludable
   - Colors suggerits: verds, blancs, terracotes, beige
5. ☕ Cafeteria/brunch spot
   - Ambient: acollidor, hipster, relaxat
   - Colors suggerits: marrons, crema, rosa pastel, turquesa
6. 🌮 Taqueria mexicana
   - Ambient: vibrant, festiu, autèntic
   - Colors suggerits: taronja, vermell, verd, groc
7. 🥐 Pastisseria francesa
   - Ambient: elegant, dolç, romàntic
   - Colors suggerits: rosa, lila, daurats, blanc
8. 🍜 Restaurant de ramen
   - Ambient: modern, urbà, acollidor
   - Colors suggerits: vermell, negre, blanc, daurats

---

## Materials proporcionats

Se t'entregarà una carpeta base amb els següents fitxers:

```text
Act2_Restaurant_Base/
├── index.html          (Estructura HTML completa)
├── styles.css          (Fitxer buit per completar)
└── README.txt          (Instruccions ràpides)
```

### Contingut de l'index.html

El fitxer HTML ja conté l'estructura completa amb:

- Header amb navegació (logo + menú)
- Hero section (títol + subtítol + botó CTA)
- Secció "Sobre nosaltres"
- Destacats del menú (3 plats amb nom, descripció i preu)
- Formulari de reserva (nom, email, data, hora, persones)
- Footer amb informació de contacte

La teva feina és:

1. Personalitzar els textos amb el nom i informació del teu restaurant
2. Crear tot l'estil CSS al fitxer `styles.css`

> IMPORTANT: No modifiquis l'estructura HTML (etiquetes, classes, ids). Només canvia els textos/continguts.

---

## Tasques a realitzar

### Tasca 1: Configuració inicial i definició de la paleta

#### 1.1 Selecció de tipografia

1. Navega a Google Fonts
2. Tria 2 fonts que encaixin amb l'ambient del teu restaurant:
   - Font per títols: més display, bold, impactant
   - Font per text: llegible, clara, professional
3. Afegeix l'enllaç al `<head>` del teu HTML
4. Exemples per temàtiques:
   - Italiana: Playfair Display + Lato
   - Sushi: Noto Sans JP + Roboto
   - Hamburgueseria: Bebas Neue + Open Sans
   - Vegetariana: Quicksand + Nunito

#### 1.2 Definició de la paleta de colors

Utilitza eines per trobar colors harmònics:

- Coolors.co - Generador de paletes
- Adobe Color - Roda cromàtica
- Material Design Colors

Variables CSS OBLIGATÒRIES al CSS.

Consells per triar colors:

- Pensa en l'emoció que vols transmetre
- Mira restaurants reals similars per inspiració
- Assegura't que hi ha bon contrast text/fons
- Usa WebAIM Contrast Checker per verificar accessibilitat

### Tasca 2: Estils

- Generals del body i tipografia
- Navegació/Header
  - Logo destacat
  - Menú amb espaiat adequat
  - Efectes hover
  - Text contrastat
- Hero Section
  - Secció destacada amb fons
  - Text centrat
  - Botó cridaner (call-to-action)
  - Padding generós
- Botons
  - Color secundari per destacar
  - Padding adequat
  - Border radius
  - Hover amb efecte visual
  - Cursor pointer
- Secció "Sobre nosaltres"
- Cards de plats destacats
  - Cards amb background blanc o clar
  - Shadow suau
  - Border radius
  - Espaiat intern generós
  - Hover amb efecte
- Formulari de reserva
  - Background diferent per destacar
  - Inputs amb estil consistent
  - Labels clars
  - Focus state amb color d'accent
- Botó de submit destacat
- Footer
- Poliment final
  - Revisa que TOTS els colors usen variables CSS
    - Cerca `#` al teu CSS
    - Només hauria d'aparèixer dins del `:root`
  - Comprova el contrast de colors
    - Usa WebAIM Contrast Checker
  - Afegeix comentaris al CSS
  - Comprova tots els hover effects
  - Valida el teu HTML i CSS
    - W3C HTML Validator
    - W3C CSS Validator

---

## Crea una carpeta amb el següent contingut

```text
Cognom_Nom_Act2_CSS/
├── index.html
├── styles.css
└── document_reflexiu.pdf
```

## Document reflexiu (1-2 pàgines)

Ha d'incloure:

1. Informació del restaurant:
   - Nom del restaurant
   - Tipus de cuina
   - Ambient/personalitat
2. Justificació de la paleta de colors:
   - Captura de la paleta (Coolors, Adobe Color...)
   - Per què has triat aquests colors?
   - Què vols transmetre amb ells?
   - Enllaç a la paleta generada
3. Justificació de les fonts:
   - Quines fonts has triat i per què?
   - Com encaixen amb l'ambient del restaurant?
4. Accessibilitat:
   - Captures
   - Resultats dels tests de contrast
5. Validació HTML i CSS:
   - Captures
   - Resultats dels tests
6. Captures de pantalla:
   - Vista completa de la landing (scroll complet)
   - Detalls de seccions importants (hero, cards, formulari)
7. Reflexió personal:
   - Dificultats trobades i com les has resolt
   - Què has après sobre variables CSS?
   - Recursos consultats (enllaços)

---

## Format de lliurament

- Carpeta comprimida (`.zip`): `Cognom_Nom_Act2_CSS.zip`
