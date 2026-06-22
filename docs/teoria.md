# INDICE GENERAL: MANUAL DE DESARROLLO WEB DESDE CERO

## BLOQUE I: HTML - El Esqueleto y la Estructura Web

- **Capítulo 1:** Introducción al Lenguaje de Marcado y ¿Qué significa HTML?
- **Capítulo 2:** Anatomía de una Etiqueta y la Estructura Base de un Documento (`<!DOCTYPE>`, `head`, `body`).
- **Capítulo 3:** Etiquetas Semánticas y Estructurales (`header`, `nav`, `section`, `footer`, `div`).
- **Capítulo 4:** Elementos de Contenido, Texto y Listas (`h1`-`h6`, `p`, `ul`, `li`).
- **Capítulo 5:** Enlaces, Multimedia y Botones (`<a>`, `<img>`, `<button>`).
- **Capítulo 6:** Atributos Esenciales: Identificadores, Categorías y Datos Ocultos (`id`, `class`, `data-*`).
- **Capítulo 7:** Estructuras Avanzadas de Interfaz (Formularios, Tablas y Controles del Campus).

---

## BLOQUE II: CSS - El Diseño, Estilo y Maquetación

- **Capítulo 8:** Introducción a las Hojas de Estilo: ¿Qué es CSS y cómo se vincula al HTML?
- **Capítulo 9:** Selectores Básicos (Etiqueta, Clase e ID) y la Regla de la Cascada.
- **Capítulo 10:** El Modelo de Cajas (Box Model): Márgenes, Bordes, Rellenos y Dimensiones (`margin`, `padding`, `border`, `width`, `height`).
- **Capítulo 11:** Colores, Fondos y Degradados (Sólidos, Opacidad y Filtros Visuales).
- **Capítulo 12:** Posicionamiento y Control de Desbordes (`position: absolute/relative`, `overflow`, `z-index`).
- **Capítulo 13:** Maquetación Moderna I: Flexbox (Ejes, Alineación y Distribución del Espacio).
- **Capítulo 14:** Maquetación Moderna II: CSS Grid (Grillas, Columnas y Filas).
- **Capítulo 15:** Estados, Pseudoclases y Transiciones (`:hover`, `:active`, cambios de estado visual).
- **Capítulo 16:** Animaciones CSS nativas y Fotogramas Clave (`@keyframes`).

---

## BLOQUE III: JAVASCRIPT - La Lógica y la Interactividad

- **Capítulo 17:** Introducción a JavaScript: Variables, Tipos de Datos y Operadores Básicos.
- **Capítulo 18:** Control de Flujo: Condicionales (`if/else`), el Atajo Ternario (`? :`) y Bucles (`for`, `while`).
- **Capítulo 19:** Funciones y Modularidad: Cómo encapsular lógica y retornar datos útiles.
- **Capítulo 20:** El DOM (Document Object Model): Cómo capturar y modificar elementos HTML en tiempo real.
- **Capítulo 21:** Escucha de Eventos y Ciclo de Vida (`addEventListener`, clics, cambios de entrada).
- **Capítulo 22:** Estructuras de Datos Avanzadas: Objetos y Arrays de Productos.
- **Capítulo 23:** Métodos Modernos de Arrays para Procesamiento (Iterar, Buscar, Filtrar y Acumular).
- **Capítulo 24:** Persistencia de Datos: Memoria local (`localStorage`) y Traducción de Datos (`JSON.parse/stringify`).
- **Capítulo 25:** Temporizadores y Dinámicas de Interfaz (`setTimeout`, alertas temporales y efectos dinámicos).

---

---

## BLOQUE I: HTML - El Esqueleto y la Estructura Web

### Capítulo 1: Introducción al Lenguaje de Marcado y ¿Qué significa HTML?

#### 1.1 Definición Técnico-Estructural

HTML es el acrónimo de HyperText Markup Language (Lenguaje de Marcado de Hipertexto).

- Lo que NO es: Es fundamental comprender que HTML no es un lenguaje de programación, ya que no maneja lógica condicional, bucles ni operaciones matemáticas.
- Lo que SÍ es: Es un lenguaje de marcado basado en etiquetas que define de manera estricta la estructura semántica y el esqueleto de un documento web. Actúa como los planos de una casa, determinando dónde se ubican los muros, las puertas y las ventanas, pero sin definir su color o sus funcionalidades dinámicas.

---

#### 1.2 El Concepto de Hipertexto y Marcado

El funcionamiento de la web moderna se sostiene sobre dos pilares conceptuales dentro de este lenguaje:

- Hipertexto: Es un sistema de organización de la información que permite enlazar fragmentos de texto, documentos o recursos multimedia entre sí. Esto rompe la lectura lineal tradicional, permitiendo que el usuario navegue de un documento a otro de forma interactiva mediante hipervínculos (enlaces).
- Marcado: Consiste en el uso de códigos especiales (etiquetas) que se añaden al texto plano para "marcarlo" o indicarle al navegador web qué tipo de elemento representa cada fragmento (un título, un párrafo, una imagen, etc.). El navegador lee estas marcas, las procesa en memoria y renderiza la interfaz visual para el usuario.

---

#### 1.3 Historia Breve y la Evolución hacia HTML5

El lenguaje fue concebido originalmente en 1989 por el científico Tim Berners-Lee en el CERN, con el objetivo de permitir a los investigadores compartir documentos científicos de forma remota.

- HTML 1.0 a 4.01: Las primeras versiones se enfocaban exclusivamente en documentos de texto con enlaces básicos. Con el crecimiento de la web, se empezaron a usar tablas y etiquetas obsoletas para diseñar visualmente, lo que volvía al código pesado y desorganizado.
- La Revolución de HTML5: Lanzado oficialmente como estándar moderno, HTML5 cambió el desarrollo web por completo. No solo introdujo etiquetas semánticas nativas para organizar las páginas limpiamente, sino que incorporó soporte directo para audio, video, gráficos avanzados y APIs que permiten crear aplicaciones web interactivas y adaptables a dispositivos móviles sin depender de complementos externos de terceros.

---

### Capítulo 2: Anatomía de una Etiqueta y la Estructura Base de un Documento

#### 2.1 Anatomía de una Etiqueta HTML

Para estructurar un documento, HTML utiliza elementos que, en su gran mayoría, se componen de una etiqueta de apertura y una etiqueta de cierre. La sintaxis estándar se define de la siguiente manera:

- Esquema básico: <etiqueta atributo="valor">Contenido del elemento</etiqueta>

- Etiqueta de apertura (<etiqueta>): Delimita el inicio del elemento e indica al navegador cómo debe interpretar el contenido subsiguiente. Es el contenedor donde se declaran los atributos.
- Atributos (atributo="valor"): Propiedades adicionales que modifican el comportamiento o proveen metadatos al elemento. Se componen de un par clave/valor.
- Contenido: El texto, datos o incluso otros elementos HTML secundarios (etiquetas anidadas) que se encuentran dentro del elemento.
- Etiqueta de cierre (</etiqueta>): Indica la finalización del elemento mediante la inclusión de una barra diagonal (/) antes del nombre de la etiqueta.

##### Elementos Vacíos o Autoconclusivos

Existen excepciones en la sintaxis donde ciertos elementos no contienen texto ni encierran a otros componentes. Estas etiquetas carecen de una etiqueta de cierre independiente y se denominan elementos vacíos (void elements). Un ejemplo crítico en tu proyecto es la etiqueta multimedia para imágenes:

- Ejemplo de imagen: <img src="img/PuertaAluminioConRaja.jpeg" alt="Puerta de Aluminio">

---

#### 2.2 Estructura Base Obligatoria de un Documento HTML5

Cualquier documento HTML válido debe respetar una jerarquía y un orden estructural estricto para que el motor de renderizado del navegador lo procese correctamente. A continuación, se detalla la plantilla base utilizada en el desarrollo profesional:

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aberturas Programacion 1 - Carrito</title>
    <link rel="icon" href="img/logoAberturas.png" type="image/png">
    <link rel="stylesheet" href="css/style.css">
</head>
<body>

    </body>

</html>

---

#### 2.3 Desglose Técnico de los Componentes Base

##### A) La declaración <!DOCTYPE html>

No es una etiqueta HTML propiamente dicha, sino una instrucción al navegador. Define que el documento actual está escrito bajo el estándar de HTML5. Su omisión obliga al navegador a entrar en "Modo de compatibilidad" (Quirks Mode), interpretando el código bajo reglas obsoletas que rompen la maquetación moderna.

##### B) El elemento raíz <html lang="es">

Representa la raíz de todo el documento. Encapsula absolutamente todo el código (excepto el DOCTYPE). El atributo lang="es" especifica el idioma principal del contenido; esto es vital para la accesibilidad (lectores de pantalla) y para que los motores de búsqueda indexen correctamente la página.

##### C) La cabecera del documento <head>

Funciona como el contenedor de los metadatos de la aplicación. El contenido dentro de <head> no se renderiza en el área visible de la página web. Sus etiquetas indispensables son:

- <meta charset="UTF-8">: Define la codificación de caracteres universal. Garantiza la correcta visualización de caracteres especiales, tildes y la letra "ñ".
- <meta name="viewport" content="width=device-width, initial-scale=1.0">: Configura la ventana gráfica. Es obligatoria para asegurar que el diseño sea adaptable (Responsive Design) en dispositivos móviles y tablets.
- <title>: Establece el título del documento que se despliega en la pestaña del navegador y en los resultados de búsqueda.
- <link>: Se utiliza para vincular recursos externos. En tu proyecto, se emplea para conectar el archivo de estilos CSS (css/style.css) y el icono de la pestaña (favicon).

##### D) El cuerpo del documento <body>

Contiene todos los elementos que componen la interfaz de usuario perceptible (textos, estructuras, imágenes, formularios y componentes interactivos). El navegador procesa secuencialmente los elementos declarados dentro de este bloque para construir la representación visual final en la pantalla.

---

### Capítulo 3: Etiquetas Semánticas y Estructurales

#### 3.1 ¿Qué es la Semántica en HTML?

En las primeras versiones de HTML, la maquetación de una página se realizaba utilizando casi exclusivamente la etiqueta genérica <div> para agrupar elementos. Esto provocaba que los navegadores y los motores de búsqueda vieran un documento compuesto por cientos de "cajas" idénticas, sin poder distinguir cuál era el menú, cuál el contenido principal o cuál el pie de página.

Con la llegada de HTML5, se introdujeron las etiquetas semánticas. Una etiqueta es semántica cuando su propio nombre describe el significado y el propósito del contenido que encierra.

##### Ventajas de la semántica:

- Accesibilidad: Permite que los lectores de pantalla utilizados por personas con discapacidad visual entiendan la estructura del sitio y naveguen de forma eficiente.
- SEO (Search Engine Optimization): Facilita que los motores de búsqueda de Internet indexen e identifiquen rápidamente la información valiosa de la web.
- Mantenibilidad: El código fuente es mucho más limpio, legible y profesional para el equipo de desarrollo.

---

#### 3.2 Desglose de Etiquetas Semánticas utilizadas en tu Proyecto

##### A) El elemento <header>

Representa la cabecera del sitio web o de una sección. Por lo general, contiene el logotipo, el nombre de la empresa y la barra de navegación principal. En tu código se implementa para agrupar la marca superior.

##### B) El elemento <nav>

Delimita un bloque que contiene enlaces de navegación. Su propósito único es agrupar los links que permiten al usuario viajar entre las diferentes páginas del sitio (como Inicio, Puertas, Ventanas, Nosotros y Carrito).

##### C) El elemento <section>

Representa una sección genérica y temática dentro del documento que agrupa contenido relacionado. Cada sección idealmente debe comenzar con un título (<h2>-<h6>). En tu proyecto segmentás el catálogo y el detalle de compras mediante esta etiqueta.

##### D) El elemento <footer>

