# Tabla de contenido

* [Vocabulario web][1]
* [Html][2]
	* [¿Qué es html?][3]
		* [Historia de html][4]
		* [Sintaxis de html][5]
		* [Estructura de html][6]
	* [Titulos y párrafos][7]
	* [Secciones de contenido (Header, main y footer)][8]
	* [Secciones de contenido (Section, article, aside)][9]
		* [Ejemplo de section dentro de article][10]
	* [Elementos de línea][11]
		* [Ejemplos][12]
	* [Atributos][13]
		* [Atributos globales importantes][14]
		* [Ejemplo][15]
	* [Enlaces][16]
		* [Rutas absolutas y rutas relativas][17]
		* [Atributos de los enlaces][18]
		* [Navegación a través de anclas][19]
	* [Listas][20]
		* [Listas anidadas][21]
		* [Atributos de las listas][22]
	* [Tablas][23]
	* [Otras etiquetas importantes][24]
		* [Etiquetas de bloque][25]
		* [Etiquetas de linea][26]
	* [Formularios][27]
		* [Asociar inputs y label][28]
		* [Input type][29]
			* [Diferencia entre type button y button][30]
			* [Inputs de tipo fecha][31]
			* [Inputs para móviles][32]
		* [Input radio][33]
		* [Input checkbox][34]
		* [Input select][35]
			* [Select basico][36]
			* [Select avanzado][37]
		* [Datalist][38]
		* [Más elementos de formularios][39]
		* [Atributos de los formularios][40]
		* [Get vs post][41]
	* [Contenido embebido][42]
		* [Imágenes][43]
		* [Decive pixel ratio][44]
			* [Atributo srcset][45]
		* [Etiqueta picture][46]
		* [Etiqueta audio][47]
		* [Etiqueta video][48]
		* [Iframes][49]
		* [Etiqueta figure][50]
	* [Etiquetas meta y accesibilidad][51]
		* [Etiquetas meta][52]
		* [Generar y añadir un favicon][53]
		* [Atributos de accesibilidad][54]
	* [Open Graph Protocol][55]
	* [Twitter card][56]

# Vocabulario web

* IP: Es el identificador numérico de una página web, es único y representa la dirección donde está el ordenador que contiene esa página web

* Dominio web / URL: Uniform Resources Locator. Es el nombre asociado a la IP que utilizamos para solicitar recursos, en nuestro caso un sitio web.

* DNS: Domain Name System. Es un servidor cuya principal función es traducir el nombre de dominio a su identificador único.

* Sitio web: Es un conjunto de uno o varios recursos web alojados en el mismo dominio.

* Servidor web: Es un ordenador cuyo objetivo es servir recursos web.

* Hosting: Es el almacenamiento del servidor web. El disco duro donde el servidor guarda los recursos.

* Petición: Es la acción de pedir recursos a un servidor.

# Html

## ¿Qué es html?

* Es un lenguaje de marcado de hipertexto (Hyper Text Markup Language)

* HTML no es un lenguaje de programación, es un lenguaje de estructura.

* Es la base con la que estan creadas todas las páginas web del mundo.

* Cada etiqueta le dice al navegador y alos motores de búsqueda cuál es la estrucutura de los documentos, elementos, organización, etc.

## HIstoria de html

* 1989 - Inicio de su desarollo

* 1991 - Lanzamiento de la web (se basa en 3 conceptos. http, thml y url)
    - http: protocolo que se debe seguir
    (conjunto de normas o reglas) que se debe
    seguir a la hora de transmitir informacion 
    con los documentos a travez de la red.
    - html: lenguaje donde en donde estan escritos todos los sitios web.
    - url: dirección donde estan los sitios web.

* 1992 - Lanzamiento de HTML (Nació de SMGL. Creado por Tim Bernes Lee)

* 1994 - Creación de la W3C ( consorcio que define los estándares de la web)
    - W3C: Se encarga de establecer las normas (lo que esta bien y esta mal) al escribir un     documento html.

* 1998 - HTML4 (versión que más duro de HTML)

* 1999 - HTML 4.1 - XHTML (actualización del estándar HTML4)

* 2004 - Creación de la WHATWG

* 2008 - HTML5 (Lanzado por WHATWG de forma independiente)

* 2014 - Estándar HTML5 (Lanzado por W3C de forma oficial)

