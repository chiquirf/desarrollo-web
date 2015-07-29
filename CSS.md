#CSS interesante a tener en cuenta:

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
  