Define el pie de página de un documento o de una sección. Se ubica al final de la estructura y suele contener información de contacto, enlaces a redes sociales, políticas de privacidad y avisos de derechos de autor (copyright).

---

#### 3.3 El Contenedor Genérico No Semántico: <div>

A pesar de la existencia de etiquetas semánticas, la etiqueta <div> (division) sigue siendo indispensable en el desarrollo web.

- Definición técnica: Es un contenedor de bloque genérico que no tiene ningún significado semántico.
- Propósito real: Se utiliza exclusivamente para agrupar elementos con fines de diseño, estilos arquitectónicos (CSS Flexbox o CSS Grid) o para ser manipulados de forma conjunta mediante JavaScript.

En tu código, utilizás <div> para crear las tarjetas individuales de los productos o para envolver el listado dinámico del carrito. Al no tener significado semántico, no interfiere con la lectura de los motores de búsqueda, pero te permite estructurar la interfaz de forma impecable.

---

### Capítulo 4: Elementos de Contenido, Texto y Listas

#### 4.1 Encabezados Jerárquicos (h1 a h6)

Los encabezados o títulos se definen mediante las etiquetas que van desde <h1> hasta <h6>. La letra "h" proviene del inglés heading.

- Definición técnica: Establecen la importancia y la estructura jerárquica de los contenidos del documento. <h1> es el título de mayor relevancia y <h6> el de menor impacto.
- Regla estricta de SEO y accesibilidad: Solo debe existir un único <h1> por cada página web, el cual representa el tema principal del sitio. No se deben saltar niveles jerárquicos (por ejemplo, pasar de un <h1> directo a un <h3> sin un <h2> de por medio).

En tu proyecto, utilizás <h1> para el nombre principal de tu negocio en la página de inicio, y los <h2> para subdividir secciones clave como "Detalle del carrito" o los títulos de los catálogos.

---

#### 4.2 Párrafos de Texto (<p>)

La etiqueta <p> (paragraph) se utiliza para estructurar bloques de texto continuo.

- Comportamiento en el navegador: Es un elemento de nivel de bloque. Esto significa que el navegador automáticamente añade un espacio en blanco (margen) antes y después del párrafo, obligando a que el siguiente elemento comience en una nueva línea.
- Separación de líneas interna: Si necesitás realizar un salto de línea dentro del mismo párrafo sin generar el espacio de separación que produce <p>, se debe utilizar la etiqueta autoconclusiva <br>.

---

#### 4.3 Estructuras de Listas (ul, ol, li)

Las listas permiten agrupar conjuntos de elementos relacionados. En el desarrollo web existen dos clasificaciones principales:

##### A) Listas No Ordenadas (ul)

La etiqueta <ul> (unordered list) agrupa elementos donde el orden secuencial no altera el significado del contenido. El navegador renderiza cada ítem precedido por una viñeta (un punto negro por defecto).

##### B) Listas Ordenadas (ol)

La etiqueta <ol> (ordered list) se emplea cuando la secuencia u orden de los factores es cronológica, lógica o numerada. El navegador antepone números correlativos de forma automática.

##### C) Elementos de Lista (li)

Tanto las listas <ul> como <ol> no pueden contener texto o etiquetas sueltas directamente en su interior. Es obligatorio que sus elementos hijos directos sean etiquetas <li> (list item).

##### Aplicación práctica en tu código y en las plantillas del campus:

En las barras de navegación, es un estándar absoluto agrupar las opciones dentro de una lista para darle estructura semántica, la cual luego se dispone horizontalmente con estilos:

- Inicio de Lista (<ul>)
  - Elemento (<li>) -> Enlace a Inicio (index.html)
  - Elemento (<li>) -> Enlace a Puertas (puertas.html)
  - Elemento (<li>) -> Enlace a Ventanas (ventanas.html)
- Fin de Lista (</ul>)

---

### Capítulo 5: Enlaces, Multimedia y Botones

#### 5.1 Enlaces de Hipertexto (<a>)

La etiqueta <a> (anchor o ancla) es el elemento fundamental que permite la existencia de la navegación web, conectando un documento con otro.

- Atributo href (Hypertext Reference): Es obligatorio. Especifica la dirección URL de destino o la ruta del archivo local al que se desea redirigir al usuario.
- Navegación interna frente a externa:
  - Interna (entre archivos locales): <a href="carrito.html">Ir al carrito</a>
  - Externa (hacia otros servidores): <a href="https://github.com">GitHub</a>. En enlaces externos, es una buena práctica añadir el atributo target="\_blank" para abrir la página en una pestaña nueva.

---

#### 5.2 Elementos Multimedia: Imágenes (<img>)

La etiqueta <img> se utiliza para empotrar recursos gráficos en el documento estructural.

- Características técnicas únicas: Es un elemento vacío (autoconclusivo). No tiene etiqueta de cierre ni contiene texto interno.
- Atributo src (Source): Define la ruta física (local o URL remota) donde se encuentra almacenado el archivo de imagen (ejemplo: src="img/PuertaAluminio.jpeg").
- Atributo alt (Alternate Text): Es obligatorio. Ofrece una descripción textual de la imagen para los lectores de pantalla (accesibilidad) o por si hay un error de red y el archivo gráfico no carga.

---

#### 5.3 Botones Interactivos (<button>)

La etiqueta <button> representa un elemento de interfaz sobre el cual el usuario puede hacer clic para desencadenar una acción directa.

- Diferencia teórica clave con los enlaces (<a>):
  - Si la acción sirve para desplazarse o viajar a otra página o sección, se utiliza <a>.
  - Si la acción sirve para ejecutar un proceso o cambiar el estado de la aplicación (como "Agregar al carrito" o "Vaciar carrito"), se debe utilizar estrictamente <button>.

---

### Capítulo 6: Atributos Esenciales - Identificadores, Categorías y Datos Ocultos

#### 6.1 El Atributo de Identificación Única (id)

El atributo id se utiliza para asignar un identificador unívoco a un elemento específico dentro del documento HTML.

- Regla de oro estructural: Un valor de id no puede repetirse dentro de la misma página web. Es el DNI de la etiqueta.
- Propósito principal: Permite que JavaScript localice de forma exacta un elemento en el DOM para modificar su contenido o escuchar sus eventos (ejemplo: document.getElementById("carrito-listado")).

---

#### 6.2 El Atributo de Categorización (class)

El atributo class se utiliza para agrupar múltiples elementos bajo una misma categoría o estilo visual.

- Regla de uso: Múltiples elementos pueden compartir exactamente la misma clase. Además, una etiqueta puede tener varias clases asignadas simultáneamente, separadas por un espacio (ejemplo: class="btn btn-primary").
- Propósito principal: Es la columna vertebral de CSS, permitiendo aplicar un diseño una sola vez y reutilizarlo en decenas de tarjetas (.card).

---

#### 6.3 Atributos de Datos Personalizados (data-\*)

Los atributos data-\* permiten almacenar información extra y personalizada directamente en el código de la estructura web, invisible para el usuario pero accesible para los scripts.

##### Aplicación práctica crítica en tu proyecto de Carrito:

En tu catálogo de aberturas, cada tarjeta utiliza estos atributos para guardar los datos técnicos y de precio, permitiendo que JavaScript los lea al instante al hacer clic:

- Elemento Contenedor (class="card" data-id="101" data-precio="230000")
  - Título: Puerta de Aluminio Blanca
  - Botón: Agregar al carrito

---

### Capítulo 7: Estructuras Avanzadas de Interfaz - Formularios, Tablas y Controles del Campus

#### 7.1 Formularios Web (<form>)

Un formulario es la estructura estándar en HTML para recolectar datos introducidos por el usuario y enviarlos a un servidor o procesarlos con JavaScript.

- La etiqueta <form>: Encapsula todos los campos de entrada. Posee atributos como "action" y "method".
- Campos de Entrada (<input>): Etiqueta vacía muy versátil. Su comportamiento cambia según el atributo type:
  - type="text": Campo de texto libre (ej: para el nombre del cliente).
  - type="number": Restringe la entrada a valores numéricos (ej: la cantidad de aberturas).
  - type="email": Valida automáticamente que el texto tenga un formato de correo electrónico.
- La etiqueta <label>: Define la etiqueta de texto para un <input>. Se vincula mediante el atributo "for", que debe coincidir con el "id" del input.

---

#### 7.2 Tablas de Datos (<table>)

Las tablas se utilizan para organizar datos en filas y columnas, ideal para mostrar resúmenes de compras o inventarios de stock.

- <table>: Contenedor principal de la estructura.
- <tr> (Table Row): Define una fila dentro de la tabla.
- <th> (Table Header): Define una celda de encabezado (en negrita y centrada por defecto).
- <td> (Table Data): Define una celda de datos estándar dentro de una fila.

Estructura de ejemplo conceptual:

- Inicio de Tabla
  - Fila de Encabezados: Producto | Cantidad | Precio Unitario
  - Fila de Datos: Puerta de Aluminio | 2 | $230.000
- Fin de Tabla

---

#### 7.3 Estructuras Especiales Basadas en las Plantillas del Campus

Existen patrones de maquetación específicos y clases de estado técnico que se repiten en el campus para construir controles de interfaz.

##### A) Menús de Navegación con Estados Activos

Para indicar en qué página está el usuario, se estructuran menús semánticos utilizando listas, marcando el enlace de la página actual con una clase de estilo dedicada (class="active").

- Estructura: Contenedor (.container) -> Navegación (<nav>) -> Lista (.bar) -> Items (<li>) -> Enlace con class="active".

##### B) Barras de Búsqueda Integradas

La combinación de formularios con contenedores flexibles para búsquedas de productos en catálogos.

- Estructura: Contenedor (.search-box) -> Formulario (<form>) -> Entrada (<input type="text">) y Botón (<button type="submit">).

## BLOQUE II: CSS - El Diseño, Estilo y Maquetación

### Capítulo 8: Introducción a las Hojas de Estilo - ¿Qué es CSS y cómo se vincula al HTML?

#### 8.1 ¿Qué es CSS? Definición Técnica

CSS es el acrónimo de Cascading Style Sheets (Hojas de Estilo en Cascada).

- Lo que NO es: No es un lenguaje de programación ni de marcado estructural.
- Lo que SÍ es: Es un lenguaje de diseño gráfico y presentación. Su única función es tomar el esqueleto crudo y plano de HTML para definir su estética: colores, tipografías, grosores, espaciados y la distribución total de las cajas en la pantalla.
- Principio de Separación de Capas: En el desarrollo profesional, mantener el contenido (HTML) separado del diseño (CSS) es una regla de oro. Permite cambiar por completo el aspecto visual de todo un sitio web modificando un solo archivo de estilos, sin tocar las estructuras de las páginas.

---

#### 8.2 Métodos de Vinculación y Conexión con HTML

Existen tres maneras de aplicar reglas de diseño a un documento HTML. Cada una tiene un impacto directo en el rendimiento de la aplicación y la mantenibilidad del código:

##### A) CSS Externo (El Estándar Profesional)

Los estilos se redactan en un archivo independiente con extensión `.css` (como tu archivo `css/style.css`) y se conectan en la cabecera (`<head>`) del HTML mediante la etiqueta `<link>`.

- Sintaxis: <link rel="stylesheet" href="css/style.css">
- Ventaja: Es el método óptimo. Permite que múltiples páginas (index.html, puertas.html, carrito.html) compartan la misma hoja de estilos, reduciendo la carga de datos y facilitando cambios globales en segundos.

##### B) CSS Interno (Estilos Incrustados)

Las reglas se escriben dentro del mismo archivo HTML, agrupadas en la cabecera mediante el uso de la etiqueta `<style>`.

