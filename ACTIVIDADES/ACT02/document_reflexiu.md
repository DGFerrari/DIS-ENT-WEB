# Documento reflexivo - Freddy Fazbear's Pizza

## 1. Información del restaurante

**Nombre:** Freddy Fazbear's Pizza  
**Tipo de cocina:** Pizzería artesanal / restaurante familiar con estilo retro y temático de animatrónicos  
**Ambiente/personalidad:** La estética del restaurante combina un aire nostálgico de los años 80, familiar, divertido y algo teatral. La web transmite una sensación de celebración, comida reconfortante y experiencia compartida, con un tono mágico y entretenido que invita a la familia y a los grupos de amigos a visitar el local.

La propuesta visual y escrita del sitio refuerza la idea de un restaurante centrado en la diversión y la memoria del cine de atracciones y de los espacios de celebración infantiles. Los textos destacan que se trata de un lugar de encuentro para aniversarios, risas y momentos inolvidables, reforzando la identidad de un restaurante que combina la pizza artesanal con una experiencia lúdicamente teatral.

---

## 2. Justificación de la paleta de colores

La paleta utilizada en la página se basa en colores oscuros, intensos y contrastados que ayudan a crear una atmósfera de cine, misterio y energía retro. Los principales colores del proyecto son:

- `#121216` — negro profundo
- `#2B3542` — gris azulado
- `#D32F2F` — rojo intenso
- `#F2B84B` — dorado / ámbar
- `#F5F0E6` — crema clara
- `#C5BDAF` — taupe suave

### ¿Por qué estos colores?

- El negro y el gris oscuro crean un fondo sólido y elegante, y aportan contraste para destacar el contenido y reforzar el ambiente nocturno y teatral.
- El rojo es el color principal de acento y hace referencia a la energía, la pasión y la sensación de emoción. También ayuda a captar la atención del visitante y a diferenciar elementos clave como botones y cabeceras.
- El dorado aporta calidez y un toque de lujo ligero, muy útil para crear un efecto premium sin perder la simplicidad del restaurante familiar.
- La crema y el taupe aportan un contraste amable y legible para el texto y para zonas que necesitan una sensación más cálida y acogedora.

### ¿Qué se quiere transmitir?

La paleta busca comunicar un ambiente de:
- diversión
- nostalgia
- energía
- celebración familiar
- sensación de restaurante con personalidad propia

No se trata solo de colores agradables visualmente, sino de colores que refuerzan la idea de un local memorable y una experiencia de ocio. La combinación de colores oscuros con acentos rojos y dorados hace que el restaurante parezca más impactante y dinámico, mientras que la crema ayuda a equilibrar la composición y a mejorar la legibilidad.

### Enlace a la paleta generada

