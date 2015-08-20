# BOOTSTRAP

[Bootstrap 3 Tutorial](http://www.w3schools.com/bootstrap/default.asp)

* **Bootstrap Get Started** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_get_started.asp)
  - Bootstrap 3 is mobile-first
  - agregar: <code>&lt;meta name="viewport" content="width=device-width, initial-scale=1"></code>
  - Crear DIV contenedor de TODA la web con:
    - .container: proporciona un responsive **fixed width container**
    - .container-fluid proporciona un **full width container**, que abarca toda la anchura de la ventana gráfica

* **Grid System** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_grid_basic.asp)
  - Grid System >> 12 columnas que se pueden agrupar (siempre debe sumar 12 por fila) .col-#-# >> .col-(clase)-(tamaño)
  - Grid Classes >> xs (for phones) / sm (for tablets) / md (for desktops) / lg (for larger desktops) >> .col-xs-4  .col-md-2  
  - Structure of a Bootstrap Grid >> Crear bloque para la fila con clase **.row**, luego agregar bloques con clase **.col-#-# ** para las columnas
  - Bloque estructura básica:
    <pre><code>&lt;div class="row">
  &lt;div class="col-#-#">&lt;/div>
  &lt;div class="col-#-#">&lt;/div>
  &lt;div class="col-#-#">&lt;/div>
&lt;/div></code></pre>

* **Text/Typography** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_ref_css_text.asp)
  - Default: body {font-size: 14px; line-height: 1.428}  (numero sin unidades es multiplicador >> 1.428   - 14px = 20px)  >>>> CAMBIARLO A font-size 16px !!!!!!!!
  - &lt;small> para crear texto secundario y más claro en cualquier título >>> &lt;h1>h1 &lt;small>sec text&lt;/small>&lt;/h1>
  - &lt;blockquote> >>> <code>&lt;blockquote> &lt;p>quotee.&lt;/p> &lt;footer>From WWF's website&lt;/footer> &lt;/blockquote></code>  //  .blockquote-reverse = alineado a la derecha
  - Otras etiquetas: mark abbr dl code kbd(teclado) pre
  - Text Color Contextual Class: .text-muted, .text-primary, .text-success, .text-info, .text-warning, and .text-danger (cada uno tiene un color diferente)
  - BG Color Contextual Class: .bg-primary, .bg-success, bg-info, bg-warning, and .bg-danger
  - transformar: .lead	(Makes a paragraph stand out) // .small	(Indicates smaller text (set to 85% of the size of the parent))  // .initialism (texto dentro de addr font-size:90% y capitalize)
  - alinear: .text-left .text-center .text-right .text-justify .text-nowrap
  - letras: .text-lowercase .text-uppercase .text-capitalize
  - listas: .list-unstyled (quita estilo y margen, no hereda a child) // .list-inline
  - descripciones: (dl > dt > dd dd) .dl-horizontal (primer dt alineado con dd)
  - .pre-scrollable >>> { max-height: 340px; overflow-y: scroll; }

* **Tables** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_ref_css_tables.asp)
  - BASICO: .table >> estilo básico, solo bordes horizontales interiores.
  - .table-striped >> alterna background de filas (como Zebra).
  - .table-bordered >> borde a toda la tabla y celdas.
  - .table-hover >> agrega bg-color al hacer hover a la fila.
  - .table-condensed >> más compacta cortando el padding a la mitad.
  - BG Color Contextual Class: se puede aplicar sobre los TR, TH y TD: .success, .info, .warning, .danger, y adicionalmente ".active" que es el mismo color que .table-striped.
  - Responsive Tables: agregar un bloque (div) contenedor con la clase .table-responsive
  
* **Images** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_ref_css_images.asp)
  - Formas: .img-rounded .img-circle .img-thumbnail
  - .img-responsive >> max-width: 100%; height: auto;
  - Gallery >> .thumbnail se puede aplicar al enlace padre de cada img
  - Responsive Embeds: 16by9 o 4by3, se aplica a &lt;iframe>, &lt;embed>, &lt;video>, and &lt;object> elements. 
    - CONTENEDOR: class="embed-responsive embed-responsive-16by9"
    - ELEMENTO: class="embed-responsive-item"

* **Jumbotron and Page Header**  [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_jumbotron_header.asp)
  - Jumbotron muestra una caja grande para llamar la atención adicional a algún contenido o información especial.
 - Usar un &lt;div> con la class <code>.jumbotron</code> para crear un jumbotron
 - Colocar el jumbotron dentro de <code>&lt;div class="container"></code> si NO queremos que el jumbotron se extiendahasta los bordes de la pantalla. y fuera si lo contrario.
 - Page Header : la clase .page-header agrega una linea horizontal debajo del header (+ agrega algo de espacio extra alrededor del elemento)
 