- Sintaxis de ejemplo:
  <style>
      body { background-color: #f4f4f4; }
  </style>
- Desventaja: Limita la reutilización. Los estilos declarados acá adentro solo afectarán a ese archivo HTML específico, duplicando trabajo si tenés un sitio de varias páginas.

##### C) CSS en Línea (Inline CSS)

Se aplican las propiedades visuales de forma directa sobre una etiqueta HTML usando el atributo global `style`.

- Sintaxis de ejemplo: <button style="background-color: blue; color: white;">Agregar</button>
- Impacto Técnico Negativo: Es considerado una mala práctica para el diseño general. Rompe la separación de capas, vuelve el código HTML pesado, dificulta el mantenimiento y ensucia la jerarquía natural de CSS.

---

#### 8.3 Anatomía de una Regla CSS

Para que el navegador interprete correctamente las instrucciones de diseño, una hoja de estilos se compone de sentencias estructuradas llamadas "reglas". Una regla responde estrictamente al siguiente esquema:

- Esquema básico: selector { propiedad: valor; }

- Selector: Es el puente que le indica al navegador a qué elemento o grupo de elementos HTML se le van a aplicar los cambios estéticos (ejemplo: `h2`, `.card`, `#carrito-listado`).
- Bloque de declaración: Todo lo que se encierra entre las llaves `{ }`. Puede contener una o decenas de instrucciones separadas por un punto y coma `;`.
- Propiedad: El atributo de diseño específico que se quiere alterar (como `color`, `font-size`, `background-color`, `margin`).
- Valor: La especificación técnica o medida concreta que se le asigna a esa propiedad (como `red`, `16px`, `#000000`).

### Capítulo 9: Selectores Básicos (Etiqueta, Clase e ID) y la Regla de la Cascada

#### 9.1 Tipos de Selectores Básicos en CSS

Para poder aplicarle diseño a la estructura que armamos en HTML, CSS utiliza selectores. Un selector es la herramienta técnica que apunta a una o varias etiquetas específicas dentro del documento. Los tres selectores esenciales son:

##### A) Selector de Etiqueta o Tipo

Apunta directamente a todas las etiquetas HTML que tengan el mismo nombre en el archivo.

- Sintaxis: p { color: #333333; }
- Impacto técnico: Modificará de forma global absolutamente todos los párrafos de la aplicación. Se usa para estilos generales del sitio.

##### B) Selector de Clase

Apunta a cualquier elemento que contenga el atributo `class` especificado. Se declara en el archivo CSS anteponiendo un punto (`.`) al nombre de la clase.

- Sintaxis: .card { border: 1px solid #ccc; }
- Impacto técnico: Es el más usado en el diseño profesional. Permite reutilizar el mismo bloque de estilos en múltiples componentes idénticos de tu catálogo, como las tarjetas de productos.

##### C) Selector de ID

Apunta de manera quirúrgica y exclusiva al único elemento que posea ese atributo `id` asignado en el HTML. Se declara anteponiendo un signo de numeral (`#`).

- Sintaxis: #carrito-contador { font-weight: bold; }
- Impacto técnico: Afecta únicamente a una sola etiqueta en toda la página web. No se debe repetir en diseño masivo.

---

#### 9.2 La Regla de la Cascada y el Conflicto de Estilos

Cuando dos o más reglas CSS intentan modificar la misma propiedad de un mismo elemento HTML al mismo tiempo (por ejemplo, definir simultáneamente que un título sea rojo y que sea azul), el motor del navegador resuelve este conflicto de manera automática usando la Regla de la Cascada.

La Cascada es el orden de lectura secuencial: si dos selectores tienen exactamente la misma importancia jerárquica, el navegador aplicará la regla que se lea en último lugar (la que esté más abajo en el archivo `.css`), pisando o sobrescribiendo a las anteriores.

---

#### 9.3 El Concepto de Especificidad (Jerarquía)

No todas las reglas tienen el mismo peso para el navegador. Si un elemento recibe estilos de fuentes cruzadas, el intérprete calcula un puntaje de prioridad técnica llamado Especificidad. Un selector más específico siempre anulará a uno más general, sin importar en qué parte física del archivo se encuentre escrito.

La jerarquía de peso e importancia se divide estrictamente de menor a mayor en tres niveles básicos:

1. Selectores de Etiqueta (Menor peso / Estilo genérico).
2. Selectores de Clase (Peso medio / Estilo reutilizable).
3. Selectores de ID (Mayor peso / Estilo quirúrgico y único).

##### Ejemplo práctico de conflicto:

Si una regla de clase (`.btn-agregar`) dice que el texto sea blanco, pero una regla de ID (`#boton-destacado`) sobre el mismo elemento define que el texto sea negro, el botón se dibujará con texto negro. El ID gana el conflicto por pura superioridad jerárquica en el cálculo de especificidad.

### Capítulo 10: El Modelo de Cajas (Box Model) - Márgenes, Bordes, Rellenos y Dimensiones

#### 10.1 ¿Qué es el Modelo de Cajas?

En CSS, el motor de renderizado del navegador interpreta absolutamente todos los elementos HTML como si fueran cajas rectangulares invisibles. Cada etiqueta, desde un título hasta un botón, se dibuja dentro de este esquema bidimensional.

El Modelo de Cajas es la regla fundamental que determina cuánto espacio ocupa un elemento en la pantalla y cómo interactúa con los componentes que lo rodean.

---

#### 10.2 Los Cuatro Componentes de una Caja

Cada caja en CSS está compuesta por cuatro capas concéntricas que se estructuran desde adentro hacia afuera:

- A) El Contenido (Content): Es la zona central donde se renderiza el texto, las imágenes o los elementos hijos (por ejemplo, el texto de un botón). Sus dimensiones se controlan con las propiedades width (ancho) y height (alto).
- B) El Relleno (Padding): Es el espacio interno transparente que separa el contenido del borde de la caja. Sirve para darle "aire" al texto y que no quede pegado a los límites del contenedor.
- C) El Borde (Border): Es la línea que delimita la caja. Puede ser invisible, delgada, gruesa, sólida o discontinua. Se configura usando la propiedad border (ej: border: 2px solid black).
- D) El Margen (Margin): Es el espacio externo transparente que separa a la caja de las otras cajas vecinas en la página web. Sirve para empujar o distanciar elementos entre sí.

---

#### 10.3 Control de Dimensiones Básicas (width y height)

Para definir el tamaño del contenido de un contenedor (como las tarjetas `.card` de tu proyecto), se utilizan las siguientes propiedades:

- width: Define el ancho del bloque. Puede expresarse en medidas fijas (como píxeles, ej: `width: 300px`) o en medidas relativas (como porcentajes, ej: `width: 100%`).
- height: Define el alto del bloque. Al igual que el ancho, responde a píxeles o porcentajes, aunque en diseño moderno se suele dejar en automático (`height: auto`) para que la caja crezca verticalmente según el contenido que tenga adentro.

---

#### 10.4 Modificando el Comportamiento con box-sizing

Por defecto, el navegador calcula el tamaño total de una caja sumando el ancho del contenido + el padding + el border. Esto significa que si creás una tarjeta de `width: 300px` y le agregás un padding de `20px` por lado, la tarjeta pasará a medir `340px` reales en la pantalla, rompiendo muchas veces la maquetación.

Para solucionar este comportamiento confuso, el desarrollo moderno utiliza una propiedad indispensable:

- box-sizing: border-box;

Al aplicar esta regla (generalmente a todos los elementos del proyecto con el selector universal `*`), le ordenás al navegador que incluya el padding y el border dentro de los `300px` que definiste originalmente. El contenido se achicará automáticamente para mantener el tamaño exacto que vos le pediste a la caja, garantizando un diseño predecible y prolijo.

### Capítulo 11: Colores, Fondos y Degradados (Sólidos, Opacidad y Filtros Visuales)

#### 11.1 Formatos de Color en CSS

Para aplicar color tanto al texto (`color`) como al fondo (`background-color`) de cualquier elemento, CSS utiliza diferentes sistemas de codificación técnica:

