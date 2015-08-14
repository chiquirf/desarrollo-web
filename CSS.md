#CSS tips:

* Tamaños de fuentes a *16px* para párrafos y usar "*em*" como unidades para el resto.
* Links: definir: *link* (default) = *visited* y *hover*. *selected* no ponerlo a menos que fuera necesario.
* List - Shorthand property para personalizar: *ul { list-style: square inside url("sqpurple.gif"); }*
* *The clearfix Hack* >> no es necesario poner un div vacio al final con clear:both; solo ponder el contenedor overflow: auto;
* Usar *display: inline-block;* en vez de float: left; para crear un grid de cajas responsive.
* SELECTORES:
  - Clases: *.nombre-clase {...}*
  - Id: *#id-elemento {...}*
  - Elemento: *elemento {...}*
  - Descendant Selector *div p {...}*
  - Child Selector *div > p {...}*
  - Adjacent Sibling Selector *div + p {...}*
  - General Sibling Selector *div ~ p {...}*   (~ = Alt+126)
* PSEUDO-CLASES: 
  - Anchor: *a:link / a:visited / a:hover / a:active* (se pueden combinar con CSS: a.highlight:hover)
  - *:first-child* pseudo-class matches a specified element that is the first child of another element. p:first-child / p i:first-child / p:first-child i
  - :lang pseudo-class allows you to define special rules for different languages.

#CSS3 tips:

* CSS3 background (IE>9)
  - SHORTHAND: background: color image position/size repeat origin clip attachment initial|inherit;
  - multiples fondos separando sus valores con "comas", ejemplo >>> background: url(img_flwr.gif) right bottom no-repeat, url(paper.gif) left top repeat;
  - Full Size Background Image. ejem >> html { background: url(img_flower.jpg) no-repeat center center fixed; background-size: cover; }
  - background-size: auto|length|cover|contain|initial|inherit; >>> "length" = [todo | ancho alto] // "contain" ajusta img para que entre toda en el contenedor // "cover" ajusta para que llene todo el contenedor.
  - background-origin: padding-box|border-box|content-box|initial|inherit;  >>>  donde se posiciona la imagen de fondo, y contando desde: padding-box (default) / border-box / content-box.
  - background-clip: border-box|padding-box|content-box|initial|inherit; >>> define área a pintar de fondo, y contando desde: border-box (default) / padding-box / content-box.
* CSS3 Colors (IE>9)
  - CSS supports color names, hexadecimal and RGB colors, CSS3: RGBA colors, HSL colors, HSLA colors, opacity. ejem >>> rgba(255, 0, 0, 0.6);
  - rgba(red, green, blue, alpha) >> rgba(0-255, 0-255, 0-255, 0-1)
  - hsla(hue, saturation, lightness, alpha) >> hsla(0-360, 0-100%, 0-100%, 0-1) >>> hue: 0 o 360 = red, 120 = green, 240 = blue ; Saturation 100% full color ; Lightness 0% is dark (black) and 100% is white.
  - Opacity: background-color:rgb(255,0,0);opacity:0.6;  == background-color:rgba(255,0,0,0.6);
* CSS3 Gradients (IE>10) 
  - background: (+prefix)linear-gradient(direction, color-stop1, color-stop2, ...);  [CSS-tricks - CSS3Gradient](https://css-tricks.com/examples/CSS3Gradient)
* CSS3 text Shadow Effects (IE>10) 
  - text-shadow: h-shadow v-shadow blur-radius color|none|initial|inherit;  >>> Acepta Multiple Shadows separandolo con comas.
* CSS3 box Shadow Effects (IE>9.0 +prefix)
  - box-shadow: none|h-shadow v-shadow blur spread color |inset|initial|inherit;  Acepta Multiple Shadows separandolo con comas.
* CSS3 Text
  - text-overflow: clip|ellipsis|string|initial|inherit; (IE>6) >>> muestra solo el texto que cabe dentro de un contenedor, combinar con "white-space: nowrap; overflow: hidden;" / ellipsis agrega puntos suspensivos al final.
  - word-wrap: normal|break-word|initial|inherit; (IE>5.5) >>> default "normal" que no corta las palabras y se ven fuera del contenedor, usar "break-word" para cortar las palabras sin contar sílabas de idioma.
  - word-break: normal|break-all|keep-all|initial|inherit; (IE>5.5)  >>> break-all rompe las palabras por caracteres para encajar en el contenedor. Por defecto no corta las palabras... ES LO NORMAL :)
