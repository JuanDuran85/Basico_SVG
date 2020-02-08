# SVG (Scalable Vector Graphics.)

SVG significa Gráficos Vectoriales Escalables. Así mismo, SVG define gráficos basados ​​en vectores en formato XML.

Por otra parte, SVG se usa para definir gráficos basados ​​en vectores para la Web. Cada elemento y cada atributo en los archivos SVG pueden ser animados.

## Ventajas SVG

Las ventajas de usar SVG sobre otros formatos de imagen (como JPEG y GIF) son:

* Las imágenes SVG se pueden crear y editar con cualquier editor de texto.
* Las imágenes SVG se pueden buscar, indexar, crear scripts y comprimir.
* Las imágenes SVG son escalables.
* Las imágenes SVG se pueden imprimir con alta calidad en cualquier resolución.
* Las imágenes SVG se pueden ampliar.
* Los gráficos SVG NO pierden calidad si se amplían o cambian de tamaño.
* SVG es un estándar abierto.
* Los archivos SVG son XML puro.
* En HTML5, puede incrustar elementos SVG directamente en sus páginas HTML.

## Sintaxis y atributos de la etiqueta SVG
La sintaxis básica es sencilla, tan solo debemos poner la etiqueta y definir un tamaño inicial. En dicha etiqueta podemos poner los atributos y etiquetas que necesitemos para realizar nuestro gráfico vectorial.

Listado de etiquetas compatibles:

1. Animación: animate, animateColor, animateMotion, animateTransform y set.
2. Descriptivas: desc, metadata y title.
3. Formas: circle, ellipse, line, path, polygon, polyline y rect.
4. Estructura: defs, g, svg, symbol y use.
5. Degradados: linearGradient, radialGradient.
6. Otras: a, altGlyphDef, clipPath, color-profile, cursor, filter, font, font-face, foreignObject, image, marker, mask, pattern, script, style, switch, text y view.

Listado de atributos compatibles:

1. Condicionales: requiredFeatures, requiredExtensions y systemLanguage.
2. Core: id, xml:base, xml:lang y xml:space.
3. Eventos: onunload, onabort, onerror, onresize, onscroll y onzoom.
4. Eventos gráficos: onfocusin, onfocusout, onactivate, onclick, onmousedown, onmouseup, onmouseover, onmousemove, onmouseout y onload.
5. Presentación: alignment-baseline, baseline-shift, clip, clip-path, clip-rule, color, color-interpolation, color-interpolation-filters, color-profile, color-rendering, cursor, direction, display, dominant-baseline, enable-background, fill, fill-opacity, fill-rule, filter, flood-color, flood-opacity, font-family, font-size, font-size-adjust, font-stretch, font-style, font-variant, font-weight, glyph-orientation-horizontal, glyph-orientation-vertical, image-rendering, kerning, letter-spacing, lighting-color, marker-end, marker-mid, marker-start, mask, opacity, overflow, pointer-events, shape-rendering, stop-color, stop-opacity, stroke, stroke-dasharray, stroke-dashoffset, stroke-linecap, stroke-linejoin, stroke-miterlimit, stroke-opacity, stroke-width, text-anchor, text-decoration, text-rendering, unicode-bidi, visibility, word-spacing y writing-mode.
6. Otros: class, style, externalResourcesRequired, x, y, width, height, viewBox, preserveAspectRatio, zoomAndPan, version, baseProfile, contentScriptType, contentStyleType, x, y, width, height, version y baseProfile.

## Explicando algunas etiquetas, atributos y propiedas importantes para las etiquetas SVG

1. Elemento `<g>`: es un contenedor usado para agrupar objetos. Las transformaciones aplicadas al elemento g son realizadas sobre todos los elementos hijos del mismo. Los atributos aplicados son heredados por los elementos hijos. Además, puede ser usado para definir objetos complejos que pueden luego ser referenciados con el elemento `<use>`. La etiqueta g es bastante útil para agrupar formas geométricas que tienen atributos en común, sin embargo, su debilidad radica en el hecho de no poder colocar todos los atributos comunes en el elemento.
2. Elemento `<use>`: El elemento use toma los nodos que están dentro del documento SVG y duplica el contenido donde éste esté siendo utilizado. El efecto es el mismo, como si éstos nodos hubiesen sido profundamente clonados en un elemento DOM no expuesto, y luego pegados donde se encuentra el elemeto use.
3. Elemento `<defs>`: permite colocar todos los atributos comunes en el elemento (a diferencia de la etiqueta `<g>`) y con ayuda de la etiqueta use se puede definir una figura clave (mediante la etiqueta `<defs>`) con todos sus atributos y luego se puede usar y replicar esta definición tantas veces como se necesite mediante la etiqueta `<use>`.
4. El atributo "xlink:href " se emplea para identificar otro elemento en el documento mediante el marcado "#" que permite seguir a un elemento mediante el atributo id.
5. El atributo viewBox: establece la porción del plano SVG que muestra la imagen. Este atributo se establece con cuatro valores:

   * Primer valor: abcisa (X) de la esquina superior izquierda de la porción del plano que muestra la imagen.
   * Segundo valor: ordenada (Y) de la esquina superior izquierda de la porción del plano que muestra la imagen.
   * Tercer valor: ancho de la porción del plano que muestra la imagen.
   * Cuarto valor: alto de la porción del plano que muestra la imagen.

