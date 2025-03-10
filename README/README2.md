# Portafolio-Curso1
Continuación del curso: HTML y CSS: ambientes de desarrollo, estructura de archivos y tags.
Curso: HTML y CSS: Clases, posicionamiento y Flexbox
Estudiante: Martín Emmanuel Gasga Varela

Documentación
https://www.w3schools.com/

Class

El atributo class permite al CSS seleccionar y acceder a elementos específicos a través de selectores de clase. Se declaran primero en el index.html como class="nombre-de-clase", posteriormente en el archivo style.css se declara como ."nombre-de-clase"{}

Reset CSS

Se utiliza para reiniciar el estilo por defecto de algún explorador, de modo que sea mas sencillo que los estilos sean similares entre diferentes navegadores.
Ejem:
* Resetear márgenes con margin: 0 en ciertos elementos como body, <h1> o <p>.
* Utilizar propiedades como box-sizing para facilitar cálculos de dimensiones.
* Utilizar display: inline-block para elementos por defecto inline que ignoran tamaños.

Referencia: https://lenguajecss.com/cascada-css/herencia/reset-css/


CSS Box Sizing

By default, the width and height of an element is calculated like this:

width + padding + border = actual width of an element
height + padding + border = actual height of an element

La propiedad box-sizing puede ser usada para ajustar el siguiente comportamiento:

* content-box es el comportamiento CSS por defecto para el tamaño de la caja (box-sizing). Si se define el ancho de un elemento en 100 pixeles, la caja del contenido del elemento tendrá 100 pixeles de ancho, y el ancho de cualquier borde o relleno ser añadirá al ancho final desplegado.
* border-box le dice al navegador tomar en cuenta para cualquier valor que se especifique de borde o de relleno para el ancho o alto de un elemento. Es decir, si se define un elemento con un ancho de 100 pixeles. Esos 100 pixeles incluíran cualquier borde o relleno que se añadan, y la caja de contenido se encogerá para absorber ese ancho extra. Esto típicamente hace mucho más fácil dimensionar elementos.


https://developer.mozilla.org/es/docs/Web/CSS/box-sizing
https://www.w3schools.com/csS/css3_box-sizing.asp


¿Qué es el Viewport?

En informática gráfica, el viewport es la porción del área visible de un plano y se utiliza como unidad de medida en CSS para crear páginas web 100% responsivas. En otras palabras, el viewport varía de dispositivo a dispositivo, por ejemplo, en computadoras, tabletas y teléfonos móviles, cada pantalla tiene dimensiones diferentes y mientras una página no responsiva presentaría elementos desproporcionados, una página responsiva utilizando viewport tendría sus elementos adecuados a cada proporción.


¿Qué es la etiqueta <section>?

La etiqueta <section> en HTML se utiliza para definir secciones en un documento. Una sección es un contenedor temático que agrupa contenido relacionado. Esta etiqueta es útil para estructurar el contenido de manera más clara y semántica, lo que facilita la comprensión tanto para los desarrolladores como para los motores de búsqueda.

Características principales de la etiqueta <section>:

1. Agrupación Temática: Agrupa contenido que pertenece a un mismo tema o propósito. Por ejemplo, un grupo de artículos sobre el mismo tema dentro de una página de noticias.

2. Mejora de la Semántica: Ayuda a mejorar la semántica del documento, lo que significa que los motores de búsqueda y otros agentes pueden entender mejor la estructura y el contenido de la página.

3. Accesibilidad: Facilita la navegación para tecnologías de asistencia, como lectores de pantalla, mejorando así la accesibilidad del sitio web.

4. Uso con Encabezados: Generalmente se utiliza en combinación con encabezados (<h1>, <h2>, etc.) para definir la estructura de la sección.

Ejemplo: 
<section>
  <h2>Título de la sección</h2>
  <p>Contenido relacionado con el tema de la sección.</p>
  <p>Más contenido relevante.</p>
</section>


CSS Flexbox

https://css-tricks.com/snippets/css/a-guide-to-flexbox/

* display
This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
.container {
  display: flex; /* or inline-flex */
}

* flex-direction
This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns.
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}

* justify-content
This defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line.
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}


FONTS
https://fonts.google.com/


Cuando usar una "div"

La etiqueta <div> define una división en un documento HTML y suele utilizarse como un contenedor para otros elementos, lo que ayuda en la estilización del bloque. Por este motivo, la <div> se utiliza frecuentemente cuando necesitamos agrupar elementos sin usar las etiquetas semánticas de HTML. Esto se debe a que la <div> no tiene valor semántico. Por lo tanto, no significa nada para los navegadores y motores de búsqueda.

Además, al ser muy utilizada para agrupar elementos, facilita la organización de la información en los diseños. De esta forma, puede ser formateada y manipulada orgánicamente a través de CSS. Por lo general, se acompaña de atributos de ID y clase para facilitar esta organización y formateo.


Gap

La propiedad gap no es exclusiva de Flexbox, sin embargo, se utiliza casi siempre en conjunto con él. Esta propiedad especifica en CSS el tamaño de los espacios entre filas y columnas en diseños de cuadrícula, flex y de varias columnas. Su sintaxis es bastante simple y acepta uno o dos valores.