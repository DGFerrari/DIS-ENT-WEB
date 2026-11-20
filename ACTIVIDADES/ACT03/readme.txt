============================================================
ACTIVITAT 3: CARTA/MENÚ DIGITAL AMB FLEXBOX
============================================================

CONTINGUT D'AQUESTA CARPETA:
----------------------------
- menu.html: Estructura HTML completa de la carta digital
- styles.css: Fitxer CSS amb comentaris guia (a completar)
- README.txt: Aquest fitxer amb instruccions


OBJECTIU DE L'ACTIVITAT:
-------------------------
Crear una carta digital per al teu restaurant utilitzant Flexbox
per organitzar tots els layouts (navegació, filtres, grid de plats,
cards individuals, begudes i footer).


PASSOS A SEGUIR:
----------------

FASE 1: PREPARACIÓ 
  ✓ Obre menu.html i personalitza tots els textos [entre corxets]
  ✓ Afegeix els teus plats (mínim 3 per categoria)
  ✓ Afegeix preus realistes
  ✓ Canvia les begudes segons el teu restaurant
  ✓ Copia el link de Google Fonts de l'Act 2 al <head>

FASE 2: VARIABLES CSS 
  ✓ Obre el styles.css de l'Activitat 2
  ✓ Copia tot el bloc :root { ... } amb les teves variables
  ✓ Enganxa-les al styles.css de l'Act 3
  ✓ Verifica que els colors i fonts són correctes

FASE 3: IMPLEMENTACIÓ FLEXBOX 
  □ Tasca 2: Navegació amb Flexbox 
  □ Tasca 3: Hero amb Flexbox 
  □ Tasca 4: Filtres amb Flexbox 
  □ Tasca 5: Grid de plats amb Flexbox 
  □ Tasca 6: Cards internes amb Flexbox 
  □ Tasca 7: Begudes amb Flexbox
  □ Tasca 8: Footer amb Flexbox 

FASE 4: RESPONSIVE
  □ Tasca 9: Media queries per tablets i mòbils
  □ Prova amb DevTools en diferents mides
  □ Assegura't que tot funciona en 320px, 768px i 1920px

FASE 5: POLIMENT
  □ Tasca 10: Verifica que TOT usa Flexbox
  □ Comprova hover effects
  □ Valida HTML i CSS
  □ Afegeix comentaris finals


ESTRUCTURA HTML PROPORCIONADA:
-------------------------------
✓ Header amb navegació (logo + menu)
✓ Hero section (títol + subtítol)
✓ Filtres de categoria (botons)
✓ Secció Entrants (3 plats)
✓ Secció Principals (4 plats)
✓ Secció Postres (3 plats)
✓ Secció Begudes (5 begudes en layout horitzontal)
✓ Footer (info + xarxes socials)

Total: 10 plats + 5 begudes = 15 ítems


ELEMENTS HTML CLAU:
-------------------
Classes importants per estilitzar:
- nav, .logo, .nav-menu
- .hero
- .category-filters, .filters, .filter-btn
- .menu-section, .dishes-grid
- .dish-card, .dish-image, .dish-info
- .dish-header, .dish-name, .dish-price
- .dish-description, .dish-allergens
- .drinks-section, .drinks-list, .drink-card
- footer, .footer-content, .footer-info, .footer-social


PROPIETATS FLEXBOX CLAU:
-------------------------
Contenidors flex:
  display: flex
  justify-content: (space-between, center, flex-start...)
  align-items: (center, stretch, flex-start...)
  flex-direction: (row, column)
  flex-wrap: (wrap, nowrap)
  gap: (1rem, 2rem...)

Elements flex:
  flex: 1 1 300px (grow, shrink, basis)
  flex-grow: 1
  flex-shrink: 1
  flex-basis: 300px


CHECKLIST ABANS DE LLIURAR:
----------------------------
□ Tots els textos personalitzats (no [corxets])
□ Variables CSS copiades de l'Act 2
□ Google Fonts afegit al <head>
□ Navegació usa Flexbox (logo esquerra, menu dreta)
□ Hero usa Flexbox (contingut centrat)
□ Filtres usen Flexbox (botons en fila)
□ Grid de plats usa Flexbox amb flex-wrap
□ Cards internes usen Flexbox
□ Begudes usen Flexbox (layout horitzontal)
□ Footer usa Flexbox
□ Responsive funciona (provat amb DevTools)
□ HTML validat (W3C Validator)
□ CSS validat (W3C CSS Validator)
□ Document reflexiu completat


RECURSOS ÚTILS:
---------------
Teoria:
- CSS-Tricks Flexbox Guide: https://css-tricks.com/snippets/css/a-guide-to-flexbox/
- MDN Flexbox: https://developer.mozilla.org/es/docs/Learn/CSS/CSS_layout/Flexbox
- W3Schools Flexbox: https://www.w3schools.com/css/css3_flexbox.asp

Pràctica:
- Flexbox Froggy: https://flexboxfroggy.com/#ca
- Flexy Boxes: https://the-echoplex.net/flexyboxes/

Validadors:
- HTML: https://validator.w3.org/
- CSS: https://jigsaw.w3.org/css-validator/

DevTools:
- Obre amb F12
- Mode responsive: Ctrl+Shift+M
- Flexbox Inspector: icona de Flexbox al inspector


CONSELLS:
---------
✓ Treballa per seccions, no ho facis tot alhora
✓ Refresca el navegador després de cada canvi
✓ Usa DevTools per veure com funciona Flexbox
✓ Si no funciona, comprova que el contenidor tingui display: flex
✓ Usa background colors temporals per veure els límits
✓ gap és el teu millor amic per espaiat
✓ flex-wrap: wrap fa màgia per responsive
✓ Prova constantment en diferents mides de pantalla


ERRORS COMUNS:
--------------
✗ Oblidar display: flex al contenidor
✗ Confondre justify-content (horitzontal) amb align-items (vertical)
✗ No usar flex-wrap i que les cards es surtin de la pantalla
✗ Oblidar copiar les variables CSS de l'Act 2
✗ No provar en mòbil (sempre prova responsive!)
✗ Usar CSS Grid en lloc de Flexbox (Grid és per l'Act 4)


PREGUNTES FREQÜENTS:
--------------------
P: Puc usar CSS Grid?
R: NO. Aquesta activitat és només Flexbox. Grid vindrà a l'Act 4.

P: He de posar imatges reals?
R: Opcional. Pots deixar .dish-image amb background-color.

P: Quantes cards mínim he de tenir?
R: Mínim 3 entrants, 3 principals, 3 postres = 9 plats totals.

P: Puc canviar les categories?
R: Sí, adapta-les al teu tipus de restaurant.

P: Com sé si estic usant Flexbox correctament?
R: Obre DevTools, inspecciona l'element. Si té display: flex, veuràs
   un indicador especial de Flexbox.


LLIURAMENT:
-----------
Carpeta comprimida amb:
  □ menu.html (personalitzat)
  □ styles.css (completat amb Flexbox)
  □ document_reflexiu.pdf

Nom del zip: Cognom_Nom_Act3_Flexbox.zip

============================================================
Que gaudeixes aprenent Flexbox! 💪✨
Si tens dubtes, consulta l'enunciat complet o pregunta al professor.
============================================================