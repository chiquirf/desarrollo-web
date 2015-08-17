#RESPONSIVE WEB DESIGN


Otro enlace de interés: [responsivedesign.is](https://responsivedesign.is/)

* Esquemas
  - Diseños para la mejor experiencia para todos los usuarios: [ver esquema típico](http://www.w3schools.com/css/css_rwd_intro.asp)
* Viewport
  - <meta name="viewport" content="width=device-width, initial-scale=1.0">
* Grid-View
  - Trabajar siempre con un grid, manual o usando un framewok para el Grid, por ejemplo: [columnal.com](http://www.columnal.com/)
  - Manual:
    1) * { box-sizing: border-box; }
	2) usuar porcentajes en los width creando estilos con num columnas y porcentajes: .col-1 {width: 8.33%;} .col-2 {width: 16.66%;} ..... .col-9 {width: 75%;} .col-10 {width: 83.33%;} .col-11 {width: 91.66%;}
.col-12 {width: 100%;}
	3) contener todos las columnas en un fila (.row) y limpiar el float agregando >> .row:after { content: ""; clear: both; display: block; }
* Media Queries (IE>9)
  - @media not|only mediatype and (media feature) { CSS-Code; } /// &ltlink rel="stylesheet" media="mediatype and|not|only (media feature)" href="mystylesheet.css">
  - mediatype (más usuados): all print screen speech
  - media feature (los más usados): aspect-ratio [max-min]-width [max-min]-height [max-min]-device-height [max-min]-device-width orientation=(landscape|portrait)
  - @media only screen and (max-width: 500px)  >> cuando screen es menor a 500px.
  - @media only screen and (min-width: 768px)  >> cuando screen es mayor a 768px.
* Images
  - ancho a 100% (usar max-width o width) >>> img {max-width: 100%; height: auto;} para que se escale pero nunca superaa el tamaño original.
  - background-size: contain | 100% 100% | cover >>> usar según sea necesario.
  - utilizar diferentes imágenes para diferentes dispositivos  >>> @media only screen and (min-device-width: 400px)
* Videos (HTMLTag "video" IE>9)
  - ancho a 100% (usar max-width o width) >>> img {max-width: 100%; height: auto;} para que se escale pero nunca superaa el tamaño original.
* Frameworks: Utilizarlos para escribir el código más rápido: BOOTSTRAP