* CSS3 Web Fonts (IE >9) 
  - @font-face { font-family: myFirstFont; src: url(sansation_light.woff); } *IE: The font format only works when set to be "installable" <<< Creo que se refiere al FTP con permisos 777.
  - Using Bold Text: agregar otra declaración agregando las reglas: @font-face { font-family: myFirstFont; src: url(sansation_bold.woff); font-weight: bold; }
  - Font Descriptors : font-family*, src*, font-stretch, font-style, font-weight, unicode-range (*)requeridos [CSS3 @font-face](http://www.w3schools.com/cssref/css3_pr_font-face_rule.asp)
* CSS3 2D Transforms (IE>10 o IE>9+prefix)
  - transform: none|transform-functions|initial|inherit; >>> varias transform-functions separadas por espacio, NO POR COMA.
  - transform functions >>> translate() rotate() scale() skewX() skewY() matrix()
  - transform-origin: x-axis y-axis|initial|inherit; >>> cambia el "origen" de la transformación, por ejemplo, rotate empieza en el top-left, pero con origin se puede modificar el eje de rotación: div { transform: rotate(45deg); transform-origin: 20% 40%; } SIEMPRE DEBE IR ACOMPAÑADO DE "transform".
* CSS3 3D Transforms (IE>10)
  - transform: none|transform-functions|initial|inherit; >>> varias transform-functions separadas por espacio, NO POR COMA.
  - transform functions >>> rotateX() rotateY() rotateZ()
  - transform-origin: x-axis y-axis z-axis|initial|inherit; >>> cambia el "origen" de la transformación, por ejemplo, rotate empieza en el top-left, pero con origin se puede modificar el eje de rotación.
  - transform-style: flat|preserve-3d|initial|inherit; >>> especifica cómo los elementos anidados se renderizan en el espacio 3D.  [demo](http://www.w3schools.com/cssref/trycss3_transform-style_inuse.htm)
  - perspective: length|none; >>> Ajusta el punto de vista desde donde se ve un elemento. (usar en combinación de perspective-origin)
  - backface-visibility: visible|hidden|initial|inherit;  >>> define si la parte trasera de un elemento debe ser visible o no cuando no está frente a la pantalla, muy util al rotar un elemento.
* CSS3 Transitions (IE>10)
  - IMPORTANTE: Para crear un efecto de transición, debe especificar dos cosas sobre el elemento: 1) la propiedad CSS que desea añadir un efecto y 2) la duración del efecto. Luego se aplica (por ejemplo con :hover) el cambio.
  - transition: property duration timing-function delay|initial|inherit;  (se pueden agregar más propiedades y sus tiempos separándolos con comas)
  - transition-property: none|all|property|initial|inherit;  >>> indicar la propiedad que se van a cambiar.
  - transition-duration: time|initial|inherit;  >>> tiempo de la transición
  - transition-timing-function: ease|linear|ease-in|ease-out|ease-in-out|cubic-bezier()|initial|inherit;  >>> especifica la curva de velocidad del efecto de transición.
  - transition-delay: time|initial|inherit;  >>>  especifica un retardo (en segundos) para el efecto de transición.
  - Se puede combinar Transition + Transformation  >>> transition: width 2s, height 2s, transform 2s;   [VER EJEMPLO](http://www.w3schools.com/css/tryit.asp?filename=trycss3_transition_transform)
* CSS3 Animations (IE>10)
  - @keyframes animationname {keyframes-selector {css-styles;}} >>> define la animación que va a cambiar gradualmente desde el estilo actual al nuevo estilo en determinados momentos.
  - elemento >>> se agregan alguna de las propiedades mínimo animation-name y animation-duration
  - keyframes-selector >>> Porcentaje: 0%-100%  //  inicio y fin: from{}  to{} >>>> Ejemplos: @keyframes animationname {from {color: red;} to {color: yellow;}}  ===  @keyframes animationname {0%{color: red;} 100%{color: yellow;}}
  - SHORTHAND: animation: name duration timing-function delay iteration-count direction fill-mode play-state;
  - animation-name: keyframename|none|initial|inherit; >>> define el nombre de la animación a usar
  - animation-duration: time|initial|inherit; >>> define el tiempo de la animación.  
  - animation-timing-function: linear|ease|ease-in|ease-out|cubic-bezier(n,n,n,n)|initial|inherit; >>> especifica la curva de velocidad de una animación.
  - animation-delay: time|initial|inherit; >>> retardo de inicio de la animación.
  - animation-iteration-count: number|infinite|initial|inherit; >>>  especifica el número de veces que una animación se debe reproducir.
  - animation-direction: normal|reverse|alternate|alternate-reverse|initial|inherit;  >>> orden de la animación // alternate (normal cada tiempo impar, reverse cada tiempo par) alternate-reverse (al reves que alternate)
  - animation-fill-mode: none|forwards|backwards|both|initial|inherit;  >>> especifica un estilo para el elemento cuando no se está reproduciendo la animación (cuando esté terminado, o cuando se tiene un retraso).
  - animation-play-state: paused|running|initial|inherit; >>> Especifica si la animación está en funcionamiento o en pausa.
* CSS3 Multiple Columns (IE>10)
  - SHORTHAND: columns: auto|column-width column-count|initial|inherit;  >>> Una propiedad abreviada para establecer la column-width y la column-count.
  - column-count: number|auto|initial|inherit;  >>> Especifica el número de columnas de un elemento se debe dividir.
  - column-gap: length|normal|initial|inherit;  >>> Especifica el espacio entre las columnas.
  - column-rule: column-rule-width column-rule-style column-rule-color|initial|inherit; >>> A shorthand property for setting all the column-rule-* properties.
  - column-rule-style: none|hidden|dotted|dashed|solid|double|groove|ridge|inset|outset|initial|inherit;  >>> Especifica el estilo de la regla entre columnas.
  - column-rule-width: medium|thin|thick|length|initial|inherit;  >>>  Especifica el ancho de la regla entre columnas.
  - column-rule-color: color|initial|inherit;  >>>  Especifica el color de la regla entre columnas.
  - column-span: 1|all|initial|inherit;  >>>  Especifica el número de columnas que un elemento debe extenderse a lo largo (si hay un H2 dentro del P por ejemplo).
  - column-width: auto|length|initial|inherit;  >>>  Especifica un ancho óptimo sugerido para las columnas (la cantidad no debe ser definida para que se asigne automáticamente por el ancho).
 * CSS3 box-sizing Property (IE>8) 
   - width + padding + border = actual width of an element  ///  height + padding + border = actual height of an element.
   - La propiedad CSS3 box-sizing: border-box; nos permite incluir el padding  y el border de la anchura y la altura total del elemento.
   - box-sizing: content-box|border-box|initial|inherit;  >>>  se sigiere * { box-sizing: border-box; } siempre "[ejemplo](http://www.w3schools.com/cssref/tryit.asp?filename=trycss3_box-sizing)".  
