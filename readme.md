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