* **Wells** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_wells.asp)
  - La clase .well añade un borde redondeado en torno a un elemento con un color de fondo gris y algo de relleno.
  - Tamaños: class="well well-sm" (Small Well) // class="well" (Normal Well) // class="well well-lg" (Large Well)

* **Alerts** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_ref_js_alert.asp)
  - muestra cuadro con mensaje .
  - Crear: .alert (tiene que ser acompañado con contextual class)
  - Color: .alert-success, .alert-info, .alert-warning or .alert-danger
  - Closing Alert: agregar dentro del box lo siguiente: <code>&lt;a href="#" class="close" data-dismiss="alert" aria-label="close"> &_times_; &lt;/a></code>
  - Animated Alerts: The .fade and .in classes adds a fading effect when closing the alert message: <code>&lt;div class="alert alert-success fade in"></code>
  
* **Buttons** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_ref_css_buttons.asp)
  - HTLM: aplicable a: a, button, input
  - BASIC: .btn (siempre debe aplicarse)
  - STYLES: .btn-default, .btn-primary, .btn-success, .btn-info, .btn-warning, .btn-danger, .btn-link
  - SIZE: .btn-lg, .btn-md, .btn-sm, .btn-xs
  - BLOCK: .btn-block >> crea un botón tipo bloque (ancho 100%)
  - ACTIVE: .active >> hace que el aparezca como presionado
  - DISABLED: .disabled >> hace el boton no se pueda clickar.

* **Button Groups** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_ref_css_buttons.asp)
  - BASICO: crear bloque contenedor con clase .btn-group
  - SIZE: .btn-group-# (#=[lg|md|sm|xs]) >> se puede aplicar a todo el grupo
  - VERTICAL: .btn-group-vertical >> alinea verticalmente los botones (no poner .btn-group)
  - JUSTIFIED: .btn-group + .btn-group-justified >> modifica el ancho para que ocupen el 100%
    - a element: aplica directo al contenedor nada más,
    - button element: se debe envolver cada button en un bloque con clase .bt-group
  - Nesting Button Groups & Dropdown Menus
    el botón lanza el desplegable
    <code><pre>
        &lt;div class="btn-group">
          &lt;button type="button" class="btn btn-primary">Apple&lt;/button>
          &lt;button type="button" class="btn btn-primary">Samsung&lt;/button>
          &lt;div class="btn-group">
            &lt;button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
            Sony &lt;span class="caret">&lt;/span>&lt;/button>
            &lt;ul class="dropdown-menu" role="menu">
              &lt;li>&lt;a href="#">Tablet&lt;/a>&lt;/li>
              &lt;li>&lt;a href="#">Smartphone&lt;/a>&lt;/li>
            &lt;/ul>
          &lt;/div>
        &lt;/div>
    </pre></code>
  - Split Button Dropdowns
    el botón se mantiene y se crea una flecha para el resto
    <code><pre>
        &lt;div class="btn-group">
          &lt;button type="button" class="btn btn-primary">Sony&lt;/button>
          &lt;button type="button" class="btn btn-primary dropdown-toggle" data-toggle="dropdown">
            &lt;span class="caret">&lt;/span>
          &lt;/button>
          &lt;ul class="dropdown-menu" role="menu">
            &lt;li>&lt;a href="#">Tablet&lt;/a>&lt;/li>
            &lt;li>&lt;a href="#">Smartphone&lt;/a>&lt;/li>
          &lt;/ul>
        &lt;/div>
    </pre></code>
  