6. importante: Cualquiera de los elementos que sean incluídos dentro de `<defs>` no sera visible a la hora de reproducir el SVG, para que estos elementos sean visibles se deberá usar la etiqueta `<use>`.  
    
## Explicación de un código SVG para un circulo

* Una imagen SVG comienza con un elemento `<svg>`
* Los atributos de ancho y alto del elemento `<svg>` definen el ancho y alto de la imagen SVG
* El elemento `</circle>` se usa para dibujar un círculo.
* Los atributos cx y cy definen las coordenadas x e y del centro del círculo. Si no se establecen cx y cy, el centro del círculo se establece en (0, 0)
* El atributo r define el radio del círculo.
* Los atributos de trazo y ancho de trazo controlan cómo aparece el contorno de una forma. Establecemos el contorno del círculo en un "borde" verde de 4px
* El atributo de relleno se refiere al color dentro del círculo. Configuramos el color de relleno en amarillo
* La etiqueta de cierre `</svg>` cierra la imagen SVG
* Nota: ¡Dado que SVG está escrito en XML, todos los elementos deben cerrarse correctamente!

Por lo tanto, la descripción del ejemplo anterior seria:

```html
<!--Realizando un circulo con SVG-->
    <svg width="100" height="100">
        <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow"></circle>
    </svg>
```

SVG tiene algunos elementos de forma predefinidos que pueden ser utilizados por los desarrolladores:

* Rectangle `<rect>`
* Circle `<circle>`
* Ellipse `<ellipse>`
* Line `<line>`
* Polyline `<polyline>`
* Polygon `<polygon>`
* Path `<path>`

Para realizar un rectagulo, se debe trabajar con las instrucciones:

```html
    <!--Realizando un rectangulo con SVG-->
    <svg width="250" height="150">
        <rect width="150" height="100" class="rectangulo"></rect>
    </svg>
```

Explicación del código:

* Los atributos ancho y alto del elemento `<rect>` definen el alto y el ancho del rectángulo.
* El atributo de estilo se usa para definir propiedades CSS para el rectángulo.
* La propiedad de relleno CSS define el color de relleno del rectángulo.
* La propiedad de ancho de trazo CSS define el ancho del borde del rectángulo.
* La propiedad de trazo CSS define el color del borde del rectángulo.

Otro de los elementos o etiquetas mas utilizadas para SVG es el elemento `<path>` "ruta", el cual, se usa para definir una ruta. Ahora bien, los siguientes comandos están disponibles para datos de ruta:

* M,m = moveto.
* L,l = lineto.
* H,h = línea horizontal a.
* V,v = línea vertical a.
* C,c = curvato.
* S,s = curva suave.
* Q,q = curva de Bézier cuadrática.
* T,t = curva de Bézier cuadrática lisa.
* A,a = arco elíptico.
* Z,z = camino cerrado.

Nota importante: Todos los comandos anteriores también se pueden expresar con letras más bajas. Las letras mayúsculas significan absolutamente posicionadas, las minúsculas significan relativamente posicionadas.

Existen funciones o propiedades importantes que permiten modificar la figura creada en SVG por cualquiera de los elementos predefinidos. Estas propiedades son: el grosor de línea, el tipo de línea o la forma de los extremos:

* Stroke-width: Grosor de la línea.
* Stroke-dasharray: Líneas discontínuas. Requiere 2 valores, para la longitud de cada raya y la separación en ellas (ejemplo: “5,5”).
* Stroke-linecap: forma de los extremos (butt=recto, round=redondo, square=cuadrado).
* Fill: permite rellenar la figura con un color establecido.
* Stroke: asigna el color de la linea del contorno de la figura.
* Stroke-width: permite modificar el grosor de la linea de contorno de la figura.

Para mayor información relacionada a todos los atributos y propiedades sobre SVG, visitar: 
[SVG cheat sheet](https://learn-the-web.algonquindesign.ca/topics/svg-cheat-sheet/) 
[Desarrollo Libre](https://www.desarrollolibre.net/blog/html/dibujando-nuestro-propios-svg-en-html-parte-1#.Xj1aHCN-HIU). 
[Convalencia Web](https://covalenciawebs.com/crear-dibujos-vectoriales-directamente-en-la-web-svg-en-html/). 
[SVG Explicaciones](https://www.mclibre.org/consultar/htmlcss/html/html-svg.html).