- **Palabras Clave (Keywords):** Colores predefinidos por el navegador mediante su nombre en inglés (ej: `red`, `blue`, `transparent`). Su uso se limita a pruebas rápidas debido a la falta de variedad.
- **Sistema Hexadecimal (#RRGGBB):** Representa la intensidad de los canales Rojo (Red), Verde (Green) y Azul (Blue) usando números del 0 al 9 y letras de la A a la F. Es el formato estándar y más liviano en el desarrollo (ej: `#ffffff` para blanco, `#000000` para negro).
- **Sistema Funcional RGB / RGBA:** Define los mismos tres canales utilizando valores numéricos del 0 al 255 (ej: `rgb(255, 0, 0)` para rojo puro). El formato **RGBA** añade un cuarto parámetro llamado **Alpha**, que regula el nivel de opacidad o transparencia del color en una escala del 0 (totalmente invisible) al 1 (totalmente sólido), por ejemplo: `rgba(0, 0, 0, 0.5)` para un fondo negro translúcido al 50%.

---

#### 11.2 Propiedades de Fondo (Backgrounds)

El control del fondo de un contenedor va más allá de un color plano. CSS permite manipular imágenes y capas traseras mediante propiedades específicas:

- `background-image`: Permite cargar un recurso gráfico detrás del contenido utilizando la sintaxis `url('ruta/imagen.jpg')`.
- `background-size`: Regula el tamaño de la imagen de fondo. Su valor más eficiente es `cover`, que estira y adapta la imagen para que cubra todo el contenedor sin deformarse.
- `background-repeat`: Por defecto, el navegador repite las imágenes en mosaico si son más chicas que la caja. Se anula usando `no-repeat`.

##### Degradados Nativos (Gradients)

Los degradados no se consideran colores planos, sino imágenes generadas por código. Se declaran mediante la propiedad `background-image`:

- **Degradados Lineales (`linear-gradient`):** Transición de color en línea recta. Permite definir la dirección en grados (ej: `45deg`) o hacia un extremo (ej: `to right`), seguido de los colores involucrados: `background-image: linear-gradient(to right, #000000, #333333);`.

---

#### 11.3 Opacidad General y Filtros Visuales

- **La propiedad `opacity`:** Modifica la transparencia de un elemento completo (incluyendo su fondo, sus textos y todos los elementos que tenga adentro) en una escala de 0 a 1. A diferencia de `rgba()`, que solo transparenta el color de fondo, `opacity` afecta a todo el bloque por igual.
- **La propiedad `filter`:** Aplica efectos gráficos de postprocesamiento directamente en el navegador sobre imágenes o contenedores. Algunos de los filtros más utilizados en interfaces modernas son `blur()` (desenfoque para fondos tipo vidrio esmerilado) y `grayscale()` (convierte elementos a escala de grises, ideal para imágenes de productos sin stock).

### Capítulo 12: Posicionamiento y Control de Desbordes (position, overflow, z-index)

#### 12.1 La Propiedad position y el Flujo Documental

Por defecto, el navegador acomoda las cajas una abajo de la otra o una al lado de la otra siguiendo el orden físico del código HTML. Para romper ese flujo natural y mover elementos de forma quirúrgica por la pantalla, se utiliza la propiedad `position` combinada con las coordenadas de empuje: `top` (arriba), `bottom` (abajo), `left` (izquierda) y `right` (derecha).

##### A) Posicionamiento Relativo (`position: relative;`)

La caja se mueve tomando como punto de partida su posición original en el flujo de la página. Aunque se desplace, el espacio vacío que ocupaba originalmente se reserva y ningún otro elemento lo puede usar.

##### B) Posicionamiento Absoluto (`position: absolute;`)

La caja se arranca por completo del flujo de la página; el resto de los elementos actúan como si esa caja no existiera y ocupan su lugar.

- **Regla de Oro de la Coordenada:** Un elemento absoluto se posiciona tomando como referencia los límites del primer contenedor padre que tenga un `position: relative;`. Si no encuentra ningún padre relativo, se moverá respecto a los bordes totales de la ventana del navegador.

---

#### 12.2 Control de Desbordes (overflow)

Cuando el contenido de una caja (un texto muy largo o una lista dinámica de productos en el carrito) supera las dimensiones de ancho o alto fijadas para su contenedor padre, se produce un desborde. La propiedad `overflow` determina cómo reacciona el navegador ante este problema:

- `overflow: visible;` (Por defecto): El contenido excedente se sale de los bordes de la caja y se dibuja por encima de los otros elementos de la página, ensuciando la interfaz.
- `overflow: hidden;` (Oculto): Corta de forma quirúrgica todo el contenido que exceda los límites de la caja, volviendo invisible el sobrante.
- `overflow: auto;` o `scroll`: Añade barras de desplazamiento (scrollbars) automáticas únicamente si el contenido supera el espacio disponible, manteniendo la estructura de la interfaz intacta. Es ideal para listados largos de compras.

---

#### 12.3 El Eje Z y la Superposición (z-index)

Cuando los elementos se posicionan de manera absoluta o relativa, es común que empiecen a encimarse unos sobre otros. CSS controla qué elemento se dibuja adelante y cuál queda escondido atrás utilizando el eje tridimensional a través de la propiedad `z-index`.

- **Funcionamiento:** Recibe valores numéricos enteros (positivos, negativos o cero). Un elemento con un número mayor (ej: `z-index: 10;`) se renderizará siempre al frente de un elemento con un puntaje menor (ej: `z-index: 2;`).
- **Restricción Técnico Crítica:** La propiedad `z-index` **solo funciona en elementos que tengan un posicionamiento declarado** (`relative`, `absolute`, `fixed`, etc.). Si se aplica sobre una caja con el flujo estático por defecto, el navegador ignorará el valor por completo.

### Capítulo 13: Maquetación Moderna I: Flexbox (Ejes, Alineación y Distribución del Espacio)

#### 13.1 ¿Qué es Flexbox y por qué es indispensable?

Flexbox (Flexible Box Layout) es un modelo de maquetación unidimensional diseñado para organizar, alinear y distribuir el espacio entre los elementos de un contenedor, incluso cuando sus dimensiones son desconocidas o dinámicas (como cuando agregás productos al carrito).

- El cambio de paradigma: A diferencia del modelo de cajas tradicional (donde los elementos se apilan vertical u horizontalmente de forma rígida), Flexbox permite que las cajas hijas alteren su ancho, alto y orden para llenar de forma óptima el espacio disponible de la pantalla, evitando que el diseño se rompa en dispositivos móviles.

---

#### 13.2 Contenedor (Flex Parent) y Elementos (Flex Items)

Para que Flexbox funcione, la estructura se divide estrictamente en dos niveles jerárquicos:

- **El Contenedor Padre:** El elemento al que se le aplica la propiedad `display: flex;`. Al hacer esto, activa el contexto flexible de forma inmediata.
- **Los Elementos Hijos:** Todas las etiquetas que se encuentran adentro del contenedor padre de forma directa. Automáticamente se convierten en "flex items" y empiezan a responder a las reglas del padre.

---

#### 13.3 El Sistema de Ejes (Main Axis y Cross Axis)

Flexbox no trabaja con las coordenadas arriba/abajo o izquierda/derecha, sino que opera bajo un sistema de dos ejes perpendiculares. Entender esto es la clave absoluta para dominar Flexbox:

- **Eje Principal (Main Axis):** Es el eje primario a lo largo del cual se acomodan los elementos hijos. Por defecto va de izquierda a derecha.
- **Eje Cruzado (Cross Axis):** Es el eje perpendicular al eje principal. Por defecto va de arriba hacia abajo.

##### Cambiando el sentido con flex-direction

La propiedad `flex-direction` define cuál va a ser el eje principal del contenedor:

- `flex-direction: row;` (Por defecto): El eje principal es horizontal. Los elementos se posicionan uno al lado del otro.
- `flex-direction: column;` (Muy usado en celulares): El eje principal pasa a ser vertical. Los elementos se apilan uno abajo del otro.

---

#### 13.4 Propiedades de Alineación y Distribución

Una vez definido el eje principal, el contenedor padre utiliza tres propiedades fundamentales para controlar la distribución de sus elementos hijos:

##### A) justify-content (Alineación en el Eje Principal)

Controla cómo se distribuye el espacio vacío que sobra en el eje principal. Sus valores más importantes son:

- `flex-start` (Por defecto): Agrupa todos los elementos al inicio del contenedor.
- `flex-end`: Empuja todos los elementos hacia el final del contenedor.
- `center`: Centra todos los elementos de forma conjunta.
- `space-between`: Separa los elementos al máximo, dejando el espacio sobrante equitativamente _entre_ ellos (las cajas de los extremos tocan los bordes del contenedor). Ideal para la barra de navegación del campus o cabeceras de e-commerce.
- `space-around`: Distribuye el espacio sobrante alrededor de cada elemento por igual.

##### B) align-items (Alineación en el Eje Cruzado)

Controla cómo se alinean los elementos hijos en el eje perpendicular (eje cruzado). Sus valores más comunes son:

- `stretch` (Por defecto): Estira a todos los elementos hijos para que midan lo mismo que la caja más alta o que el contenedor padre.
- `center`: Centra los elementos verticalmente (si están en fila), logrando que los textos y botones queden perfectamente alineados sin importar sus diferentes alturas.
- `flex-start` / `flex-end`: Alinea los elementos al tope superior o al borde inferior del eje cruzado.

##### C) gap (Espaciado Inteligente)

En la maquetación moderna ya no se usan márgenes difíciles de calcular para separar las cajas flexibles. Se aplica la propiedad `gap` (o `row-gap` y `column-gap`) directamente en el contenedor padre.

- Ejemplo: `gap: 20px;` le indica al navegador que mantenga una separación exacta de 20 píxeles estrictamente _entre_ los elementos hijos, sin agregar márgenes molestos en los bordes externos del contenedor.

### Capítulo 14: Maquetación Moderna II: CSS Grid (Grillas, Columnas y Filas)

#### 14.1 ¿Qué es CSS Grid y en qué se diferencia de Flexbox?

CSS Grid Layout es el sistema de maquetación más potente de CSS. A diferencia de Flexbox, que es un modelo unidimensional (diseñado para trabajar en filas o en columnas a la vez), CSS Grid es un modelo bidimensional.

- **El superpoder de Grid:** Permite controlar de forma simultánea tanto las filas (eje vertical) como las columnas (eje horizontal). Está pensado para la estructura general de la interfaz de usuario, permitiendo diseñar grillas complejas y ordenadas sin necesidad de anidar infinitos contenedores div.

---

#### 14.2 Conceptos Clave de la Arquitectura Grid

Para armar una grilla correctamente, es necesario conocer los componentes técnicos que la conforman:

- **Grid Container (Contenedor):** El elemento padre que activa el contexto de grilla al declararle la propiedad `display: grid;`.
- **Grid Item (Elemento hijo):** Cada una de las cajas que se encuentran directamente dentro del contenedor.
- **Grid Line (Línea de la grilla):** Las líneas divisorias invisibles (horizontales y verticales) que delimitan las filas y columnas. Se empiezan a contar desde el número 1.
- **Grid Track (Banda o Carril):** El espacio comprendido entre dos líneas consecutivas. Es el término técnico para referirse a una fila o a una columnna completa.
- **Grid Cell (Celda):** La unidad mínima de la grilla, delimitada por la intersección de una fila y una columna (el equivalente a una celda de Excel).

---

#### 14.3 Definición de la Estructura (grid-template)

Una vez activado el `display: grid;` en el contenedor padre, se debe definir cuántas columnas y filas va a tener la grilla usando las siguientes propiedades:

##### A) grid-template-columns

Define el número y el ancho de las columnas. Se puede especificar usando medidas fijas (`px`), relativas (`%`) o la unidad nativa de Grid: la Fracción (`fr`).

- **La unidad `fr`:** Representa una fracción del espacio libre disponible dentro del contenedor. Si definís `grid-template-columns: 1fr 2fr 1fr;`, el navegador dividirá el espacio en 4 partes iguales: la primera y tercera columna ocuparán una parte, y la del medio ocupará el doble de espacio.
- **La función `repeat()`:** Para evitar escribir muchas veces el mismo valor, se usa el atajo `repeat(cantidad, tamaño)`. Por ejemplo, `grid-template-columns: repeat(3, 1fr);` crea una grilla perfecta de 3 columnas iguales.

##### B) grid-template-rows

Define la cantidad y la altura de las filas de la grilla de forma idéntica a las columnas. En maquetación de catálogos se suele combinar con valores fijos o con la palabra clave `auto` para que la altura de la fila se adapte al tamaño del contenido de los productos.

---

#### 14.4 Ubicación Quirúrgica de los Elementos (Grid Placement)

La verdadera potencia de Grid se nota cuando queremos que un elemento hijo ocupe más de una celda o se estire a lo largo de varias columnas (por ejemplo, para que el `header` o el `footer` de tu proyecto cruce toda la pantalla de lado a lado). Para lograr esto, se aplican propiedades directamente sobre el elemento hijo usando los números de las líneas divisorias:

- `grid-column-start`: La línea vertical donde empieza el elemento.
- `grid-column-end`: La línea vertical donde termina el elemento.

##### Atajos profesionales:

- `grid-column`: Es la unión de los dos anteriores separados por una barra diagonal. Ejemplo: `grid-column: 1 / 4;` (el elemento empezará en la línea 1 y terminará en la línea 4, ocupando 3 columnas completas).
- **La palabra clave `span`:** Se usa para indicarle al navegador cuántas columnas o filas debe estirarse el elemento desde su posición actual sin importar el número de línea final. Ejemplo: `grid-column: span 3;` (se estira a lo largo de 3 columnas).

Al igual que en Flexbox, la separación entre todas las celdas se maneja de forma limpia usando la propiedad `gap: 20px;` directamente en el contenedor padre, garantizando un diseño simétrico y prolijo.

### Capítulo 15: Estados, Pseudoclases y Transiciones (:hover, :active, cambios de estado visual)

#### 15.1 ¿Qué son las Pseudoclases?

Las pseudoclases son palabras clave que se añaden a los selectores CSS para definir un estilo específico basado en el estado actual del elemento, la interacción del usuario o la posición estructural de la etiqueta en el HTML.

- **Sintaxis:** Se declaran anteponiendo dos puntos (`:`) al nombre de la pseudoclase inmediatamente después del selector. Ejemplo: `selector:pseudoclase { propiedad: valor; }`
- **Propósito en la interfaz:** Permiten que la página web responda de forma visual a las acciones del usuario (como pasar el mouse por encima de una tarjeta o hacer clic en un botón) sin necesidad de recurrir a programación con JavaScript.

---

#### 15.2 Pseudoclases de Interacción Esenciales

Para mejorar la experiencia de usuario (UX) en elementos interactivos como los botones de tu catálogo o los enlaces del menú del campus, se utilizan tres pseudoclases fundamentales de interacción:

##### A) :hover (Paso del cursor)

Se activa de forma inmediata cuando el usuario posiciona el puntero del mouse por encima de un elemento (sin necesidad de hacer clic).

- **Aplicación típica:** Cambiar el color de fondo de un botón (`.btn-agregar:hover`) o subrayar un enlace para indicarle claramente al usuario que ese elemento es interactivo y se puede cliquear.

##### B) :active (Momento del clic)

Se activa estrictamente durante el microsegundo en que el usuario mantiene presionado el botón izquierdo del mouse sobre el elemento.

- **Aplicación típica:** Achicar sutilmente el tamaño de un botón o hundir su sombra (`.btn-agregar:active`) para simular físicamente el efecto mecánico de un pulsador real.

##### C) :focus (Elemento seleccionado)

Se activa cuando un elemento recibe el foco de atención de la interfaz, ya sea porque el usuario hizo clic adentro de él o porque navegó usando la tecla Tabulador del teclado.

- **Aplicación típica:** Es indispensable en los campos de los formularios (`input:focus`). Cambiar el color del borde del campo de texto cuando el usuario está escribiendo su nombre o correo ayuda a la accesibilidad del sitio.

---

#### 15.3 Transiciones CSS (Suavizado de Cambios de Estado)

Por defecto, cuando un elemento pasa de su estado normal a un estado interactivo (como de `.btn` a `.btn:hover`), el navegador cambia los colores o tamaños de forma instantánea y brusca. Para suavizar este comportamiento y generar efectos visuales profesionales, se utiliza la propiedad `transition`.

La propiedad `transition` se debe declarar siempre en la **caja base o estado normal** del elemento (no dentro del `:hover`), y requiere configurar tres parámetros clave:

- **Propiedad a animar (`transition-property`):** Qué atributo de diseño va a cambiar de forma fluida (ej: `background-color`, `transform`, `all` si se quieren suavizar todos los cambios).
- **Duración (`transition-duration`):** Cuánto tiempo va a tardar en completarse el efecto, expresado en segundos (`s`) o milisegundos (`ms`). Un estándar fluido en diseño web es usar entre `0.2s` y `0.3s`.
- **Función de tiempo (`transition-timing-function`):** Regula la aceleración del movimiento. El valor `ease` (por defecto) arranca lento, acelera en el medio y frena suave al final.

##### Ejemplo de código integrado para un botón:

```css
/* Estado Normal Base */
.btn-agregar {
  background-color: #000000;
  color: #ffffff;
  /* Suaviza los cambios en el fondo y el tamaño durante 0.3 segundos */
  transition:
    background-color 0.3s ease,
    transform 0.2s ease;
}

/* Estado al pasar el mouse */
.btn-agregar:hover {
  background-color: #333333;
}

/* Estado al hacer clic */
.btn-agregar:active {
  transform: scale(0.95); /* Achica el botón un 5% simulando presión */
}
```

### Capítulo 16: Animaciones CSS nativas y Fotogramas Clave (@keyframes)

#### 16.1 Diferencia entre Transiciones y Animaciones

Aunque ambas herramientas sirven para generar movimiento y dinamismo en la pantalla, tienen propósitos técnicos completamente diferentes:

- **Las Transiciones:** Requieren obligatoriamente un disparador o acción del usuario (como un `:hover` o un cambio de clase con JavaScript) para pasar de un punto A a un punto B de forma fluida.
- **Las Animaciones:** Son autónomas. Tienen la capacidad de ejecutarse de forma automática apenas se carga la página web, pueden repetirse en bucle de manera infinita y permiten trazar recorridos complejos pasando por múltiples puntos intermedios (A, B, C, D, etc.).

---

#### 16.2 La Regla de Fotogramas Clave (@keyframes)

Para crear una animación nativa en CSS, el proceso se divide estrictamente en dos pasos independientes: **definir la línea de tiempo** y **asignar esa línea de tiempo al elemento**.

La regla `@keyframes` se utiliza para declarar los fotogramas clave y especificar qué propiedades de diseño van a cambiar en momentos exactos de la secuencia. Su sintaxis utiliza porcentajes que van desde el `0%` (inicio de la animación) hasta el `100%` (final de la animación):

Estructura técnica de una secuencia:

- Al 0% (Inicio): El elemento arranca invisible (opacity: 0) y desplazado hacia abajo (transform: translateY(20px)).
- Al 50% (Medio): El elemento se vuelve completamente visible (opacity: 1) y sube un poco de más por inercia (transform: translateY(-5px)).
- Al 100% (Fin): El elemento se acomoda y se asienta en su posición final exacta (transform: translateY(0)).

---

#### 16.3 Propiedades de Control de la Animación

Una vez que la línea de tiempo está creada con `@keyframes`, se debe vincular al selector del elemento HTML que se desea mover (por ejemplo, una alerta de "Producto agregado" o un cartel flotante). Para controlar su comportamiento, CSS utiliza las siguientes propiedades:

##### A) animation-name

Especifica el nombre exacto de la línea de tiempo `@keyframes` que se va a utilizar.

##### B) animation-duration

Define cuánto tiempo tarda la animación en completar un ciclo completo, expresado en segundos (`s`) o milisegundos (`ms`). Un estándar fluido suele ser `0.5s`.

##### C) animation-iteration-count

Determina cuántas veces se va a reproducir el ciclo de movimiento. Puede recibir un número entero fijo (ej: `3`) o la palabra clave `infinite` para que la animación no se detenga nunca (ideal para iconos de carga o spinners).

##### D) animation-timing-function

Al igual que en las transiciones, regula el ritmo y la aceleración del movimiento a lo largo del tiempo (`ease`, `linear`, `ease-out`).

##### E) animation-fill-mode

Es una propiedad crítica. Determina qué pasa con los estilos del elemento cuando la animación termina.

- Por defecto, el elemento vuelve bruscamente a sus estilos originales del CSS base.
- Si se configura en `forwards`, el navegador obliga al elemento a retener los estilos exactos declarados en el último fotograma clave (`100%`), evitando saltos visuales desprolijos.

##### El Atajo Profesional (Sintaxis Shorthand):

Para ahorrar líneas de código, todas estas subpropiedades se pueden agrupar en una sola línea siguiendo un orden estricto:

- Sintaxis: `.alerta-carrito { animation: aparecerYFlotar 0.5s ease-out 1 forwards; }`

### Capítulo 16: Animaciones CSS nativas y Fotogramas Clave (@keyframes)

#### 16.1 Diferencia entre Transiciones y Animaciones

Aunque ambas herramientas sirven para generar movimiento y dinamismo en la pantalla, tienen propósitos técnicos completamente diferentes:

- **Las Transiciones:** Requieren obligatoriamente un disparador o acción del usuario (como un `:hover` o un cambio de clase con JavaScript) para pasar de un punto A a un punto B de forma fluida.
- **Las Animaciones:** Son autónomas. Tienen la capacidad de ejecutarse de forma automática apenas se carga la página web, pueden repetirse en bucle de manera infinita y permiten trazar recorridos complejos pasando por múltiples puntos intermedios (A, B, C, D, etc.).

---

#### 16.2 La Regla de Fotogramas Clave (@keyframes)

Para crear una animación nativa en CSS, el proceso se divide estrictamente en dos pasos independientes: **definir la línea de tiempo** y **asignar esa línea de tiempo al elemento**.

La regla `@keyframes` se utiliza para declarar los fotogramas clave y especificar qué propiedades de diseño van a cambiar en momentos exactos de la secuencia. Su sintaxis utiliza porcentajes que van desde el `0%` (inicio de la animación) hasta el `100%` (final de la animación):

Estructura técnica de una secuencia:

- Al 0% (Inicio): El elemento arranca invisible (opacity: 0) y desplazado hacia abajo (transform: translateY(20px)).
- Al 50% (Medio): El elemento se vuelve completamente visible (opacity: 1) y sube un poco de más por inercia (transform: translateY(-5px)).
- Al 100% (Fin): El elemento se acomoda y se asienta en su posición final exacta (transform: translateY(0)).

---

#### 16.3 Propiedades de Control de la Animación

Una vez que la línea de tiempo está creada con `@keyframes`, se debe vincular al selector del elemento HTML que se desea mover (por ejemplo, una alerta de "Producto agregado" o un cartel flotante). Para controlar su comportamiento, CSS utiliza las siguientes propiedades:

##### A) animation-name

Especifica el nombre exacto de la línea de tiempo `@keyframes` que se va a utilizar.

##### B) animation-duration

Define cuánto tiempo tarda la animación en completar un ciclo completo, expresado en segundos (`s`) o milisegundos (`ms`). Un estándar fluido suele ser `0.5s`.

##### C) animation-iteration-count

Determina cuántas veces se va a reproducir el ciclo de movimiento. Puede recibir un número entero fijo (ej: `3`) o la palabra clave `infinite` para que la animación no se detenga nunca (ideal para iconos de carga o spinners).

##### D) animation-timing-function

Al igual que en las transiciones, regula el ritmo y la aceleración del movimiento a lo largo del tiempo (`ease`, `linear`, `ease-out`).

##### E) animation-fill-mode

Es una propiedad crítica. Determina qué pasa con los estilos del elemento cuando la animación termina.

- Por defecto, el elemento vuelve bruscamente a sus estilos originales del CSS base.
- Si se configura en `forwards`, el navegador obliga al elemento a retener los estilos exactos declarados en el último fotograma clave (`100%`), evitando saltos visuales desprolijos.

##### El Atajo Profesional (Sintaxis Shorthand):

Para ahorrar líneas de código, todas estas subpropiedades se pueden agrupar en una sola línea siguiendo un orden estricto:

- Sintaxis: `.alerta-carrito { animation: aparecerYFlotar 0.5s ease-out 1 forwards; }`

## BLOQUE III: JAVASCRIPT - La Lógica y la Interactividad

### Capítulo 17: Introducción a JavaScript - Variables, Tipos de Datos y Operadores Básicos

#### 17.1 ¿Qué es JavaScript? Definición Técnica

JavaScript (JS) es un lenguaje de programación de alto nivel, interpretado, orientado a objetos y multiplataforma.

- **Su rol en la web:** Mientras que HTML crea la estructura (el esqueleto) y CSS define la estética (la piel y la ropa), JavaScript aporta el comportamiento y la interactividad (los músculos y el sistema nervioso). Permite que la página web responda a eventos complejos, procese cálculos matemáticos, manipule los productos del carrito en tiempo real y guarde datos sin necesidad de recargar la pestaña.

---

#### 17.2 Variables y Constantes (El Almacenamiento de Datos)

Una variable es un espacio reservado en la memoria de la computadora destinado a guardar un valor temporal que la aplicación necesita utilizar o modificar más adelante. En JavaScript moderno existen tres formas de declarar estos contenedores:

##### A) let (Variables Mutables)

Se utiliza para declarar variables cuyo valor puede cambiar (mutar) a lo largo de la ejecución del programa.

- **Ejemplo práctico:** `let cantidadProductos = 1;` (si el usuario hace clic en agregar, este número subirá a 2).

##### B) const (Constantes Inmutables)

Se emplea para declarar valores fijos que no pueden ser reasignados ni modificados una vez definidos. Si intentás cambiar su valor por código, el navegador arrojará un error técnico.

- **Ejemplo práctico:** `const precioUnitario = 230000;` o `const ID_PRODUCTO = "A102";`. En el desarrollo profesional se prioriza el uso de `const` por sobre `let` para evitar errores accidentales.

##### C) var (Obsoleto)

Era la forma antigua de declarar variables. Hoy en día está completamente desaconsejado su uso debido a problemas de alcance o ámbito técnico (scope) que provocaban comportamientos erráticos e impredecibles en scripts extensos.

---

#### 17.3 Tipos de Datos Primitivos

Cada valor que se almacena en una variable pertenece a un tipo de dato específico, lo que le indica al motor de JavaScript qué operaciones puede realizar con él. Los tipos primitivos esenciales son:

- **Number (Numéricos):** Representa valores cuantitativos, ya sean enteros (`let stock = 14;`) o decimales (`let total = 4500.50;`). A diferencia de otros lenguajes, JS maneja todos los números bajo el mismo tipo de dato.
- **String (Cadenas de Texto):** Secuencias de caracteres alfanuméricos utilizadas para representar texto. Se encierran estrictamente entre comillas simples (`'...'`), comillas dobles (`"..."`) o comillas invertidas (Backticks `` `...` ``). Ejemplo: `const nombreProducto = "Puerta de Aluminio Blanca";`.
- **Boolean (Booleanos):** Tipo de dato lógico que solo puede adoptar uno de dos valores posibles: `true` (verdadero) o `false` (falso). Es la columna vertebral de la lógica de control. Ejemplo: `let carritoVacio = true;`.
- **Undefined:** Estado por defecto que adopta una variable que ha sido declarada por el programador pero a la cual todavía no se le ha asignado ningún valor concreto (ej: `let subtotal;`).
- **Null:** Valor que representa la ausencia intencional de cualquier objeto o valor. El programador lo asigna explícitamente para indicar que una variable está vacía por diseño.

---

#### 17.4 Operadores Básicos

Los operadores son símbolos técnicos que le permiten al motor de JavaScript realizar acciones, cálculos o comparaciones sobre los valores de nuestras variables.

##### A) Operadores Aritméticos (Cálculos Matemáticos)

Sirven para procesar operaciones matemáticas estándar dentro de la aplicación (como calcular el total de una compra):

- Suma (`+`): `let total = precio + envio;` (Ojo: si se aplica entre textos, los concatena/une).
- Resta (`-`): `let saldo = presupuesto - costo;`
- Multiplicación (`*`): `let subtotal = precio * cantidad;`
- División (`/`): `let promedio = total / 2;`
- Módulo o Resto (`%`): Retorna el residuo de una división entera (muy usado para saber si un número es par o impar).

##### B) Operadores de Asignación con Operación (Atajos de Código)

Permiten modificar el valor actual de una variable combinando una operación aritmética básica en un solo paso corto:

- Incremento corto: `cantidad += 1;` (es el equivalente exacto a escribir `cantidad = cantidad + 1;`).
- Decremento corto: `stock -= 1;`

##### C) Operadores de Comparación

Se utilizan para evaluar dos valores y retornan obligatoriamente un booleano (`true` o `false`):

- Mayor que (`>`) y Menor que (`<`): `stock < 5`
- Mayor o igual (`>=`) y Menor o igual (`<=`)
- Igualdad Estricta (`===`): Compara que tanto el valor como el tipo de dato sean exactamente idénticos (ej: `10 === 10` es `true`, pero `10 === "10"` es `false`). **Se debe usar siempre este operador en lugar del doble igual (`==`) para evitar fallos de conversión automáticos.**
- Distinto Estricto (`!==`): Evalúa si dos componentes son diferentes en valor o tipo.

### Capítulo 18: Control de Flujo - Condicionales (if/else), el Atajo Ternario (? :) y Bucles (for, while)

#### 18.1 ¿Qué es el Control de Flujo?

Por defecto, el motor de JavaScript lee y ejecuta tu archivo de código de forma secuencial, es decir, línea por línea desde el principio hasta el final.

El Control de Flujo es la capacidad de romper esa lectura lineal y rígida. Nos permite introducir bifurcaciones en el camino para tomar decisiones (ejecutar un bloque de código solo si se cumple una condición) o repetir tareas de forma automática sin necesidad de duplicar líneas de código escritas a mano.

---

#### 18.2 Estructuras Condicionales (if, else if, else)

Las estructuras condicionales evalúan una expresión lógica (que devuelve true o false) y, en base al resultado, deciden qué camino debe seguir el programa.

##### A) La sentencia if (Si condicional)

Es la estructura básica. El código dentro de sus llaves solo se ejecutará si la condición entre paréntesis es verdadera.

- Ejemplo:
  if (stock > 0) {
  // Este código se ejecuta solo si hay stock disponible
  console.log("Producto disponible para la venta");
  }

##### B) La cláusula else (De lo contrario)

Se encadena inmediatamente al if para definir un camino alternativo y obligatorio en caso de que la condición principal sea falsa.

- Ejemplo:
  if (stock > 0) {
  console.log("Producto disponible");
  } else {
  // Se ejecuta estrictamente si stock es igual o menor a 0
  console.log("Alerta: Sin stock disponible");
  }

##### C) La estructura else if (Anidación selectiva)

Permite evaluar múltiples condiciones en orden secuencial. El navegador las revisará una por una de arriba hacia abajo y ejecutará únicamente el bloque de la primera condición que resulte verdadera.

- Ejemplo:
  if (precio === 0) {
  console.log("Error: El precio no puede ser cero.");
  } else if (precio < 0) {
  console.log("Error: El precio no puede ser un valor negativo.");
  } else {
  console.log("Precio validado correctamente.");
  }

---

#### 18.3 El Atajo Ternario (? :)

El operador ternario es una forma compacta y elegante de escribir una estructura if / else simple en una sola línea de código. Es ideal para asignar valores a variables de forma directa basándose en una condición.

- Sintaxis: condición ? expresión_si_es_true : expresión_si_es_false;

##### Ejemplo práctico comparativo:

- Usando if/else tradicional:
  let mensajeStock;
  if (stock > 0) {
  mensajeStock = "Disponible";
  } else {
  mensajeStock = "Agotado";
  }

- Usando el Atajo Ternario (Mismo resultado en una sola línea):
  let mensajeStockTernario = (stock > 0) ? "Disponible" : "Agotado";

---

#### 18.4 Estructuras de Repetición o Bucles (Loops)

Los bucles permiten ejecutar un mismo bloque de código de forma repetitiva tantas veces como sea necesario. Son indispensables para recorrer listados, como las tarjetas de aberturas de tu catálogo.

##### A) El Bucle for (Repetición controlada por conteo)

Se utiliza de forma estricta cuando sabés de antemano cuántas veces exactas necesitás que se repita la acción. Su sintaxis agrupa tres instrucciones en su cabecera separadas por punto y coma:

1. Inicialización: Crea una variable contador (ej: let i = 0;).
2. Condición de permanencia: El bucle seguirá iterando mientras esto sea true (ej: i < 5;).
3. Actualización: Incrementa o decrementa el contador en cada vuelta (ej: i++).

- Ejemplo:
  // Este bucle imprimirá en la consola los números del 0 al 4
  for (let i = 0; i < 5; i++) {
  console.log("Vuelta número: " + i);
  }

##### B) El Bucle while (Repetición controlada por condición)

Se utiliza cuando no sabés la cantidad exacta de vueltas que dará el bucle, ya que depende enteramente de que una condición lógica sea verdadera.

- Riesgo Técnico Crítico (Bucle Infinito): Si la condición dentro del while nunca se vuelve falsa durante la ejecución, el bucle se repetirá infinitamente, congelando el navegador del usuario y consumiendo el 100% de la memoria. Siempre se debe asegurar que ocurra un cambio interno que rompa la condición.

- Ejemplo:
  let vueltas = 0;
  while (vueltas < 3) {
  console.log("Procesando...");
  vueltas++; // Operación crítica: modifica el valor para que la condición dé false eventualmente
  }

### Capítulo 19: Funciones y Modularidad - Cómo encapsular lógica y retornar datos útiles

#### 19.1 ¿Qué es una Función? El Concepto de Encapsulamiento

Una función es un bloque de código estructurado e independiente que realiza una tarea específica.

- **El superpoder de la modularidad:** En lugar de escribir las mismas líneas de código cada vez que querés calcular el total del carrito o aplicar un descuento, agrupás esas instrucciones adentro de una función. Este bloque queda "aislado" y protegido (encapsulado) y no se ejecutará de forma automática; solo se activará cuando lo llames explícitamente por su nombre desde otra parte de tu script.
- **Ventajas profesionales:**
  - Evita la duplicación de código (Principio DRY: Don't Repeat Yourself).
  - Facilita la detección de errores (si el cálculo del precio falla, arreglás la función una sola vez y se soluciona en todo el sitio).
  - Vuelve al código limpio, ordenada y fácil de leer para tus compañeros de grupo.

---

#### 19.2 Declaración e Invocación de Funciones Tradicionales

Para trabajar con funciones nativas en JavaScript, el proceso técnico consta de dos momentos obligatorios y secuenciales:

##### A) Declaración de la Función

Se utiliza la palabra reservada `function`, seguida de un nombre descriptivo en minúscula (usando la convención camelCase), paréntesis para las variables de entrada y llaves para encerrar las instrucciones.

- Estructura:
  function saludarUsuario() {
  console.log("¡Bienvenido a Aberturas Oeste!");
  }

##### B) Invocación o Llamado (Execution)

Escribir el nombre de la función en el código no hace nada si no la "despertás". Para ejecutar las instrucciones que tiene guardadas adentro, tenés que invocarla escribiendo su nombre exacto seguido de paréntesis obligatorios `()`.

- Estructura:
  saludarUsuario(); // Acá el navegador recién ejecuta el console.log

---

#### 19.3 Parámetros y Argumentos (Entrada de Datos)

Para que una función sea verdaderamente útil y reutilizable, debe ser capaz de procesar datos dinámicos y variables en lugar de valores fijos. Esto se logra mediante el uso de canales de comunicación:

- **Parámetros:** Son variables locales temporales que se declaran entre los paréntesis en la cabecera de la función. Actúan como "enchufes" o moldes vacíos que recibirán información externa.
- **Argumentos:** Son los valores reales y concretos que vos le pasás (le inyectás) a la función entre los paréntesis en el momento exacto de su invocación.

- Ejemplo práctico de estructura:
  // "nombreProducto" y "precio" son los parámetros (moldes)
  function mostrarDetalle(nombreProducto, precio) {
  console.log("Producto: " + nombreProducto + " - Precio: $" + precio);
  }

  // Pasamos los datos reales como argumentos al invocarla:
  mostrarDetalle("Puerta Aluminio", 230000);
  mostrarDetalle("Ventana Corrediza", 120000);

---

#### 19.4 Retorno de Valores (La Sentencia return)

Por defecto, cuando una función termina de ejecutar sus líneas de código, se destruye internamente y no le devuelve nada al flujo principal de tu programa. Si necesitás que la función realice un cálculo matemático y te entregue el resultado final para guardarlo en una variable, tenés que usar la palabra clave `return`.

- **Regla estricta del return:** La instrucción `return` finaliza inmediatamente la ejecución de la función de forma quirúrgica. Cualquier línea de código que escribas adentro de esa función abajo del `return` será completamente ignorada por el navegador (código muerto).

- Ejemplo de cálculo integrado:
  function calcularTotalConIva(precioBase) {
  let total = precioBase \* 1.21;
  return total; // Envía el resultado final hacia afuera de la función
  }

  // Capturamos el valor retornado guardándolo en una constante nueva:
  const precioFinalPuerta = calcularTotalConIva(230000);
  console.log(precioFinalPuerta); // Imprime 278300

### Capítulo 20: El DOM (Document Object Model) - Cómo capturar y modificar elementos HTML en tiempo real

#### 20.1 ¿Qué es el DOM y cómo funciona?

El DOM (Document Object Model o Modelo de Objetos del Documento) es una interfaz de programación de aplicaciones (API) que el navegador crea de forma automática en la memoria de la computadora apenas carga un archivo HTML.

- **La estructura en árbol:** El navegador toma tu código HTML jerárquico y lo transforma en un árbol de nodos interconectados. En este modelo, absolutamente cada elemento, etiqueta, atributo o fragmento de texto se convierte en un "objeto" viviente al que JavaScript puede acceder de forma directa.

- **El superpoder de la interactividad:** Gracias al DOM, JavaScript puede actuar de forma quirúrgica sobre la interfaz: tiene el poder de cambiar textos, alterar estilos CSS de un elemento en base a una acción, borrar componentes viejos o inyectar etiquetas completamente nuevas (como cuando se renderiza una fila nueva en la lista de compras del carrito).

---

#### 20.2 Métodos de Captura o Selección de Elementos

Para que JavaScript pueda modificar una etiqueta que declaraste en tu estructura HTML, primero necesita "apuntar" hacia ella y capturarla en una variable dentro del script. Para lograr esto, el objeto global `document` provee los siguientes métodos técnicos estándar:

##### A) document.getElementById()

Busca y selecciona el único elemento de la página web que coincida de forma exacta con el valor del atributo `id` especificado entre los paréntesis.

- Estructura: `const listado = document.getElementById("carrito-listado");`
- Impacto técnico: Es el método más rápido y directo de captura debido a la naturaleza única de los identificadores.

##### B) document.querySelector()

Es un método moderno, flexible y extremadamente potente. Permite capturar el **primer** elemento de la página que coincida con un selector CSS completo (ya sea una clase, una etiqueta o una combinación anidada).

- Captura por clase (lleva punto): `const boton = document.querySelector(".btn-agregar");`
- Captura por etiqueta: `const titulo = document.querySelector("h2");`

##### C) document.querySelectorAll()

Busca y captura **absolutamente todos** los elementos de la página que coincidan con el selector CSS ingresado. Retorna una estructura técnica indexada llamada `NodeList` (muy similar a un array), que se puede recorrer con un bucle para aplicar cambios masivos.

- Estructura: `const todasLasTarjetas = document.querySelectorAll(".card");`

---

#### 20.3 Modificación de Propiedades y Contenidos del DOM

Una vez que capturaste un elemento en una variable, podés alterar sus propiedades internas de forma instantánea. Las herramientas más utilizadas en el desarrollo de aplicaciones son:

##### A) alteración de Texto (.innerText y .textContent)

Permiten leer o modificar el texto plano que se encuentra encerrado entre la etiqueta de apertura y la etiqueta de cierre de un elemento, sin interpretar código HTML intermedio.

- Estructura:
  `const contador = document.getElementById("contador-items");`
  `contador.innerText = "5"; // Cambia el número en la pantalla de forma inmediata`

##### B) Inyección de Código Estructural (.innerHTML)

Esta propiedad lee o reemplaza todo el contenido interno de un elemento interpretando de forma nativa las etiquetas HTML que le envíes. Es la herramienta clave que se utiliza para armar las plantillas dinámicas de los productos desde tu script.

- Estructura:
  `const contenedorCard = document.querySelector(".contenedor-aberturas");`
  `contenedorCard.innerHTML = "<h2>Puerta Aluminio</h2><p>Precio: $230.000</p>";`

##### C) Control de Clases CSS (.classList)

En lugar de escribir estilos CSS largos directamente con JavaScript (lo cual es una mala práctica), lo correcto es crear las clases visuales en tu hoja de estilos (`style.css`) y usar la propiedad `classList` para agregarlas o quitarlas según la lógica del programa:

- `elemento.classList.add("nombre-clase");` -> Añade una clase estratégica (ej: para mostrar una alerta).
- `elemento.classList.remove("nombre-clase");` -> Remueve una clase de la etiqueta (ej: para ocultar un modal).
- `elemento.classList.toggle("nombre-clase");` -> Comportamiento interruptor: si la clase no está la agrega, y si ya está puesta la saca (ideal para menús desplegables).

### Capítulo 21: Escucha de Eventos y Ciclo de Vida (addEventListener, clics, cambios de entrada)

#### 21.1 ¿Qué es un Evento en JavaScript?

Un evento es una señal técnica o notificación enviada por el navegador que indica que "algo ha sucedido" dentro de la página web, ya sea por una interacción directa del usuario o por un cambio de estado del propio sistema.

Los eventos son el puente definitivo que permite a JavaScript reaccionar ante el comportamiento humano. Algunos ejemplos cotidianos en interfaces son: cuando el usuario hace clic en un botón de "Comprar", cuando escribe su nombre en un campo de texto, o cuando desliza la rueda del mouse por la pantalla.

---

#### 21.2 El Escuchador de Eventos (addEventListener)

Para que JavaScript pueda capturar estas señales y ejecutar una tarea en consecuencia, se utiliza un método estándar de control llamado addEventListener (Escuchador de Eventos). Este método se acopla directamente sobre el elemento del DOM que queremos vigilar.

- Sintaxis y Parámetros: elemento.addEventListener("tipo_evento", funcion_a_ejecutar);

1. Tipo de Evento (String): El nombre técnico del evento que queremos escuchar (siempre se escribe en minúsculas y sin el prefijo "on"). Ejemplo: "click", "change", "input".
2. Función de Retorno (Callback): El bloque de código o función que el navegador mandará a ejecutar de forma automática estrictamente después de que el evento haya ocurrido.

- Ejemplo práctico estructurado:
  const botonAgregar = document.querySelector(".btn-agregar");
  function procesarClick() {
  console.log("Se hizo clic en el botón de agregar.");
  }
  botonAgregar.addEventListener("click", procesarClick);

---

#### 21.3 Eventos de Interacción Esenciales en e-Commerce

Para dar vida a un catálogo interactivo con carrito de compras, es indispensable dominar tres tipos de eventos fundamentales:

##### A) Evento "click" (Acción directa)

Se dispara cuando el usuario presiona y suelta el botón izquierdo del mouse sobre un elemento de la interfaz.

- Uso típico: Ejecutar la lógica de agregar un producto al array del carrito o abrir/cerrar la ventana del listado de compras.

##### B) Evento "input" (Monitoreo en tiempo real)

Se dispara de forma instantánea cada vez que el valor de un campo de texto cambia, es decir, con cada letra o número que el usuario escribe o borra en el teclado.

- Uso típico: Validar que el formato de un correo electrónico sea correcto mientras se escribe o filtrar las aberturas del catálogo en tiempo real a medida que el usuario tipea en la barra de búsqueda.

##### C) Evento "change" (Confirmación de estado)

A diferencia de input, el evento change no se dispara con cada letra, sino cuando el elemento pierde el foco de atención o cuando el usuario confirma una selección definitiva.

- Uso típico: Se aplica en listas desplegables (select) para detectar si el cliente cambió el filtro de ordenamiento de productos (por ejemplo, cambiar de "Menor Precio" a "Mayor Precio") o en los selectores de cantidad numérica de artículos dentro del carrito.

---

#### 21.4 Introducción al Ciclo de Vida y el Evento DOMContentLoaded

Cuando un usuario ingresa a una página web, el navegador lee el archivo HTML de arriba hacia abajo. Si tu script de JavaScript intenta capturar un elemento del DOM (como un botón) antes de que el navegador haya terminado de dibujar esa etiqueta en la pantalla, el script fallará arrojando un error crítico de tipo TypeError: cannot read properties of null.

Para solucionar este problema de sincronización y garantizar la estabilidad de la aplicación, el ciclo de vida del documento provee un evento fundamental:

- DOMContentLoaded: Este evento se dispara de forma automática directamente sobre el objeto global document en el instante preciso en que el navegador ha terminado de descargar, leer y armar la estructura completa del árbol de nodos HTML, sin esperar a que terminen de cargarse elementos pesados externos como imágenes o videos.

- Estructura profesional de seguridad:
  document.addEventListener("DOMContentLoaded", () => {
  console.log("El DOM está listo. Ya es seguro capturar elementos.");
  const boton = document.querySelector(".btn-agregar");
  boton.addEventListener("click", () => {
  console.log("Clic seguro");
  });
  });

### Capítulo 22: Estructuras de Datos Avanzadas - Objetos y Arrays de Productos

#### 22.1 Introducción a las Estructuras Complejas

Hasta ahora hemos trabajado con tipos de datos primitivos donde cada variable almacena un único valor aislado (un texto, un número o un booleano). Sin embargo, en el desarrollo de aplicaciones reales como un e-commerce, los elementos del mundo real poseen múltiples características interconectadas que no pueden separarse.

Para agrupar y organizar esta información de forma eficiente, JavaScript provee estructuras de datos complejas: los **Objetos** (para describir un elemento en detalle) y los **Arrays** (para agrupar colecciones de elementos).

---

#### 22.2 Objetos Literales (Estructura Clave-Valor)

Un objeto es una estructura de datos que permite agrupar múltiples variables y valores bajo un mismo contenedor único. Representa un elemento entidad (por ejemplo, un producto específico de tu catálogo).

- **Sintaxis:** Se declaran utilizando llaves `{}`. En su interior, la información se organiza estrictamente en pares de **Clave: Valor** (Key-Value), separados entre sí por comas.
- **Propiedades:** Cada clave declarada dentro de un objeto se denomina técnicamente "propiedad". Las propiedades actúan como etiquetas descriptivas del objeto.

- Ejemplo técnico de un producto:
  const producto = {
  id: "P01",
  nombre: "Puerta de Aluminio Blanca",
  precio: 230000,
  stock: 14,
  disponible: true
  };

##### Lectura de Propiedades (Notación de Punto)

Para acceder, leer o modificar el valor de una propiedad específica dentro de un objeto, se utiliza la Notación de Punto (`.`), conectando la variable del objeto con la clave deseada:

- Leer un valor: `console.log(producto.nombre); // Imprime "Puerta de Aluminio Blanca"`
- Modificar un valor: `producto.stock = 13; // Modifica el stock de forma directa`

---

#### 22.3 Arrays (Listas Indexadas)

Un Array (o arreglo) es una colección ordenada de elementos o datos estructurados en forma de lista. A diferencia de los objetos, los elementos dentro de un array no tienen una clave con nombre, sino que se ordenan de forma secuencial mediante un número de posición llamado **Índice (Index)**.

- **Regla del Índice Cero:** En JavaScript, las posiciones de los arrays se empiezan a contar estrictamente desde el número `0`. El primer elemento de la lista ocupa el índice `0`, el segundo el índice `1`, el tercero el `2`, y así sucesivamente.
- **Sintaxis:** Se declaran utilizando corchetes `[]` y los elementos se separan mediante comas.

- Ejemplo de lista básica:
  const marcas = ["Aluar", "Hydro", "Mesa"];
  console.log(marcas[0]); // Accede al primer elemento: Imprime "Aluar"

##### La Propiedad .length

Todos los arrays poseen de forma nativa la propiedad `.length`, la cual retorna un número entero que representa la cantidad total de elementos presentes en la lista en ese momento.

- Ejemplo: `console.log(marcas.length); // Imprime 3`

---

#### 22.4 La Estructura Maestra: Array de Objetos

En el desarrollo profesional de software, la forma estándar y más eficiente de representar una base de datos o un catálogo de productos es combinando ambas estructuras: un **Array que contiene Objetos adentro**.

Esta estructura compuesta permite que cada objeto actúe como una ficha de producto detallada, mientras que el array general los agrupa a todos en un solo listado ordenado que se puede recorrer y manipular fácilmente por código.

- Ejemplo integrado de un catálogo de aberturas:
  const catalogoProductos = [
  {
  id: "P01",
  nombre: "Puerta de Aluminio Blanca",
  precio: 230000,
  stock: 14
  },
  {
  id: "V02",
  nombre: "Ventana Corrediza 120x90",
  precio: 120000,
  stock: 8
  },
  {
  id: "P03",
  nombre: "Portón de Chapa Inyectado",
  precio: 450000,
  stock: 3
  }
  ];

##### Acceso Quirúrgico Combinado

Para leer un dato dentro de esta estructura mixta, se debe combinar el índice del array con la notación de punto del objeto:

- `console.log(catalogoProductos[1].nombre); // Apunta al segundo objeto e imprime "Ventana Corrediza 120x90"`
- `console.log(catalogoProductos[0].precio); // Apunta al primer objeto e imprime 230000`

### Capítulo 23: Métodos Modernos de Arrays para Procesamiento (Iterar, Buscar, Filtrar y Acumular)

#### 23.1 El Paradigma Declarativo en JavaScript Moderno

En versiones anteriores de JavaScript, para recorrer un listado de productos o filtrar elementos según su precio, era obligatorio utilizar el bucle `for` tradicional controlando manualmente los índices y contadores.

Hoy en día, el desarrollo profesional utiliza Métodos de Iteración Avanzados. Estos métodos son funciones nativas de los arrays que adoptan un enfoque declarativo: en lugar de escribir paso a paso _cómo_ tiene que recorrer el navegador la lista, simplemente le declaramos _qué_ queremos que haga con los datos. Todos estos métodos reciben como parámetro una función secundaria llamada Callback, la cual se ejecuta de forma automática para cada elemento del array.

---

#### 23.2 Métodos de Recorrido y Búsqueda

##### A) .forEach() (Iterar sin alterar)

Recorre el array de principio a fin y ejecuta la función callback para cada uno de los elementos de la lista. Se utiliza exclusivamente para realizar acciones externas individuales (como renderizar las tarjetas HTML de cada producto en el DOM), pero no retorna ningún valor ni modifica el array original.

- Estructura:
  catalogo.forEach(producto => {
  console.log(producto.nombre);
  });

##### B) .find() (Búsqueda quirúrgica de un elemento)

Recorre el array y retorna el **primer** elemento que cumpla con la condición lógica especificada dentro del callback. Si encuentra una coincidencia, corta la búsqueda de inmediato y devuelve el objeto completo. Si ningún elemento cumple la condición, retorna `undefined`.

- Uso típico: Buscar un producto específico del catálogo mediante su código `id` único cuando el usuario lo agrega al carrito.
- Estructura:
  const encontrado = catalogo.find(prod => prod.id === "V02");

---

#### 23.3 Métodos de Transformación y Filtrado

##### A) .filter() (Filtrado masivo)

Recorre el array y evalúa una condición lógica sobre cada elemento. Retorna un **array nuevo** compuesto exclusivamente por todos los elementos que hayan devuelto `true` en la condición. Si ningún elemento coincide, devuelve un array vacío `[]`. El array original se mantiene intacto.

- Uso típico: Filtrar el catálogo para mostrarle al usuario únicamente los productos que pertenezcan a una categoría o aquellos que tengan stock disponible.
- Estructura:
  const conStock = catalogo.filter(prod => prod.stock > 0);

##### B) .map() (Transformación y clonación)

Recorre el array, procesa cada elemento y retorna un **array nuevo** con la misma cantidad exacta de elementos que el original, pero con los datos transformados según las instrucciones del callback. Es una de las herramientas más potentes para manipular datos sin destruir la base original.

- Uso típico: Crear una lista con los precios actualizados tras aplicar un porcentaje de aumento por inflación o un descuento por promoción.
- Estructura:
  const preciosConIva = catalogo.map(prod => prod.precio \* 1.21);

---

#### 23.4 El Método de Acumulación

##### A) .reduce() (Reducción a un único valor)

Es el método más avanzado de procesamiento de arrays. Recorre la lista con el objetivo de procesar todos los elementos y compactarlos (reducirlos) a un único valor final de salida (que puede ser un número, un texto o un nuevo objeto).

Su sintaxis requiere dos parámetros principales dentro del callback:

1. **Acumulador (acc):** La variable temporal que va guardando y sumando el resultado acumulado vuelta tras vuelta.
2. **Valor Actual (curr):** El elemento del array que se está procesando en la vuelta actual.
3. **Valor Inicial:** Un número o dato que se coloca por fuera del callback (después de la coma) para indicarle al método en cuánto debe arrancar el acumulador.

- Uso típico: Calcular el valor total bruto de la compra sumando los precios de todos los artículos depositados dentro del carrito de compras.
- Estructura técnica integrada:
  const carrito = [
  { nombre: "Puerta", precio: 230000 },
  { nombre: "Ventana", precio: 120000 }
  ];

  // El 0 del final indica que el acumulador arranca en cero
  const totalCompra = carrito.reduce((acumulador, productoActual) => {
  return acumulador + productoActual.precio;
  }, 0);

  console.log(totalCompra); // Imprime 350000

### Capítulo 24: Persistencia de Datos - Memoria local (localStorage) y Traducción de Datos (JSON.parse/stringify)

#### 24.1 El Problema de la Volatilidad de la Memoria

Hasta este punto de la cursada, todas las variables, objetos y arrays de productos con los que trabajamos se almacenan de forma exclusiva en la memoria RAM del navegador. Esto significa que los datos son completamente volátiles: si el usuario recarga la pestaña, presiona F5 o cierra el navegador, el estado de la aplicación se destruye y el carrito de compras vuelve a quedar totalmente vacío.

Para lograr una experiencia de usuario fluida y real, las aplicaciones web necesitan persistir la información, es decir, lograr que los datos sobrevivan a los cierres de sesión y recargas de página.

---

#### 24.2 El Mecanismo de localStorage

`localStorage` es una API nativa del navegador que proporciona una base de datos web local integrada. Permite almacenar información directamente en el disco rígido del dispositivo del usuario de forma permanente, sin fecha de expiración. Los datos persisten incluso si la computadora se apaga o se reinicia.

- **La regla del almacenamiento:** Funciona bajo un sistema simple de almacenamiento de claves y valores (`Key-Value`). Cada dato guardado debe identificarse con una etiqueta única de texto.
- **Restricción Técnica Crítica:** `localStorage` **solo tiene capacidad para almacenar cadenas de texto plano (Strings)**. No puede guardar números nativos, booleanos, arrays u objetos directamente en su formato original; si intentás pasarle un objeto sin traducir, el navegador lo guardará roto bajo el texto inválido `"[object Object]"`.

##### Métodos de Control Esenciales:

- Guardar datos: `localStorage.setItem("clave", "valor_texto");`
- Recuperar datos: `let dato = localStorage.getItem("clave");`
- Borrar un dato específico: `localStorage.removeItem("clave");`
- Vaciar todo el almacenamiento local: `localStorage.clear();`

---

#### 24.3 Traducción de Datos con el Objeto JSON

Para evadir la restricción de almacenar únicamente texto y lograr guardar estructuras de datos avanzadas (como tu array `carrito` compuesto por objetos de aberturas), es obligatorio recurrir al objeto global **JSON** (JavaScript Object Notation).

JSON es un formato de texto ligero y universal para el intercambio de datos. El objeto de JavaScript provee dos métodos estáticos quirúrgicos para realizar la traducción bidireccional de datos:

##### A) JSON.stringify() (De Objeto a Texto)

Toma una estructura de datos compleja (un array o un objeto) y la traduce de forma exacta a una cadena de texto plano formateada como un String de JSON. Este proceso técnico se conoce en la industria como **serialización**.

- Uso típico: Transformar el array de compras en texto justo antes de mandarlo a guardar en el disco rígido.
- Estructura:
  const carrito = [{ nombre: "Puerta", precio: 230000 }];
  const carritoTexto = JSON.stringify(carrito);
  localStorage.setItem("carritoLocal", carritoTexto);

##### B) JSON.parse() (De Texto a Objeto)

Toma una cadena de texto con formato JSON (recuperada desde la memoria) y la reconstruye, decodificándola de vuelta a su tipo de dato original de JavaScript (un objeto o array nativo viviente). Este proceso técnico se denomina **deserialización**.

- Uso típico: Recuperar el carrito guardado apenas el usuario entra al sitio web para volver a computar las operaciones.
- Estructura:
  const datosGuardados = localStorage.getItem("carritoLocal");
  const carritoRestaurado = JSON.parse(datosGuardados);
  console.log(carritoRestaurado[0].precio); // Funciona de nuevo la notación de punto

---

#### 24.4 Flujo Integrado: El Ciclo de Persistencia Profesional

En un desarrollo profesional de e-commerce, la sincronización de la persistencia de datos sigue un flujo circular lógico y automatizado que combina la escucha de eventos con la traducción de objetos:

1. **Fase de Carga (Lectura):** Al dispararse el evento `DOMContentLoaded`, el script consulta inmediatamente a `localStorage` si existe un carrito previo guardado por el usuario. Si lo encuentra, lo decodifica con `JSON.parse()` y lo carga en la memoria RAM para dibujarlo en pantalla; si no existe, inicializa el array del carrito completamente vacío `[]`.
2. **Fase de Modificación (Escritura):** Cada vez que el usuario realiza una acción interactiva sobre el listado de productos (hacer clic en "Agregar Producto", "Eliminar" o "Vaciar Carrito"), el script actualiza primero el array en la memoria RAM y, de forma inmediata, ejecuta un guardado de respaldo convirtiendo la estructura con `JSON.stringify()` hacia el `localStorage`.

### Capítulo 25: Temporizadores y Dinámicas de Interfaz (setTimeout, alertas temporales y efectos dinámicos)

#### 25.1 Asincronismo Básico: El Control del Tiempo en la Web

Por defecto, JavaScript es un lenguaje de programación sincrónico y de un solo hilo (single-thread). Esto significa que ejecuta una sola tarea a la vez y no arranca la línea de código siguiente hasta que la actual haya terminado por completo.

Sin embargo, en las interfaces modernas necesitamos romper esa sincronía para ejecutar acciones en diferido o planificar tareas a futuro sin congelar la pantalla del usuario (asincronismo). Para lograr esto, el navegador nos provee herramientas nativas de control de tiempo llamadas Temporizadores, las cuales permiten programar la ejecución de funciones después de que transcurra un intervalo exacto de milisegundos.

---

#### 25.2 El Mecanismo de setTimeout()

El método `setTimeout()` es una función global del sistema que se utiliza para ejecutar un bloque de código o una función secundaria (callback) una única vez, luego de que haya transcurrido un período de tiempo específico.

- **Sintaxis y Parámetros:** `setTimeout(funcion_a_ejecutar, tiempo_en_milisegundos);`
- **La escala temporal:** El tiempo de espera se mide estrictamente en milisegundos (`ms`). Recordá siempre la equivalencia de conversión: **1 segundo es igual a 1000 milisegundos**. Por ende, si deseás configurar una espera de 3 segundos, debes ingresar el valor `3000`.

- Ejemplo de estructura básica:
  setTimeout(() => {
  console.log("Pasaron 3 segundos de espera.");
  }, 3000);

##### Cancelación Quirúrgica (clearTimeout)

Cuando ejecutás un `setTimeout()`, el navegador genera un número de identificación único para ese temporizador y lo deja corriendo en segundo plano. Si el usuario realiza una acción que vuelve innecesaria la tarea programada, podés frenar el reloj antes de que se cumpla el tiempo usando el método `clearTimeout(id_del_temporizador)`.

---

#### 25.3 Dinámicas de Interfaz: Alertas Temporales de Compra

La aplicación más importante de los temporizadores en un catálogo o e-commerce es la gestión de componentes dinámicos de realimentación (feedback), como los carteles flotantes o notificaciones tipo "Toast" que avisan: _¡Producto agregado al carrito con éxito!_

Dejar un cartel de alerta clavado permanentemente en la pantalla arruina la estética y tapa los productos. El flujo interactivo correcto utilizando temporizadores sigue estos pasos técnicos en la interfaz:

1. **El Disparador:** El usuario hace clic en el botón "Agregar al Carrito".
2. **La Activación:** La lógica de JavaScript captura el evento, busca el div de la alerta flotante en el DOM y le inyecta una clase CSS (por ejemplo, `.alerta-visible`) utilizando `classList.add()`. Esto hace que el cartel aparezca de forma fluida con una transición.
3. **El Temporizador:** Inmediatamente abajo, se programa un `setTimeout()` configurado para ejecutarse de forma automática a los 2500 milisegundos (2.5 segundos).
4. **La Desactivación:** Al cumplirse el tiempo de espera, la función callback del temporizador se despierta y remueve la clase visual usando `classList.remove(".alerta-visible")`, logrando que la notificación desaparezca sola de la pantalla sin que el usuario tenga que cerrarla a mano.

---

#### 25.4 Introducción a setInterval() (Flujos en Bucle)

A diferencia de `setTimeout()` (que se ejecuta una sola vez y muere), JavaScript provee otro temporizador nativo fundamental para dinámicas cíclicas: `setInterval()`.

- **Funcionamiento:** Ejecuta la función callback de forma repetitiva e infinita cada vez que se cumple el intervalo de tiempo configurado. No se detiene nunca por sí solo.
- **Uso típico:** Se emplea para crear componentes de la interfaz que requieren actualización constante en tiempo real, como carruseles de imágenes de ofertas que pasan solas cada 5 segundos, contadores regresivos de ofertas por tiempo limitado o relojes digitales instalados en el sistema.
- **Control de frenado:** Al igual que el temporizador simple, se debe almacenar el ID del intervalo en una variable para poder destruirlo y frenar el ciclo repetitivo invocando a la función `clearInterval(id_del_intervalo)`.
