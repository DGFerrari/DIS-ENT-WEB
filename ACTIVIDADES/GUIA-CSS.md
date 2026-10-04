# Guía básica de CSS

Esta guía reúne conceptos importantes para entender y escribir CSS en la práctica de Freddy Fazbear's Pizza. No hace falta memorizar todas las propiedades: lo más importante es comprender qué hacen y saber cuándo consultarlas.

## 1. ¿Qué es CSS?

CSS (*Cascading Style Sheets*, u hojas de estilo en cascada) define cómo se presenta el contenido HTML: colores, tipografías, tamaños, espacios, distribución y adaptación a diferentes pantallas.

Una regla CSS suele tener esta forma:

```css
selector {
  propiedad: valor;
}
```

Por ejemplo:

```css
h1 {
  color: gold;
  font-size: 2rem;
}
```

El selector `h1` elige los títulos de nivel 1. Las declaraciones entre llaves indican qué estilos aplicarles.

## 2. Selectores básicos

Los selectores sirven para elegir qué elementos HTML reciben un estilo:

```css
p {
  color: white;
} /* Todos los párrafos */

.aviso {
  color: gold;
} /* Elementos con class="aviso" */

#menu {
  padding: 2rem;
} /* El elemento con id="menu" */

nav a {
  text-decoration: none;
} /* Enlaces que están dentro de nav */
```

- Una **clase** (`class`) se puede usar en varios elementos. En CSS se escribe con un punto, como `.dish-card`.
- Un **id** (`id`) identifica normalmente un único elemento de la página. En CSS se escribe con `#`, como `#menu`.
- Un selector combinado, como `.nav-menu a`, elige enlaces que están dentro de un elemento con la clase `nav-menu`.

## 3. La cascada y la especificidad

Cuando varias reglas afectan al mismo elemento y propiedad, el navegador decide cuál aplicar. En términos generales:

1. Una regla más específica suele ganar a una menos específica.
2. Si las reglas tienen la misma especificidad, suele ganar la que aparece más abajo.
3. Los estilos en línea y `!important` tienen reglas especiales; es mejor no recurrir a `!important` salvo que haya un motivo claro.

```css
p {
  color: white;
}

.aviso {
  color: gold;
}
```

Un `<p class="aviso">` será dorado: la regla de clase es más específica que la regla del elemento `p`.

## 4. Reset básico y estilos generales

Los navegadores aplican algunos estilos por defecto, por ejemplo márgenes en títulos y párrafos. Un **reset** quita o normaliza parte de esos estilos para que la página empiece desde una base más predecible.

```css
*,
*::before,
*::after {
  box-sizing: border-box;
}

body,
h1,
h2,
h3,
p {
  margin: 0;
}
```

El reset no impide añadir márgenes más adelante. Una regla posterior y suficientemente específica puede dar a un elemento el espacio que necesite:

```css
p {
  margin: 0;
}

.about p {
  margin-top: 1rem;
}
```

La primera regla establece el punto de partida. La segunda añade margen superior a los párrafos de `.about`.

El reset es una elección, no una lista universal obligatoria. Es habitual quitar algunos márgenes y después definir deliberadamente el espaciado de cada sección.

## 5. El modelo de caja y `box-sizing`

Cada elemento se representa como una caja compuesta por:

- **Contenido (`content`)**: texto, imagen u otro contenido.
- **Relleno interior (`padding`)**: espacio entre el contenido y el borde.
- **Borde (`border`)**: línea que rodea el relleno y el contenido.
- **Margen (`margin`)**: espacio exterior que separa la caja de otros elementos.

La regla:

```css
*,
*::before,
*::after {
  box-sizing: border-box;
}
```

selecciona todos los elementos (`*`) y también los pseudo-elementos `::before` y `::after`. Con `border-box`, el `width` o `height` declarado incluye el contenido, el `padding` y el borde; el margen queda fuera.

Por ejemplo:

```css
.caja {
  width: 200px;
  padding: 20px;
  border: 5px solid;
}
```

Con `border-box`, el ancho total de la caja es de 200 px. Sin `border-box`, el ancho exterior sería 250 px: `200 + 20 + 20 + 5 + 5`.

## 6. Enlaces y estados interactivos

El navegador muestra los enlaces con estilos predeterminados, normalmente subrayados y de color azul o púrpura si ya se visitaron. Se pueden personalizar:

```css
a {
  color: inherit;
  text-decoration: none;
}
```

- `color: inherit` hace que el enlace use el color de texto heredado de su elemento contenedor.
- `text-decoration: none` quita el subrayado.

