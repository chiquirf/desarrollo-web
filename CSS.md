#CSS interesante a tener en cuenta:

* Tamaños de fuentes a *16px* para párrafos y usar "*em*" como unidades para el resto.
* Links generales: *link* (default) = *visited* y *hover* = *selected*
* List - Shorthand property para personalizar: *ul { list-style: square inside url("sqpurple.gif"); }*
* List: *ul { list-style-type: none;}* == *ul li { list-style: none;}*
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
* PSEUDO-CLASSES: 
  - Anchor: *a:link / a:visited / a:hover / a:active* (se pueden combinar con CSS: a.highlight:hover)
  - Input: *:focus / :checked / :disabled / :enabled / :in-range / :invalid / :optional / :out-of-range / :read-only / :read-write / :required*
  - Parrafo: *:first-child / :first-of-type / :lang(language) (HTML: &lt;q lang="language"&gt;) / :last-child / :last-of-type / :nth-child(n) / :nth-last-child(n) / :nth-last-of-type(n) / :nth-of-type(n)* 
  - Letra capital Blog: p:first-child::first-letter {color: #ff0000; font-size:200%;}
  - :lang pseudo-class allows you to define special rules for different languages. CSS: q:lang(no) / HTML: &lt;q lang="no"&gt;
  - Ver más [Pseudo-classes](http://www.w3schools.com/css/css_pseudo_classes.asp)
* PSEUDO-ELEMENTS:
  - INSERT: *::after / ::before* + propiedad: *content: "text";* o *content: url(smiley.gif);*
  - SELECT: *::first-letter / ::first-line / ::selection*
  - Ver más [Pseudo-elements](http://www.w3schools.com/css/css_pseudo_elements.asp)
* opacity: 0.4; filter: alpha(opacity=40); /* For IE8 and earlier */
* USABILIDAD: the font-size property can be used for both screen and print media, but perhaps with different values. A document usually needs a larger font-size on a screen than on paper, and sans-serif fonts are easier to read on the screen, while serif fonts are easier to read on paper.
* Attribute Selectors:   
  - *[attribute]* (existe attr)
  - *[attribute="value"]* (igual)
  - *[attribute~="value"]* (contiene palabra especificada) (~ = Alt+126)
  - *[attribute|="value"]* (empieza palabra completa, [class|=top] >> SI: class="top-header" / NO:class="topcontent"> )
  - *[attribute^="value"]* (empieza con caracters, [class|=top] >> SI: class="top-header" / SI:class="topcontent"> )
  - *[attribute$="value"]* (termina con caracteres)
  - *[attribute*="value"]* (contiene caracteres)
* border-radius: orden: top-left top-right bottom-right bottom-left. Se pueden poner dos vlores por cada esquina *border-radius: 50px/15px;*