[Paleta Coolors basada en la web del restaurante](https://coolors.co/121216-2b3542-d32f2f-f2b84b-f5f0e6)

> Aquí se puede añadir la captura de la paleta generada en Coolors o Adobe Color, si se quiere entregar el documento con la imagen correspondiente.

---

## 3. Justificación de las fuentes

La tipografía elegida para la página es una combinación entre una fuente más impactante y otra más legible, adaptada a la personalidad del restaurante.

### Fuentes utilizadas

- **Fugaz One**: fuente decorativa y muy destacada para los títulos principales. Aporta un efecto más dinámico, expresivo y teatral.
- **Carter One**: fuente de titulares con forma más amigable y cercana, pero aún muy robusta y visualmente fuerte.
- **Arial, sans-serif**: fuente de apoyo para textos generales y párrafos, utilizada por su legibilidad y claridad.

### ¿Por qué encajan con el ambiente?

Las fuentes seleccionadas tienen un aire retro-futurista y de parque infantil/animatrónico, que encaja perfectamente con la idea de un restaurante familiar inspirado en la cultura pop y el mundo del entretenimiento. Además, el uso de una tipografía más grande y contundente en los títulos ayuda a dar fuerza visual a la marca y a reforzar el carácter festivo del restaurante.

La combinación de títulos expresivos con texto general ligero y legible consigue un equilibrio entre personalidad y funcionalidad, algo importante en una landing page de atracción y reserva.

> Enlaces a las fuentes:
> - [Google Fonts – Fugaz One](https://fonts.google.com/specimen/Fugaz+One)
> - [Google Fonts – Carter One](https://fonts.google.com/specimen/Carter+One)

---

## 4. Accesibilidad

La página intenta cumplir con criterios básicos de accesibilidad visual y navegación, ya que se cuida mantener un contraste claro entre los textos y los fondos, así como utilizar estilos de enfoque visibles para los elementos interactivos.

### Elementos que refuerzan la accesibilidad

- El texto principal es claro y, en su mayoría, se mantiene sobre fondos oscuros para garantizar contraste.
- Los botones y los enlaces tienen una identidad visual clara y una zona de enfoque visible mediante el estilo `:focus-visible`.
- Los controles del formulario tienen dimensiones adecuadas y un estilo consistente para facilitar la interacción.
- El HTML utiliza etiquetas semánticas (`header`, `section`, `footer`, `form`, `nav`, etc.) que ayudan a la navegación asistida.

### Consideraciones

Para un documento final más robusto, se puede comprobar la relación de contraste con herramientas como WebAIM Contrast Checker y validar que el rojo y el dorado no reduzcan la legibilidad del texto en estado normal. En general, la página presenta una buena lectura gracias al uso de fondos oscuros y textos blancos o crema.

> Aquí se pueden incorporar capturas de pantalla de los resultados de contraste y de la navegación con enfoque visible.

---

## 5. Validación HTML y CSS

La landing page está construida con una estructura HTML clara y separada por secciones, y el CSS utiliza variables para centralizar los colores, mantener la consistencia visual y facilitar la personalización.

### Puntos destacados de la validación

- La estructura del documento está bien organizada en `header`, `hero`, `about`, `menu`, `reservation` y `footer`.
- Se utilizan variables CSS en `:root` para no repetir códigos de color y hacer más mantenible el proyecto.
- Los cambios de tamaño y los breakpoints en `@media` ayudan a adaptar la disposición a diferentes tamaños de pantalla.
- El formulario y los elementos interactivos refuerzan la usabilidad y mantienen una coherencia visual.

### Herramientas de validación recomendadas

- W3C HTML Validator
- W3C CSS Validator
- WebAIM Contrast Checker

> En el documento final se pueden añadir capturas de las validaciones realizadas y los resultados obtenidos.

---

## 6. Capturas de pantalla

Las capturas a incluir en el documento final pueden ser:

- Vista completa de la landing page (scroll completo)
- Hero section con el título principal y el CTA
- Sección "Sobre nosotros"
- Tarjetas del menú con los platos destacados
- Formulario de reserva
- Footer con información de contacto

> Añade aquí las capturas del sitio web para completar la documentación visual.

---

## 7. Reflexión personal

El principal reto de esta actividad fue transformar una estructura básica HTML en una página con personalidad propia, sin alterar la semántica ni la funcionalidad del proyecto. La parte más importante fue decidir una identidad visual coherente que hiciera que el restaurante se percibiera como un lugar familiar, dinámico y memorable.

Una de las cosas que más me ha ayudado ha sido el uso de variables CSS. Me permiten centralizar colores y mantener el diseño más ordenado y fácil de modificar. Esto facilita la coherencia del proyecto y evita repetir códigos, algo muy útil en páginas con múltiples secciones y elementos repetidos.

También he aprendido que la tipografía y la paleta de colores no solo decoran la página: definen el ambiente, la marca y la forma en que el visitante percibe el restaurante. Un buen diseño debe combinar atractivo visual, legibilidad y funcionalidad, sin perder la claridad de la experiencia.

### Recursos consultados

- Google Fonts
- Coolors
- Documentación básica de CSS y HTML
- W3C y WebAIM

---

## Conclusión

Freddy Fazbear's Pizza es un ejemplo de restaurante con una propuesta visual fuerte y muy definida. La página consigue transmitir un estilo retro, divertido y familiar gracias a la combinación de colores oscuros e intensos, la tipografía impactante y la estructura clara de la landing page. El resultado es una propuesta que combina identidad visual, claridad y experiencia de navegación adecuada para un negocio que quiere captar clientes y reforzar su imagen de marca.