Es importante que el usuario pueda reconocer los elementos interactivos y navegar con teclado. Por ejemplo:

```css
a:hover {
  text-decoration: underline;
}

a:focus-visible {
  outline: 3px solid gold;
  outline-offset: 3px;
}
```

`:hover` se activa al pasar el cursor. `:focus-visible` ofrece una indicación visible cuando se llega al enlace con el teclado. No conviene quitar el foco visible sin proporcionar otra señal clara.

## 7. Variables CSS

Las variables CSS permiten guardar valores reutilizables. Se suelen declarar en `:root`, que las hace disponibles en toda la página:

```css
:root {
  --primary-color: #121216;
  --accent-color: #d32f2f;
}

h1 {
  color: var(--accent-color);
}
```

Los nombres de variables personalizadas empiezan con dos guiones (`--`) y se usan mediante `var(...)`. Si se cambia `--accent-color`, se actualizan las reglas que usan esa variable.

Son útiles para mantener una paleta de colores y valores compartidos sin repetirlos por todo el archivo.

## 8. Tipografía y unidades

Algunas unidades comunes:

- `px`: unidad fija; suele ser útil para detalles como bordes.
- `rem`: relativo al tamaño de letra raíz; es práctico para texto, rellenos y márgenes.
- `%`: relativo a una dimensión del elemento contenedor.
- `vw`: relativo al ancho de la ventana del navegador.
- `fr`: fracción del espacio disponible en CSS Grid.

`clamp()` permite que un valor crezca o disminuya dentro de límites:

```css
h1 {
  font-size: clamp(2rem, 5vw, 4rem);
}
```

En este ejemplo, el tamaño intenta seguir el ancho de la ventana (`5vw`), pero no baja de `2rem` ni supera `4rem`.

## 9. Flexbox y Grid

Flexbox y Grid sirven para distribuir elementos, pero suelen resolver problemas distintos:

- **Flexbox** organiza elementos en una dirección principal: una fila o una columna.
- **Grid** organiza elementos en filas y columnas.

Ejemplo de navegación en fila con Flexbox:

```css
nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 1rem;
}
```

- `display: flex` activa Flexbox.
- `align-items` alinea los elementos en el eje perpendicular.
- `justify-content` reparte el espacio en el eje principal.
- `gap` establece separación entre elementos.

Ejemplo de tarjetas en Grid:

```css
.dishes {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 1rem;
}
```

Esto crea tres columnas de igual tamaño. `minmax(0, 1fr)` permite que las columnas compartan el espacio disponible y ayuda a evitar que contenido largo fuerce el ancho de una columna.

## 10. Diseño adaptable y media queries

Una página adaptable (*responsive*) ajusta su distribución para distintos tamaños de pantalla. Las media queries aplican reglas solo cuando se cumple una condición:

```css
@media (max-width: 520px) {
  .dishes {
    grid-template-columns: 1fr;
  }
}
```

En este caso, cuando la ventana mide 520 px o menos, las tarjetas pasan a una columna. Así se evita intentar mostrar tres tarjetas estrechas en un móvil.

Conviene comprobar la página en tamaños grandes y pequeños. No hay un único ancho correcto para todos los diseños: el punto de cambio depende de cuándo el contenido empieza a quedar apretado.

## 11. Orden y mantenimiento del CSS

- Agrupa las reglas por secciones de la página, como navegación, portada, menú y formulario.
- Usa nombres de clase que describan la función del elemento, por ejemplo `.dish-card`.
- Reutiliza variables para colores y valores compartidos.
- Evita repetir reglas o acumular selectores demasiado específicos si una clase clara resuelve el caso.
- Mantén juntas las reglas relacionadas y coloca las media queries de forma ordenada.
- Si algo no se ve como esperabas, usa las herramientas de desarrollo del navegador para inspeccionar el elemento y comprobar qué reglas están activas o sobrescritas.

## 12. Qué merece la pena aprender primero

Prioriza entender estos conceptos:

1. Selectores de elementos, clases e ids.
2. Cascada, herencia y especificidad.
3. Modelo de caja: `margin`, `padding`, `border` y `box-sizing`.
4. Flexbox para distribuciones en una dimensión.
5. Grid para filas y columnas.
6. Media queries para adaptar el diseño.
7. Estados de interacción y foco visible.
8. Variables CSS para valores reutilizables.

No es necesario memorizar todas las propiedades. Es más útil entender cómo se combinan las reglas, practicar con ejemplos pequeños y consultar la documentación cuando aparezca una propiedad nueva.
