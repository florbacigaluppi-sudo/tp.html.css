# Trabajo Práctico: maquetación Web con HTML Y CSS

![Vista previa del proyecto](./assets/Vista%20previa%20proyecto/vistaprevia.PROYECTO.png)

Adjunto un screen  del sitio terminado.

## Desarrollo del Proyecto

### 1. Desarrollo del HTLM:

En primer lugar analice la estructura del Diseño que debía realizar, observando sus `sections`, `divs`, y `articles` posibles.

Dado que el diseño no ocupaba el tamaño total de la página decidí trabajarlo todo como una `section` en un sitio Web. Clasifique a esta `section` principal como _"card"_.

Por esta razón en mi diseño no hay un `header`, sino que para simularlo utilice una `div` a la cual nombre _"header"_. Incluye el logo, el nombre del sitio y el boton de _swichtmode_. Simula ser un `header`pero de la `section`principal, no del sitio.

Para el resto del HTML, también utilicé `divs` y los clasifique como _"text"_ para el título y `textarea`;
_"options"_ para los `checkbox`y "reading time"; _"results"_ para las tarjetas con los resultados (cada tarjeta es un `article`); y, por último _"letterdensity"_ para las letras, barras de progreso, porcentajes y botón. Cada una de las letras es una `li`dentro de una `ul`.

Para las "barras de progreso" investigue algunas opciones pero la que utilicé por practicidad fue crear dos `divs`, uno para definir el tamaño del contenedor de la barra, al cual clasifiqué _"bar"_, y otro para definir el tamaño de la línea de progreso de acuerdo al porcentaje, al cual clasifiqué _"fill"_.

Durante la creación del HTLM fui descargando las imagenes del logo, iconos de los dos botones y background de las tarjetas de resultados. Las descargue copiando la imagen en ChatGPT y luego acomodando el "tamaño del lienzo" en "Photoshop".

La mayor dificultad con el desarrollo de HLML fue la creación de las barras de progreso. 

### 2. Desarrollo de CSS:

En primer lugar definí las variables. Agregué los colores y las tipografías.

También reseteé los valores de `marging`y `padding`.

Luego comencé a definir el tamaño y estilos de mi `section`principal y su ubicación dentro de `body`.

Una vez definido el espacio con el que iba a trabajar el contenido de mi _"card"_, comencé a estilar cada uno de los `divs`por orden de aparición. 

Definí el padding de toda la `card` y luego fui dando `margin`y `padding`a cada `div` para que sea similar al sitio que debía diseñar. 

#### Header: 
Utilicé Flex Box para alinear los elementos horizotalmente; definí el tamaño del logo y del botón; alineé el botón a la derecha y lo estilé quitandole la apariencia por defecto.

#### Text:

Estilé el texto del título y `textarea` y luego quité la apariencia por defecto del `textarea`y le estilé los bordes, color.

#### Checkbox:

Utilicé FlexBox para alinear a los `inputs`y reading time horizontalmente.


#### Results:

También utilicé FlexBox en el contenedor principal de los `articles`para que aparezcan alineados horizontalmente. 

También utilicé FlexBox en cada `article`para que el contenido se pueda alinear y central. En este caso también utilicé `flex-direction: column`.

Cada `article`había sido clasificado previamente en HTLM como "_result1_" _"result2"_ y _"result3" para poder tener un selector distinto para cada uno, ya que cada uno tiene un `background`diferente.

#### LetterDensity"

Saqué la apariencia por defecto de la `ul`.
Estilé la fuente de las letras y el porcentaje

Cada uno de los items también utlizan FlexBox ya que la letra, la barra y el procentaje estan alineados horizontalmente. 

Luego dimensione el tamaño de la `bar`dandole un `width`y un `high`, y le di un `background-color`;  lo mismo hice con el `fill` dandole como `width`el porcentaje que figura para cada item y también le puse un `background-color`.

Por último, estilé el botón con su tamaño, color, borde, etc. 
 También utilicé FlexBox para alinear el texto con el icono horizonalmente. 

 #### ":hover": 
 Luego de haber estilizado a todos los `divs` con su contenido agregué los `:hover`. Agregue a los dos botones un cambio de `background` y un pequeño "zoom".

 También agregue un "zoom" a cada uno de las tarjetas de resultados.


 ### Responsitive Desing:

 Haciendo el diseño "_responsitive_" encontré varias dificultades. No pude solucionar que funcione el _"scroll vertical"_ en "Iphone 12" y otros dispositivos móviles. Sólo funciona en "Iphone SE" o en el modo "Responsitve" del DevTools.

 El problema es que baja el _"scroll"_ hasta una altura y luego se traba. 
 Adjunto imagenes en donde se ve el defecto.

 Vista en iPhone 12:

![Vista previa del proyecto](./assets/Vista%20previa%20proyecto/vistaprevia.iPhone12.png)

Es una captura del scroll de un Iphone 12. No baja el scroll y queda cortado el sitio.


Vista iPhone SE y modo Responsitive:

![Vista previa del proyecto](./assets/Vista%20previa%20proyecto/vistaprevia.RESPONSITIVE1.png)
![Vista previa del proyecto](./assets/Vista%20previa%20proyecto/vistaprevia.RESPONSITIVE2.png)

Esta en una captura del iPhone SE en donde el scroll si baja hasta el final del sitio.