* **Glyphicons**  [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_glyphicons.asp)
  - Bootstrap ofrece 200 glyphicons del conjunto [Glyphicons](http://glyphicons.com/) Medianos
  - Syntax: <code>&lt;span class="glyphicon glyphicon-*name*">&lt;/span></code>
  - Ejemplos: .glyphicon-envelope .glyphicon-search .glyphicon-print 
  - [Lista de nombres](http://www.w3schools.com/bootstrap/bootstrap_ref_comp_glyphs.asp)
  - NO TIENE ICONOS DE REDES SOCIALES
  
* **Badges and Labels** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_ref_comp_navs.asp)
  - BADGES: son indicadores numéricos de cuántos elementos se asocian con un enlace.
    - Usar la clase .badge  en un elemento &lt;span> para crear un badges dentro de un enlace o un botón.
  - LABELS: se utilizan para proporcionar información adicional acerca de algo
    - Básico: .label y se aplica a un &lt;span>
    - Style: .label-default, .label-primary, .label-success, .label-info, .label-warning or .label-danger
    - Tamaño lo dicta elemento padre.
    
* **Progress Bars** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_progressbars.asp)
  - PARTES:
    - 1 Contenedor: <code>&lt;div class="progress"></code>
    - 2 Barra: <code>&lt;div class="clases" role="progressbar" aria-valuenow="porcentaje" aria-valuemin="0" aria-valuemax="100" style="width:porcentaje"></code>
    - 3 Etiqueta: texto directo o con <code>&lt;span class="sr-only">70% Complete&lt;/span></code> para que no se muestre.
  - TIPOS (aplicados al DIV de la barra:
    - BASICO: <code>&lt;div class="progress-bar" role="progressbar" aria-valuenow="70" aria-valuemin="0" aria-valuemax="100" style="width:70%"></code>
    - Colored: .progress-bar-success, .progress-bar-info, .progress-bar-warning, .progress-bar-danger
    - Striped: .progress-bar-striped >> a rayas
    - Animated: .progress-bar-striped + .active >> las dos juntas para que las rayas se muevan.
    - Stacked: agregar multiple div's de las barras al contenedor .progress, sin los atributos aria-#
    
* **Pagination** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_ref_comp_navs.asp)
  - Basic: Para crear una paginación básica, agregue la clase .pagination a un elemento &lt;ul>
  - Active State: agregar la clase .active al &ltli> correspondiente.
  - Disabled State: agregar la clase .disabled al &ltli> correspondiente.
  - Sizing: pagination + [.pagination-lg (grande) | sin nada (normal) |  .pagination-sm (pequeño)]
  - Pager: Para crear botones anterior/siguiente, añadir la clase .pager a un elemento &lt;ul>
  - Pager aling: para alinear a los laterales de la pagina, agregar .previous and .next a los &li> correspondientes.
  
* **List Groups** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_list_groups.asp)
  - Basic: utilizar un &lt;ul> con .list-group, y &lt;li> con clase .list-group-item
  - With Linked Items: en vez de UL y LI, utiliza DIV y A, se puede mantener activado con la clase.active
  - Disabled: agregar la clase .disabled al item.
  - Contextual Classes: .list-group-item + [.list-group-item-success | .list-group-item-info | .list-group-item-warning | .list-group-item-danger]
  - Custom Content, dentro de las listas o enlaces se puede poner un encabezado (H4) y un parrafo (P) con los siguientes clases: .list-group-item-heading y .list-group-item-text
  
* **Panels** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_panels.asp)
  - Un panel en bootstrap es una caja con borde con un poco de padding alrededor de su contenido.
  - BASICO: Los paneles se crea con la clase .panel y contenido dentro del panel tiene una clase .panel-body.
  - Heading: La clase .panel-heading agrega un encabezado en el panel.
  - Footer: La clase .panel-footer agrega un footer en el panel.
  - Group: envolver con un DIV con clase .panel-group varios paneles (quita el margin-bottom de los paneles)
  - Contextual Classes: .panel-default, .panel-primary, .panel-success, .panel-info, .panel-warning, or .panel-danger
  
* **Dropdowns** [ver detalles](http://www.w3schools.com/bootstrap/bootstrap_ref_js_dropdown.asp)
  - La clase .dropdown indica un menú desplegable.
  - Para abrir el menú desplegable, utilice un botón o un enlace con una clase de .dropdown-toggle y el atributo <code>data-toggle="dropdown"</code>.
  - La clase .caret crea un icono de flecha-abajo, que indica que el botón es un desplegable.
  - Agregue la clase .dropdown-menu para un &lt;ul> para construir realmente el menú desplegable.
  - Divider >> La clase .divider se utiliza para separar los enlaces dentro del menú desplegable (se aplica al &lt;li>)
  - Header >> La clase .dropdown-header se utiliza para agregar un encabezado dentro del menú desplegable (se aplica al &lt;li>)
  - Disable an Item >> Usar la clase .disabled
  - Dropdown Position >> Para alinear a la derecha el dropdown, agregar la clase .dropdown-menu-right al elemento que tenga .dropdown-menu (se alinea a la derecha del contenedor del .dropdown)
  -  Dropdown Accessibility  >> incluir los atributos <code>role</code> y <code>aria-#</code>, al crear un menú desplegable.
    - <code>&lt;ul class="dropdown-menu" role="menu" aria-labelledby="menu1"></code>
    - <code>&lt;li role="presentation"><a role="menuitem" href="#">HTML</a></li></code>
  
*   
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  