[Documentación oficial MDN](https://developer.mozilla.org/es/docs/Web/HTML)

[Enlace oficial W3C](https://www.w3.org/TR/html52/)

## Sintaxis de HTML

```html
<etiqueta> Etiqueta de apertura
    Contenido de la etiqueta
</etiqueta> Etiqueta de cierre
```

* Sintaxis de un comentario en html 

```html
<!--Este es un comentario-->
```

* Los comentarios son para los desarrolladores y no afectan al html

* No todas las etiquetas sirven para poner el mismo tipo de contenido

## Estructura de HTML

[Documentación oficial html](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/html)

[Documentación oficial head](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/head)

[Documentación oficial title](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/title)

[Documentación oficial body](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/body)

```html

<!--Establece el tipo de estandar del documento (HTML5)-->
<!DOCTYPE html> <!--No tiene etiqueta de cierre-->

<!--La etiqueta html representa el inicio del documento HTML--> <!--lang representa el lenguaje de la pagina-->
<html lang="es"></html>

<!--Datos que le pasamos al navegador con información de nuestra página web-->
<head></head>


<!--charset es un set de caracteres para visualizar correctamente los acentos-->
<meta charset="UTF-8"> <!--No tiene etiqueta de cierre-->

<!--Representa el titulo o nombre de la pestaña de la página web-->
<title></title>

<!--Representa todo el contenido de nuestra página web-->
<body></body>
```

## Titulos y párrafos (headings and paragraphs)

[Documentación oficial títulos](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/Elementos_t%C3%ADtulos)

```html
<body>
	<h1>Harry Potter</h1> <!--Titulo principal-->

	<h2>Sinopsis</h2> <!--Subtitulo-->

	<p>Lorem ipsum dolor sit amet consectetur</p> <!--Contenido del subtitulo-->

	<h2>Novelas</h2> <!--Subtitulo-->

	<p>lorem ipsum dolor sit amet consectetur</p> <!--Contenido del subtitulo-->

	<h3>Harry Potter y la Piedra filosofal</h3> <!--Subtitulo dentro del subtitulo-->

	<p>lorem ipsum dolor sit amet consectetur</p> <!--contenido del subtitulo-->

	<h4>Personajes</h4> <!--subtitulo del subtitulo-->

	<p>Lorem</p> <!--contenido del subtitulo-->

	<p>Ipsum</p> <!--contenido del subtitulo-->

	<p>Dolor</p> <!--contenido del subtitulo-->

</body>
```

## Secciones de contenido (Header, main y footer)

[Documentación oficial header](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/header)

[Documentación oficial main](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/main)

[Documentación oficial footer](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/footer)

```html
<body>
	<!--
		<header>
		</header> 

		<main>
		</main> 

	    <footer>
	    </footer>
	-->
	<header> <!--Encabezado-->
		<!--menú de navegación, logo, redes sociales....-->
		Inicio
		Novelas
		Peliculas
		Contacto
	</header>
	<main> <!--Contenido principal-->
		<h1>Harry Potter</h1> <!--Titulo principal-->
		<h2>Sinopsis</h2> <!--Subtitulo-->
		<p>Lorem ipsum dolor sit amet consectetur</p> <!--Contenido del subtitulo-->
		<h2>Novelas</h2> <!--Subtitulo-->
		<p>lorem ipsum dolor sit amet consectetur</p> <!--Contenido del subtitulo-->
	</main>
	<footer> <!--Pie de página-->
		<!--Copyright 2020-2021...-->
	</footer>
</body>
```

## Secciones de contenido (Section, article, aside)

[Documentación oficial section](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/section)

[Documentación oficial article](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/article)

[Documentación oficial aside](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/aside)

* Section: Es un contenedor genérico que agrupa contenido que está relacionado. Cuando creamos bloques cuyo contenido es parte de un bloque total usaremos section.

* Article: Es un contenedor que representa contenido independiente, es decir, podemos leer ese fragmento en cualquier otro sitio y tendria sentido por si mismo.

* Aside: Se utiliza para representar contenido relacionado pero que no forma parte del conenido principal.

* Anidamiento: 
    Un section puede contener articles, por ejemplo, si tenemos varios articulos que hablan sobre etiquetas HTML, deben ir dentro de un section, ya que es un contenido relacionado entre si, y los article serían contenido independiente porque prodríamos leer uno sin haber leido el resto, y seguiria teniendo sentido.
    El article es definido como un componente de la página de contenido independiente, esto implica que esta etiqueta pueda tener un header y un footer propios.

    Tambien existe el caso en el que un article contenga varias secciones, el articulo independiente podria ser navegadores y este contener dentro secciones como "Navegadores más utilizados en 2020"

```html
<body>
	<header>
		<h1>Noticias nacionales</h1>
	</header>
	<aside> <!--Aside que muestra contenido relacionado-->
		Visita esta otra pagina
	</aside>
	<main>
		<section>
			<h2>Section como contenedor</h2>
			<section>
				<h3>Noticias del Día</h4>
				<article>
					<header>
						<h4>Noticia 1</h4>
					</header>
					<p>lorem ipsum dolor sit amet consectetur</p>
					<footer>
						La noticia ocurrio en un lugar del mundo
					</footer>
				</article>
			</section>
		</section>
	</main>	
	<footer>
		06-01-2021
	</footer>
</body>
```

### Ejemplo de section dentro de article

```html
<body>
	<header>
		<h1>Noticias nacionales</h1>
	</header>
	<main>
		<article>
			<h2>Navegadores más utilizados en 2020</h2>
			<section>
				<header>
					<h3>Chrome</h3>
				</header>
				<p>lorem ipsum dolor sit amet consectetur</p>
				<footer>
					Creado por google
				</footer>
			</section>
			</section>
				<header>
					<h3>Firefox</h3>
				</header>
				<p>lorem ipsum dolor sit amet consectetur</p>
				<footer>
					Creado por mozilla
				</footer>
			</section>
		</article>
	<main>
	<footer>
		06-01-2021
	</footer>
</body>
```

## Elementos de línea

[Documentación oficial em](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/em)

[Documentación oficial strong](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/strong)

[Documentación oficial small](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/small)

[Documentación oficial br](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/br)

[Documentación oficial wbr](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/wbr)

[Documentación oficial time](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/time)

[Documentación oficial i](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/i)

[Documentación oficial b](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/b)

[Documentación oficial u](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/u)

* em -> enfasis

* strong -> más enfasis

* small -> menos enfasis que el texto normal

* br -> forzar un salto de linea

* wbr -> salto de linea si hiciera falta

* time -> se usa para representar un contenido de hora/fecha

* i -> italic

* b -> bold

* u -> undeline

* sup -> super-indice

* sub -> sub-indice

### Ejemplos

```html
<em>Soy una etiqueta em</em>

<strong>Soy una etiqueta strong</strong>

<small>Soy una etiqueta small</small>

<p>Soy un parrafo con una etiqueta<br>br para saltos de linea</p>

<time>07 de enero</time>

<i>Soy una etiqueta i</i>

<b>Soy una etiqueta b</b>

<u>Soy una etiqueta u</u>

<p>4 elevado al cuadrado se representa así 4<sup>2</sup></p>

<p>Agua oxigenada tiene la formula H<sub>2</sub>O<sub>2</sub></p>
```

Esto se veria algo así:

<em>Soy una etiqueta em</em>

<strong>Soy una etiqueta strong</strong>

<small>Soy una etiqueta small</small>

<p>Soy un parrafo con una etiqueta<br>br para saltos de linea</p>

<time>07 de enero</time>

<i>Soy una etiqueta i</i>

<b>Soy una etiqueta b</b>

<u>Soy una etiqueta u</u>

<p>4 elevado al cuadrado se representa así 4<sup>2</sup></p>

<p>Agua oxigenada tiene la formula H<sub>2</sub>O<sub>2</sub></p>

## Atributos

[Documentación oficial atributos](https://developer.mozilla.org/es/docs/Web/HTML/Atributos)

Los atributos son valores adicionales que configuran os elementos y/o ajustan su comportamiento.

En terminos generales hay dos tipos de atributos

* Comunes: 
   Su sintaxis es -> atributo="valor"
* Booleanos:
   Su sintaxis es -> atributo

```html
<html lang="es"> <!--lang es un atributo comun y "es" el valor-->

<meta charset="UTF-8"> <!--charset es un atributo comun y "UTF-8" es el valor-->
```

### Atributos globales importantes

Algunos atributos globales que están disponibles para la mayoría de etiquetas en HTML

* class -> Éste atributo se usa para dar estilos a través de css
* id -> Es un identificador único que se utiliza para seleccionar el elemento desde javascript y para hacer navegación a través de anclas
* title -> Es un atributo que ayuda a la accesibilidad mostrando una descripción del elemento al que pertenece. Aparece el mensaje en un tooltip
* data-* -> Es un atributo que nos permite guardar algún valor en la etiqueta HTML

### Ejemplo

```html
<head>
	<style type="text/css">
		.parrafo-1 {
			color: red;
		}
	</style>
</head>
<body>
	<p class="parrafo-1">Clases</p>

	<p id="parrafo">Identificador a través de un ID</p>

	<p title="Este es un ejemplo del atributo title">Titulo con tooltip</p>

	<p id="parrafo-2" data-ejemplo="Datos de ejempplo">Datos pasados en la etiqueta</p>

	<script type="text/javascript">
		const p = document.getElementById('parrafo');
		const parrafo2 = document.getElementById('parrafo-2');

		console.log(p.textContent);
		console.log(parrafo2.dataset.ejemplo);
	</script>
</body>
```

## Enlaces 

[Documentación oficial a](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/a)

* Enlaces: Conocidos también por links popularmente. Su objetivo es conectar una pagina web con ora pagina web, con un recurso tanto interno como externo, o cono otro sitio web.
* Tienen el atributo obligaorio "href", donde le especificamos la ruta del recurso o sitio que queremos obtener.
* Tambien tiene el atributo target, que configura cómo queremos visualizar el recurso o sitio que solicitamos.

se usa el atributo "a" con su atributo obligatorio "href"

```html
<!--Dentro de href va la ruta o url a donde nos queremos dirigir.

Por ejemplo estamos en index.html y tenemos un documento llamado contacto.html lo indicariamos de la siguiente forma-->

<a href="contacto.html">Ir a contacto</a>
```

### Rutas absolutas y rutas relativas

* Rutas absolutas: 
   Tienen un protocolo, http/https y son unicas en la red.
   Se suelen utilizar para rutas externas.

* Rutas relativas:
   Pueden ser relativas al punto donde nos encontramos o relativas a la raíz del proyecto.

   No usan protocolo

   Si el recurso se encuentra al mismo nivel (en la misma carpeta) pondremos unicamente el nombre del archivo.

   Si necesitamos salir de la carpeta actual usaremos ../ y se pone uno por cada nivel (carpeta) de la que queramos salir.

```html
<!--Esto es una ruta absoluta-->
<a href="https://google.com">Ir a google</a>

<!--Esto es una ruta relativa al punto donde nos encontramos-->
<a href="contacto.html">Ir a contacto</a>

<!--Esto es una ruta relativa saliendo de la carpeta actual-->
<a href="../index.html">Ir a inicio</a>
```

### Atributos de los enlaces 

* target: define donde se abrirá el recurso solicitado. Por norma general siempre que usen rutas absolutas pondran como valor "_blank"
   "_self" -> es el valor por defecto (Es como no poner nada)
* download: Atributo booleano, sirve para descargar el rescurso solicitado.
   IMPORTANTE, el recurso debe estar en tu mismo servidor

```html 
<!--Nos envia a google abriendo una pestaña diferente-->
<a href="https://google.com" target="_blank">Ir a google</a>

<!--Nos descarga el archivo contacto.html-->
<a href="contacto.html" download>Descargar</a>
```

### Navegación a través de anclas

Con la etiqueta "a" nos movemos en la pagina por medio de un id puesto en alguna etiqueta

* Se usa "#" para indicar que vamos a poner id

```html
<body>
	<nav>
		<p><a href="#post-1">Post 1</a></p>
		<p><a href="#post-2">Post 2</a></p>
		<p><a href="#post-3">Post 3</a></p>
	</nav>
	<article id="post-1">
		<h1>post 1</h1>
		<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
		tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam</p>
	</article>
	<article id="post-2">
		<h1>post 2</h1>
		<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
		tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam</p>
	</article>
	<article id="post-3">
		<h1>post 3</h1>
		<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
		tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam</p>
	</article>
</body>
```

## Listas

[Documentación oficial li](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/li)

[Documentación oficial ul](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/ul)

[Documentación oficial dl](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/dl)

Las listas en HTML sirven para listar contenido. En función del tipo de contenido de nuestra lista tendremos tres tipos de listas:

* ul -> unordered list: Se utilizan cuando el orden de los elementos no influye (lista de la compra)
* Cada elemento de la lista se representa con la etiqueta "li", tanto en las ul como en las ol ("li" significa list item)

```html
<ul>
	<li>Pan</li>
	<li>Azucar</li>
	<li>Leche</li>
</ul>
```

* ol -> ordered list: Se utiliza cuando el orden de los elementos es importante (top 10)
* Cada elemento de la lista se representa con la etiqueta "li", tanto en las ul como en las ol ("li" significa list item)

```html
<ol>
	<li>HTML</li>
	<li>CSS</li>
	<li>JAVASCRIPT</li>
</ol>
```

* dl -> difinition list: Se utiliza para hacer una lista de definiciones (diccionario)

Cada elemento de una lista de definición lleva 2 etiquetas:

	- dt -> Definition term: El término que vamos a definir
	- dd -> definition descrption: La descripción del término

```html
<dl>
	<dt>HTML</dt>
	<dd>HyperText Markup Language: Es un lenguaje de marcado que se usa para estructurar datos en una página web</dd>

	<dt>CSS</dt>
	<dd>Cascade Style Sheets: Es un lenguaje de diseño que se utiliza para dar estilos al HTML</dd>
	
	<dt>JAVASCRIPT</dt>
	<dd>Es un lenguaje de programación para dar interactividad a un sitio web</dd>
</dl>
```

### Listas anidadas

Se pueden construir listas anidadas teniendo en uno de los li otro ul/ol según sea necesario 

```html
<ol>
	<li>
		HTML
		<ul>
			<li>Estructura</li>
			<li>Sintaxis</li>
			<li>Etiquetas</li>
		</ul>
	</li>
	<li>CSS</li>
	<li>JAVASCRIPT</li>
</ol>
```

### Atributos de las listas

* ol -> 
   type: Estilo de numeración (1, A, a, I, i)
   start: Inicio de las secuencia (un número)

```html
<!--con start con el valor 3 empezara a contar desde el 3-->
<ol type="A" start="3">
	<li>no</li>
</ol>
```

* ul ->
   type: Estilo de los item (disc, square, circle)

```html
<!--disc es el valor por defecto-->
<!--square son cuadrados-->
<!--circle son circulos vacios-->
<ul type="circle">
	<li>si</li>
</ul>
```

## Tablas

[Documentación oficial tablas](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/table)

Las tabalas en HTML sirven para mostrar contenido tabulado.

La estructura básica de una tabla se compone de:

* table -> Etiqueta que encierra una tab^la
* tr -> table row, etiqueta que construye una fila
* td -> table data, etiqueta que contruye una celda

truco: el número de celdas dentro de un td establecerá el número de columnas de la tabla.

Los titulos de las tabalas se establecen con la etiqueta caption, es una etiqueta opcional, y según la espeficicación esa etiqueta se coloca justo después de la etiqueta table

Las cabeceras de las tablas se establecen con la etiqueta thead.
Dentro tendremos una etiqueta tr normal, pero con la etiqueta th en lugar de td

El contenido de la tabla debe ir dentro de una etiqueta tbody para representar el cuerpo de la tabla

De forma opcional podemos colocar un tfoot a la tabla para establecer un pie de tabla, esto es algo que algunas tablas tienen como suma de cantidades o total.

Para hacer que las celdas ocupen más de una fila o más de una columna tenemos 2 atributos:

* rowspan: sirve para que una celda ocupe más de una file, el valor por defecto es 1
* colspan sirve para que una celda ocupe más de una columna, el valor por defecto es 1

Cuando necesitamos seleccionar una columna, tenemos la etiqueta colgroup, que nos permite seleccionar una columna en concreto. Dentro pondremos tantas etiquetas col como columnas tengamos, cada etiqueta col equivaldrá a una columna siguiento el mismo orden que tienen en la tabla

Si necesitamos que una etiqueta col agrupe más de una columna, tenemos el atributo span, qie funciona exactamente igual que rowspan y colspan.

```html
<table>
	<caption>HORARIO DE CLASES</caption>
	<colgroup>
		<col span="5">
		<col>
		<!-- <col>
		<col>
		<col>
		<col> -->
	</colgroup>
	<thead>
		<tr>
			<th></th>
			<th>L</th>
			<th>M</th>
			<th>X</th>
			<th>J</th>
			<th>V</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>8:30 - 9:30</td>
			<td>Matemáticas</td>
			<td>Matemáticas</td>
			<td>Sociales</td>
			<td>Matemáticas</td>
			<td>Matemáticas</td>
		</tr>
		<tr>
			<td>9:30 - 10:25</td>
			<td>Lengua</td>
			<td>Lengua</td>
			<td>Matemáticas</td>
			<td>Ciencias</td>
			<td>Lengua</td>
		</tr>
		<tr>
			<td>10:25 - 11:20</td>
			<td>Educación Física</td>
			<td>Ciencias</td>
			<td>Lengua</td>
			<td>Lengua</td>
			<td>Educación física</td>
		</tr>
		<tr>
			<td>11:20 - 11:45</td>
			<td colspan="5">Recreo</td>
		</tr>
		<tr>
			<td>11:45 - 12:40</td>
			<td>Ingles</td>
			<td>Sociales</td>
			<td>Ingles</td>
			<td>Tutoría</td>
			<td>Ingles</td>
		</tr>
		<tr>
			<td>12:40 - 13:35</td>
			<td rowspan="2">Tecnología</td>
			<td>Educación física</td>
			<td>Plástica</td>
			<td>Religión</td>
			<td rowspan="2">Música</td>
		</tr>
		<tr>
		<td>13:35 - 14:30</td>
			<td>Francés</td>
			<td>Tecnología</td>
			<td>Francés</td>
		</tr>
	</tbody>
	<tfoot>
		<tr>
			<td colspan="5">Total de asignaturas</td>
			<td>12</td>
		</tr>
	</tfoot>
</table>
```

## Otras etiquetas importantes

### Etiquetas de bloque

[Documentación oficial address](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/address)

[Documentación oficial blockquote](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/blockquote)

[Documentación oficial pre](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/pre)

[Documentación oficial https://developer.mozilla.org/es/docs/Web/HTML/Elemento/div](div)

[Documentación oficial hr](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/hr)

* address -> Se utiliza apra aportar información de contacto para el article más cercano o para todo el body

```html
<address>
	Tony Stark
	Malibú 10880
	90265
	California
</address>
```

* blockquote -> Se utiliza para marcar las citas a otros autores o documentos. Se puede incluir el atributo cite para poner un enlace al documento original o fuente

```html
<blockquote cite="https://www.entrepreneur.com/article/312598">
	<p>
		“Hay cosas que nunca le pregunté a mi padre. Hay preguntas que me hubiera gustado hacerle: cómo se sentía por lo que hacía su empresa, si estaba conflictuado, si tenía dudas (…). Vi a jóvenes estadounidenses ser asesinados por las armas que creaba para defenderlos y protegerlos. Me di cuenta que era parte de un sistema que no rinde cuentas”
	</p>
</blockquote>
```

* pre -> Se utiliza para tener código preformateado que necesita ser representado igual que se escribió 

```html
<pre>
	Hola,
	¿que tal?
</pre>
```

* div -> Se sua como división del documento, semánticamente no significa nada, es un contenedor genérico que se usa generalmente para dar estilo a través de css o para usar algo denominado "delegación de eventos" en javascript

```html
<div>
	<h2>Usuario</h2>
	<p>email</p>
	<p>Descripción</p>
</div>
```

* hr -> horizontal rule, se utiliza para decirle al navegador que vamos a cambiar de tema 

```html
<hr> <!--Se representa como una linea pero no es para dibujar lineas, sirve para cambiar de tema-->
```

### Etiquetas de linea

[Documentación oficial span](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/span)

[Documentación oficial q](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/q)

[Documentación oficial code](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/code)

[Entidades especiales html](https://ascii.cl/es/codigos-html.htm)

* span -> Es un contenedor de línea, equivalente a div, se suele usar para encerrar palabras o pequeños textos y darles estilo a través de css o localizarlos desde javascript, Semánticamente no significan nada

```html
<p>Lorem ipsum dolor <span>sit amet, consectetur</span> adipisicing elit, sed do eiusmod tempor incididunt</p>
```

* q -> Es el equivalente a blockquote, significa quote, por eso el de bloque se llama block - quote. Sirve para poner citas pero en linea.

```html
<q cite="">Yo soy Iron Man</q>
```

* code -> Sirve para encerrar código que queremos representar visualmente, suele ir unido con la etiqueta pre.

```html
<pre>
	<code>
		span {
			color: red; 
		}
	</code>
</pre>
```

* Entidades especiales en HTML - Código ADCII
https://ascii.cl/es/codigos-html.htm

```html
<p>La etiqueta <code>&#60;h1&#62;</code> se utiliza para representar títulos de primer nivel</p>

<!--Símbolo de copyright-->
&copy;
```

## Formularios

[Documentación oficial form](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/form)

[Documentación oficial label](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/label)

[Documentación oficial input](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/input)

[Documentación oficial button](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/button)

La estructura básica de un formulario se compone de de 4 elementos

* form -> Es la etiqueta que engloba nuestro formulario
* label -> Sirve para escribir el nombre del campo a rellenar,
debe de tener el atributo for al cual se le indica un id que lo que hará será emparejar el label con su input correspondiente
* input -> Sirve para crear un campo que permitirá al usuario interactuar. El único atributo obligatorio del input es name
* button -> crea un botón que permitirá enviar el formulario

```html
<form>
	<label>Nombre</label>
	<input>
	<button>Enviar formulario</button>
</form>
```

### Asociar inputs y label

Hay dos maneras para asociar un input con un label

```html
<form>
	<label for="name">Nombre</label>
	<input id="name">
	<button>Enviar formulario</button>
</form>
```
y la segunda forma es:

```
<form>
	<label>
		Nombre
		<input>
	</label>
	<button>Enviar formulario</button>
</form>
```

### input type:

* hidden -> Campo oculto, puede contener valor pero no se mostrará 

#### Diferencia entre type button y button

* button -> Se comporta igual que un <button>, visualmente es igual, pero el formulario no se enviará
* submit -> Se utiliza para enviar el formulario

```html
<form>
	<input>
	<input type="button" value="Envíar input"> <!--No sirve para enviar el formulario-->
	<input type="submit" value="Envíar formulario"> <!--Sirve para enviar el formulario igual que <button>-->  
	<button>Envíar</button>
</form>
```

#### Inputs de tipo fecha

* date -> Se utiliza para introducir una fecha
* datetime -> obsoleto
* datetime-local -> fecha y hora, no funciona en firefox
* time -> Se utiliza para introducir una hora
	- TIP
	Se recomienda usar datetime-local y time para seleccionar fecha y hora
* month -> Se utiliza para introducir un mes
* week -> Se utiliza para introducir el número de semana del año 

```html
<form>
	<input type="date">
	<input type="datetime-local"> <!--No funciona en firefox-->
	<input type="date">
	<input type="time">
	<input type="month">
	<input type="week">
</form>
```

#### Inputs para móviles

* email -> Se utiliza para introducir un email
* password -> Se utiliza para contraseñas 
* tel -> Se utiliza para introducir números telefónicos
* search -> Se utiliza para las barras de búsqueda
* url -> Se utiliza para introducir URLs

```html
<form>
	<label> search
		<input type="search">
	</label>
	<label> teléfono
		<input type="tel">
	</label>
	<label> email
		<input type="email">
	</label>
	<label> password
		<input type="password">
	</label>
	<label> url
		<input type="url">
	</label>
</form>
```

* color -> Se utiliza para especificar un color
* number -> Se utiliza para valores numéricos
* range -> Se utiliza para establecer un rango
* reset -> Se utiliza para resetear el formulario
* text -> valor por defecto

```html
<input type="color">
<input type="number">
<input type="text">
<input type="range" step="5" min="0" max="20">
<input type="reset">
```

### Input radio

* radio -> Permite seleccionar una única opción de una lista de opciones relacionadas

```html
<h1>Elementos seleccionables</h1>
<form>
	<h2>Género</h2>
	<label>Masculino
		<input type="radio" name="gender" value="masculino" checked>
	</label>
	<label>Femenino
		<input type="radio" name="gender" value="femenino">
	</label>
	<label>Desconocido
		<input type="radio" name="gender" value="desconocido">
	</label>
</form>
```

### Input checkbox

* checkbox -> Permite seleccionar varias opciones de una lista de opciones relacionadas

```html
<form>
	<h1>Lenguajes que conoces</h1>
	<label>HTML
		<input type="checkbox" name="languages" value="html" checked>
	</label>
	<label>CSS
		<input type="checkbox" name="languages" value="css">
	</label>
	<label>JAVASCRIPT
		<input type="checkbox" name="languages" value="javascript">
	</label>
</form>
```

### Input select

* select -> Crea una lista de opciones donde podemos seleccionar una o varias opciones

Cada opción irá dentro de una etiqueta <option></option>

#### Select basico

```html
<form>
	<h1>Elementos seleccionables</h1>
	<select name="lenguajes" multiple>
		<option value="html">HTML</option>
		<option value="css">CSS</option>
		<option value="javascript">JAVASCRIPT</option>
	</select>
</form>
```

#### Select avanzado

Si tenemos muchas opciones podemos ordenarlas por categorías a través de la etiqueta <optgroup></optgroup> con el atributo label para nombrar la categoría

```html
<form>
	<select name="mascotas">
		<optgroup label="4 patas">
			<option value="perro">Perro</option>
			<option value="gato">Gato</option>
			<option value="hamster">Hamster</option>
			<option value="conejo">Conejo</option>
		</optgroup>
		<optgroup label="aves">
			<option value="loro">Loro</option>
			<option value="canario">Canario</option>
		</optgroup>
		<optgroup label="otras">
			<option value="serpiente">Serpiente</option>
			<option value="tarantula">Tarántula</option>
		</optgroup>
	</select>
</form>
```

### Datalist

```html
<form>
	<input type="list" list="pets">
	<datalist id="pets">
		<option value="perro"></option>
		<option value="gato"></option>
		<option value="hamster"></option>
		<option value="conejo"></option>	
		<option value="loro"></option>
		<option value="canario"></option>
		<option value="serpiente"></option>
		<option value="tarantula"></option>
	</datalist>
</form>
```

### Más elementos de formularios

* fieldset -> Se utiliza para agrupar elementos dentro de un formulario
* legend -> Rperesenta una etiqueta para el contenido del fielset

```html
<form>
	<fieldset>
		<legend>Datos Personales</legend>
		<label for="name">Nombre</label>
		<input type="text" id="name">
		<label for="surname"></label>
		<input type="text" id="surname">
	</fieldset>
</form>
```

* file -> Este input se utilliza para cargar archivos y enviarlos desde un formulario

```html
<form>
	<input type="file">
</form>
```

* meter -> Representa un valor dentro de un rango conocido

```html
<form>
	<label for="fuel">Combustible</label>
	<meter 
		id="fuel" 
		min="0" 
		max="100" 
		value="50" 
		low="30" 
		high="70" 
		optimum="50"
	></meter>
</form>
```

* progress -> Representa el proceso de una tarea

```html
<form>
	<label for="task">Tarea 1</label>
	<progress id="task" value="10" max="100">
</form>
```

* textarea -> Se utiliza para introducir texto en un formulario

```html
<form>
	<label for="message">Mensaje</label>
	<textarea name="" id="message" cols="30" rows="10"></textarea>
</form>
```

### Atributos de los formularios

* placeholder -> Da una pista de lo que el usuario tiene que introducir

```html
<input type="text" placeholder="Introduce tu nombre">
```

* required -> Hace que un campo sea obligatorio

```html
<input type="text" required>
```

* readonly -> Hace que un campo sea de solo lectura

```html
<input type="text" value="hola" readonly="">
```

* disabled -> Desactiva el campo, no se podrá escribir en el autofocus

```html
<input type="text" value="hola" disabled="">
```

* min - max -> Establece el minimo y máximo de caracteres de un campo numerico

```html
<input type="number" min="5" max="10">
```

* minlenght - maxlenght -> Establece el minimo y máximo de caracteres de un campo de texto

```html
<input type="text" minlength="3" maxlength="5" required="">
```

* selected -> Equivale a checked en los select, sirve para establecer una opción por defecto

```
<select name="numbers">
	<option value="one">One</option>
	<option value="two" selected>Two</option>
</select>
```

autofocus -> Para poner el foco por defecto al cargar el formulario

```html
<input type="text" autofocus>
```

### Get vs post

Información que servira despues para javascript (?)

```html
<!--
	GET es el metodo por defecto al entrar en toda página

	POST es como enviar el formulario por la parte de atras de la página
-->
<form action="enviar.html" method="POST">
	<label for="name">Nombre</label>
	<input type="text" id="name" name="name">
	<label for="surname">Apellido</label>
	<input type="text" id="surname" name="surname">
	<input type="submit">
</form>
```

## Contenido embebido

[Documentación oficial webp](https://developers.google.com/speed/webp)

[Conversor de imágenes a webp](https://imagen.online-convert.com/es/convertir-a-webp)

* El contenido embebido es todo el contenido que nos traemos desde fuera

* Estos archivos son los que más peso (tamaño) añaden a un sitio web

* Los más conocidos son:
   - Imágenes
   - Audio
   - Vídeo
   - Iframes

### Imágenes 

* Los formatos de imágenes para web los podemos clasificar en 2 tipos
   - Vectoriales
      * svg (recomendado siempre que se pueda)
   - Mapa de bits
      * jpg
      * png 8 y 24 (si necesitas transparencias)
      * gif (si necesitas una imagen animada)
      * webp (el formato que menos pesa)

#### Insertar imágenes en el HTML

[Documentación oficial img](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/img)

```html
<body>
	<h1>Contenido embebido</h1>
	<!--src que es la ruta donde esta la imagen-->
	<!--alt es para en caso de que no carge la imagen o de que alguien use un lector de pantalla-->
	<img src="imagen.jpg" alt="imagen">
</body>
```

### Device pixel ratio

[Página para comprobar tu viewport](https://whatismyviewport.com/)

DPR (Device Pixel ratio):

Es la relación que existe entre los píxeles reales que tiene el dispositivo y los píxeles que tenemos disponibles para "pintar" contenido

DPR = pixeles reales / pixeles disponibles

#### Atributo srcset

[Documentación oficial Imágenes adaptables](https://developer.mozilla.org/es/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)

```
<!-- 3x, 2x, 1x, etc. Es el dpr del dispositivo -->
<img srcset="
img/imagen-desktop.webp,
img/imagen-desktop.jpg, 
img/imagen-mobile.webp 2x,
img/imagen-mobile.jpg 2x" 
src="img/imagen-desktop.jpg" alt="dea"> 
<!-- Usamos src como emergencia por si usamos un navegador viejo como internet explorer que no soporta webp ni srcset -->
``` 

#### Etiqueta picture (Experimental)

[Documentación oficial picture](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/picture)

Otra forma de poner imagenes y lo soportan todos los navegadores principales menos IE

```html
<picture>
	<!-- En source va la imagen para el otro dispositivo con copia de seguirdad y media le indica el tamaño en el que cambiara -->
	<!-- Igual soporta usar 3x, 2x, etc. -->
	<source srcset="
		img/imagen-mobile.webp,
		img/imagen-mobile.jpg" 
		media="(max-width: 1200px)"
	>
	<!-- Es importante poner el img si no no funciona -->
	<img src="img/imagen.jpg" alt="">
</picture>
```

### Etiqueta audio

[Documentación oficial audio](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/audio)

```html
<!-- controls es para que nos salga en la pagina el audio si no no se muestra -->
<!-- los navegadores pueden desactivar autoplay automaticamente -->
<!-- muted hace que sirva el autoplay pero en muted como en instagram -->
<!-- loop es para que se reproduzca de nuevo cuando termine -->
<audio src="audio/si.mp3" controls autoplay muted loop></audio>
```

### Etiqueta video

[Documentación oficial video](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/video)

```html
<!-- controls es para que nos salga en la pagina el audio si no no se muestra -->
<!-- los navegadores pueden desactivar autoplay automaticamente -->
<!-- muted hace que sirva el autoplay pero en muted como en instagram -->
<!-- loop es para que se reproduzca de nuevo cuando termine -->
<!-- poster es para darle una miniatura al video, pero con el autoplay no se puede ver la miniatura -->
<video src="video/dea.mp4" controls autoplay muted loop poster="img/ola.jpg"></video>
```

### Iframes

[Documentación oficial iframe](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/iframe)

Funciona para añadir cosas (como video) de sitios externos (youtube, facebook, instragram, spotify, etc)

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/v0NgKhTz75A" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

No es buena idea usar muchos iframes porque relentizan mucho la página 

### Etiqueta figure

[Documentación oficial figure](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/figure)

Sirve para meter contenido relacionado pero que es opcional que este, si lo quitamos el contenido de la página sigue teniendo sentido

```html
<body>
	<h1>Gatos</h1>
	<p>Lorem ipsum dolor sit, amet consectetur adipisicing, elit. Suscipit exercitationem, delectus expedita quisquam hic, aliquam?</p>
	<p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Assumenda, voluptatum!</p>

	<!-- No afecta si esta o no -->
	<!-- No solo puede usar imagenes, puede usar tablas, imagenes, fragmentos de codigo, etc. -->
	<figure>
		<img src="foto-de-gato.png" alt="gato deah">
		<figcaption>Gato común</figcaption> <!-- Es opcional para dar una descripción a la imagen -->
	</figure>

	<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum, mollitia.</p>
</body>
```

figure se utiliza siempre que se quiera romper el curso del contenido con un contenido relacionado pero que no es necesario para interpretación del articulo

## Etiquetas meta y accesibilidad 

### Etiquetas meta

[Documentación oficial meta](https://developer.mozilla.org/es/docs/Web/HTML/Elemento/meta)

La mayoria de las etiqueta meta tienen un atributo name y uno content

```html
<!-- Es la descripción que aparece al encontrar la pagina en google -->
<meta name="description" content="Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod">

<!-- Menciona quien es el dueño de la pagina al encontrar la pagina en google -->
<meta name="author" content="Dueño de la web">

<!-- Sirve para la codificación de caracteres -->
<meta charset="UTF-8">

<!-- Sirve para adaptar mejor el sitio web a celular -->
<meta name="viewport" content="width-device-width, initial-scale=1.0">
```

### Generar y añadir un favicon

[Documentación oficial favicon](https://developer.mozilla.org/es/docs/Learn/HTML/Introduccion_a_HTML/Metados_en#agregar_iconos_personalizados_a_tu_sitio)

Crearemos nuestros favicons en la pagina https://www.favicon-generator.org/

Ahí generaremos iconos para la web, android, microsoft, and iOS Apps, una ves generado descargaremos los favicon generados y los guardaremos en el proyecto y dentro de la etiqueta <head></head> copiaremos los links que nos da la página:

```html
<head>
	<link rel="apple-touch-icon" sizes="57x57" href="/apple-icon-57x57.png">
	<link rel="apple-touch-icon" sizes="60x60" href="/apple-icon-60x60.png">
	<link rel="apple-touch-icon" sizes="72x72" href="/apple-icon-72x72.png">
	<link rel="apple-touch-icon" sizes="76x76" href="/apple-icon-76x76.png">
	<link rel="apple-touch-icon" sizes="114x114" href="/apple-icon-114x114.png">
	<link rel="apple-touch-icon" sizes="120x120" href="/apple-icon-120x120.png">
	<link rel="apple-touch-icon" sizes="144x144" href="/apple-icon-144x144.png">
	<link rel="apple-touch-icon" sizes="152x152" href="/apple-icon-152x152.png">
	<link rel="apple-touch-icon" sizes="180x180" href="/apple-icon-180x180.png">
	<link rel="icon" type="image/png" sizes="192x192"  href="/android-icon-192x192.png">
	<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
	<link rel="icon" type="image/png" sizes="96x96" href="/favicon-96x96.png">
	<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
	<link rel="manifest" href="/manifest.json">
	<meta name="msapplication-TileColor" content="#ffffff">
	<meta name="msapplication-TileImage" content="/ms-icon-144x144.png">
	<meta name="theme-color" content="#ffffff">
</head>
```

### Atributos de accesibilidad

[Documentación oficial accesibilidad w3c](https://www.w3.org/TR/wai-aria-practices-1.1/)

[Documentación oficial accesibilidad mdn](https://developer.mozilla.org/es/docs/Web/Accessibility/ARIA)

[Documentación oficial accesibilidad google](https://developers.google.com/web/fundamentals/accessibility/semantics-aria)

[Post sobre ARIA](https://www.lullabot.com/articles/what-heck-aria-beginners-guide-aria-accessibility)


```html
<body>
	<!-- Sirve para movernos pulsando el tabulador y sirve tambien para personas que ocupan un navegador por voz -->
	<p tabindex="1">Lorem, ipsum.</p>
	<p tabindex="2">Lorem, ipsum.</p>
	<p tabindex="3">Lorem, ipsum.</p>
</body>
```

```html
<body>
	<!-- aria-label da mas información al navegador por voz -->
	<!-- role da infomación sobre lo que es lo pulsado -->
	<a href="#" role="link" aria-label="Leer más sobre la noticia de si dea">Leer más</a>
</body>
```

## Open Graph Protocol

[Documentación de Open Graph Protocol](https://ogp.me/)

A menudo cuando queremos compartir un enlace en las redes nos topamos con el problema de que las imágenes no se muestran como deberían, o la descripción no se ajusta al contenido del enlace.

Open Graph es el protocolo que nace para poder compartir enlaces de una manera adecuada principalmente en Facebook, aunque muchas de sus características también funcionan para Google+ y Twitter.

¿Cómo funciona Open Graph?
Se trata simplemente de una serie de meta-datos que se podrán incluir en el <head> del código fuente de nuestra web. Dentro de este código le podremos especificar las características del enlace u objeto que querremos compartir: título, tipo de contenido, url, idioma e imagen, entre otras cosas.

Este protocolo que fue creado originalmente por Facebook cuenta con una documentación muy completa que está disponible en la web oficial del Open Graph Protocol.

De la larga serie de propiedades que nos da el protocolo sólo tres son indispensables: og:type, og:image y og:url. El resto lo decidiremos en base a nuestras necesidades.

Existen además plugins de WordPress que ya tienen implementado el protocolo. Instalando estos plugins nuestras páginas ya estarán preparadas para ser compartidas en las redes.

## Twitter card

Es parecido al Open Graph Protocol pero exclusivo para twitter

[Documentación de Twitter card](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/abouts-cards)

Las Twitter Cards o tarjetas de twitter son un formato enriquecido para los tweets, que permite a modo vista previa mostrar información multimedia del mismo con título, resumen, autor e imagen, lo que lo hace más atractivo a la vista del usuario.

Existen varios formatos de Twitter Cards según las necesidades, hoy en día hay seis disponibles: resumen, producto, foto, resumen con imagen grande, reproductor y app:

Las Twitter Cards no sólo hacen más atractivo el tweet, sino que favorecen el branding de la marca que lanza el tweet ya que le da mayor visibilidad, y es visible tanto en formato escritorio como en formato móvil.

[1]: #vocabulario-web
[2]: #html
[3]: #que-es-html
[4]: #historia-de-html
[5]: #sintaxis-de-html
[6]: #estructura-de-html
[7]: #titulos-y-parrafos-headings-and-paragraphs
[8]: #secciones-de-contenido-header-main-y-footer
[9]: #secciones-de-contenido-section-article-aside
[10]: #ejemplos-de-section-dentro-de-article
[11]: #elementos-de-linea
[12]: #ejemplos
[13]: #atributos
[14]: #atributos-globales-importantes
[15]: #ejemplo
[16]: #enlaces
[17]: #rutas-absolutas-y-rutas-relativas
[18]: #atributos-de-los-enlaces
[19]: #navegacion-a-traves-de-anclas
[20]: #listas
[21]: #listas-anidadas
[22]: #atributos-de-las-listas
[23]: #tablas
[24]: #otras-etiquetas-importantes
[25]: #etiquetas-de-bloque
[26]: #etiquetas-de-linea
[27]: #formularios
[28]: #asociar-inputs-y-label
[29]: #input-type
[30]: #diferencia-entre-type-button-y-button
[31]: #inputs-de-tipo-fecha
[32]: #inputs-para-moviles
[33]: #input-radio
[34]: #input-checkbox
[35]: #input-select
[36]: #select-basico
[37]: #select-avanzado
[38]: #datalist
[39]: #mas-elementos-de-formularios
[40]: #atributos-de-los-formularios
[41]: #get-vs-post
[42]: #contenido-embebido
[43]: #imagenes
[44]: #decive-pixel-ratio
[45]: #atributo-srcset
[46]: #etiqueta-picture
[47]: #etiqueta-audio
[48]: #etiqueta-video
[49]: #iframes
[50]: #etiqueta-figure
[51]: #etiquetas-meta-y-accesibilidad
[52]: #etiquetas-meta
[53]: #generar-y-añadir-un-favicon
[54]: #atributos-de-accesibilidad
[55]: #open-graph-protocol
[56]: #twitter-card