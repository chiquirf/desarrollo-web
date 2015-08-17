#HTML interesante a tener en cuenta:

* The lang Attribute &lt;html lang="en-US"> // &lt;html lang="es-ES">
* [HTML data-* Attributes](http://www.w3schools.com/tags/att_global_data.asp) Atributos personalizados para utilizarlos con JS o CSS.
* [HTML tabindex Attribute](http://www.w3schools.com/tags/att_global_tabindex.asp) Especifica el orden de “tab” de uno o varios elementos.
* &lt;header> tag cannot be placed within a &lt;footer>, &lt;address> or another &lt;header> element.
* &lt;b> any extra importance. &lt;strong> added semantic "strong" importance.
* &lt;i> any extra importance. &lt;em> added semantic importance.
* &lt;q> defines a short quotation usually insert quotation marks. &lt;blockquote> defines a quoted section usually indent &lt;blockquote> elements.
* &lt;blockquote cite="http://..."> agregar attr "cite" si es un a cita.
* &lt;abbr title="World Health Organization">WHO&lt;/abbr> abbreviation or an acronym
* &lt;cite> element defines the title of a work
* HTML Description Lists: &lt;dl> tag defines the description list, the &lt;dt> tag defines the term (name), and the &lt;dd> tag describes each term
* Horizontal Lists >>> ul#menu li { display: inline;}
* Block-level Elements: div h1-h6 p form
+ Inline Elements: span a img
* &lt;div>	Defines a section in a document (block-level) // &lt;span>	Defines a section in a document (inline)
* Website Layout Using HTML5
  - header	Defines a header for a document or a section
  - nav	Defines a container for navigation links
  - section	Defines a section in a document
  - article	Defines an independent self-contained article
  - aside	Defines content aside from the content (like a sidebar)
  - footer	Defines a footer for a document or a section
  - details	Defines additional details
  - summary	Defines a heading for the details element
* FORMS - HTML5 
  - &lt;datalist> Element specifies a list of pre-defined options for an &ltinput> element.
  - INPUT HTML TYPES: text, password, submit, radio, checkbox, button, 
  - INPUT HTM5 TYPES: color, date, datetime, datetime-local, email, month, number, range, search, tel, time, url, week
  - Attr *form="idform"* en un input, se puede incluir dentro de un Form (id="form1") un input que esté fuera de la etiqueta form, agregando el atributo *form="form1"*
  - Use simple syntax for linking style sheets (CSS) and for loading external scripts (JS): the type attribute is not necessary.
* HTML5 VIDEO (IE>=9)
  - soporte máximo: .MP4 y .OGG
  - &lt;video width="320" height="240" controls> &lt;source src="movie.mp4" type="video/mp4"> &lt;source src="movie.ogg" type="video/ogg"> Your browser does not support the video tag. &lt;/video>  ...[ver más detalle](http://www.w3schools.com/tags/tag_video.asp) 
* HTML APIs : 
  - Geolocation (HTML Geolocation is used to locate a user's position.)
  - Drag/Drop (Drag and drop is a part of the HTML5 standard.)
  - Local Storage (HTML local storage, better than cookies.)
  - Application Cache (accessible without an internet connection)
  - Web Workers (A web worker is a JavaScript running in the background, without affecting the performance of the page.)
  - Server-Sent Events (Server-Sent Events allow a web page to get updates from a server.)
  