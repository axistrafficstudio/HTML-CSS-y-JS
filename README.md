# REPASO-HTML-XERO9D
 
 El archivo index.html debe llamarse SIEMPRE así para que el servidor web (cuando la web sea pública en internet) sepa qué archivo debe cargar por defecto.

Los elementos HTML se pueden conformar de una etiqueta o de dos.

Dependiendo del tipo de elemento de HTML al que nos refiramos estos contendrán otros elemenos de HTML u otro contenido.

Las etiquetas <meta> de HTML siempre se encontrarán en el <head></head> del documento y valdrán para configurar ciertos aspectos técnicos de la web así como la carga de otros archivos externos. Hay dos que son obligatorias en la estructura de cualquier archivo HTML:
    - La etiqueta <meta> de codificación. Para cargar el set de caracteres que necesitaremos en la web.
    - La etiqueta <meta> para indicar al navegador que la web es responsive. name="viewport"

Para activar el "word wrap" -> Al+Z

Para abrir la web en el navegador:
    - Botón "Go Live" en la interfaz de Visual abajo a la derecha.
    - Click Derecho sobre cualquier archivo de la web y "reveal in file explorer"

En el primer nanosegundo en el que abrimos la web en el navegador vamos a abrir también las DevTools con F12 o Click Derecho "Inspeccionar".

Los elementos de TML que va a rendereizar el navegador SIEMPRE se encontrarán dentro del elemento <body></body>, algunos serán visibles para el usuario y otros no. 

AÑADIR ESTOS ELEMENTOS AL HTML:

- Un subtitulo.
- Un sub-subtitulo.

- Un párrafo y dentro del párrafo, que una palabra o varias sean un enlace clickable a la Wikipedia. <p> <a href="url">
- Otro párrafo y dentro una palabra en negrita y otra en cursiva. <strong><em> / NO USAR <b></b>/<i></i> (DEPRECATED)
- Otro párrafo y dentro un salto de línea. <br>
Para los párrafos copiar texto de Wikipedia o Lorem Ipsum.

- Una lista desordenada de lo que queramos. <ul>
- Una lista ordenada de números (con el texto en inglés). <ol>

-----

- Descargar una imagen (jpg o png o webp) y conventirla en un enlace a un artículo de Wikipedia / Meter un <img src="dirección/imagen.png"> Dentro de un <a href="url"></a>

- Agrupar 2 de los 3 párrafos anteriores dentro de otro elemento de HTML que funcione como un contenedor. <div> <section>: La diferencia entre ambas es que el div es un contenedor sin más, el section es un contenedor semántico, por lo que el navegador le aplica prioridades

Recomienda hacer commit cada vez que subimos fotos/archivos

En los <img src="" alt=""> el alt es el texto alternativo de la imagen y debe de describir la imagen bien, esto es importante para el SEO ya que Google se basa, entre otras cosas, en estos alt para las búsquedas, por lo que es más probable que si alguien busca "Patapon", le salga la img de mi web

COMANDOS:
Alt + Flechas arriba o abajo : MUEVE LAS LÍNEAS DE CÓDIGO ARRIBA O ABAJO

REPASO CSS

CLASE REPASO 3

VW y VH:
Viewport Width Medida relativa de anchura al tamaño de la pantalla del usuario
Funciona como un % pero relativo al viewport del usuario.

Viewport Height Medida relativa de altura al tamaño de la pantalla del usuario

La diferencia de esta medida con la medida % es que los %'s hacen referencia al tamaño del contenedor o elemento padre.

EM y REM:

Dos medidas relativas al font size

Em relativo al tamaño del font size del contenedor padre. 




## CREAR UN LAYOUT RESPONSIVE

Para crear un layout responsive y que tenga sentido en nuestra web debemos usar contenedores para organizar el contenido de la web. 

Estos contenedores

## FLEXBOX

Gúia flexbox https://css-tricks.com/snippets/css/a-guide-to-flexbox/ 

## MEDIA QUERIES

Para realizar ajustes sobre un layout adaptativo, que habremos maquetado usando propiedades de Flexbox o de Grid, usaremos las media-queries.

Se trata de una regla especial de CSS que me permite detectar el tamaño del ancho de la pantalla del usuario y sobreescribir ciertos selectores y propiedades que me interesen para adaptar mi interfaz o layout.

Estos media-queries siempre se encontrarán al final del archivo de CSS debajo de mi código de CSS base.

## GRID CSS LAYOUT

Grid al igual que flexbox, no es más que un conjunto de propiedades para desarrollar interfaces adaptativas y responsive.

La estructura que debemos tener en nuestro html para usar las propiedades de Grid, es la misma que en Flexbox, es decir, un contenedor (que será nuestro contenedor grid) y una serie de elementos hijos.

En nuestra web, podremos maquetar algunas partes con las propiedades de Flexbox, y otras partes con Grid. 

## TRANSITION:

La propiedad transition me permite crear una transición animada entre dos estados de algún elemento.

## TRANSFORM:

La propiedad transform es una propiedad especial que toma como valores, funciones de css, que me permiten modificar la forma, el tamaño, la posición, la rotación etc... de un elemento de forma fija o a través de un efecto :hover.

## ANIMATION

Las animaciones de CSS me permiten crear interpolaciones entre fotogramas clave. 

1) Definir animación con @keyframes, y darle un nombre con sentido lógico.

2) Aplicar la animación a un elemento con la propiedad animation

CTRL + Ç PARA AUTOCOMENTAR ALGO

## JAVASCRIPT (JAVASCRIPT NATIVO O VANILLA JS)

Es el único lenguaje de programación que funciona en el lado del cliente. 

JS es interpretado por el navegador y no necesita ser compilado (lo que le hace ser más rápido y eficiente). 

Javascript es un lenguaje débilmente tipado. 

3 formas diferentes de añadir código de JS a nuestro HTML (nuestra web).

1) Directamente en los elementos HTML. Mediante atributos de tipo evento podemos llamar a funciones de JS pero esta forma no es la más correcta.

2) Usando el elemento de HTML <script></script> que me permite añadir código de JS dentro del elemento. Podemos cargar este elemento y el código de JS en el <head> de nuestro HTML (esto lo reservaremos normalmente para cargar librerias de JS).

Esta etiqueta <script></script> también se puede encontrar justo antes de cerrar el <body></body> esta forma es la más correcta de cargarlo en el <head> ya que permite que se haya cargado todo el código de HTML previamente. 

3) Enlazar un archivo externo de JS a nuestro HTML.

## VARIABLES DE JS

Para declarar una variable de JS (v5) usaremos la palabra reservada -> var 

1) Declaramos la variable y le damos un nombre.

2) Le asignamos un valor a la variable con el simbolo = 

3) Llamar a la variable o invocarla (invoke) o hacer referencia (reference) 

A las variables se les puede reasignar un valor nuevo tantas veces como sea necesario. 

Las variables pueden contener letras, números y _ (guión bajo).

Actualmente, en la versión (v6) de JS, existen 2 formas nuevas de declarar variables:

- let (sustituye a var)
- const -> Este tipo de variables (constantes) no permiten re-asignar un nuevo valor. 

TIPOS DE DATOS EN JS:

- String (cadena de carácteres o texto) -> puede contener: letras, números, carácteres especiales y espacios. Siempre estará contenido entre comillas dobles o simples dependiendo de la situación.

- Number (números) -> tenemos 2 tipos de números: los enteros (int o integer) y los decimales (float). Los números decimales SIEMPRE con un (.) no con (,)

- Boolean (booleano) -> Verdadero o Falso (true or false) 

- NaN -> Not a Number: Es un tipo de dato que aparecerá como resultado cuando intentemos hacer un cálculo y JS no sepa resolverlo.

- Array (lista) [] -> Se trata de un tipo de dato que me permite crear un conjunto de otros tipos de datos. Estos elementos de un Array, pueden ser todos del mismo tipo, o de diferentes tipos.

- Object (objeto) {} -> Son un tipo de dato complejo que me permite guardar de forma ordenada otros tipos de datos siguiendo el formato -> clave: valor, (key-value). Todos los tipos de datos introducidos dentro de un objeto acaban en , y no en ;

## Comparaciones de JS:

- Mayor que >
- Menor que <
- Mayor o igual que >=
- Menor o igual que <=
- Igual que == (comparación no estricta o débil)
- Totalmente igual que === (comparación estrica, no solo compara el valor del dato si no el tipo de dato, no es lo mismo un var = 3 que un string = 3)
- Diferente que !=
- Totalmente diferente !== (compara por tipo de dato también)

## Operadores Lógicos o Puertas Lógicas:

- AND lógico -> &&
- OR Lógico -> || 
- NOT Lógico -> !

## Funciones de JS:

Una función (o método) es un conjunto de instrucciones en forma de líneas de código que cumplen un trabajo determinado. 

Las funciones de JS trabajan como una "caja negra". 
Nosotros llamamos o usamos una función porque sabemos qué es lo que hace, pero internamente no sabemos cómo funciona. Esto en el caso de que usemos ya definidas. 

Existen funciones que trabajan dándonos simplemente un output o resultado de su trabajo y existen muchas otras funciones que admiten o necesitan un input para poder trabajar y darnos un output.

Tenemos dos tipos de funciones en JS:

1) Las funciones de JS ya definidas en el core del lenguaje que nosotros podemos usar para hacer un trabajo determinado. Por ejemplo, las funciones alert() y log(), son funciones de este tipo que se conocen como funciones built-in.

2) Las funciones de JS que nosotros mismos podemos definir desde cero con nuestro popio código. Estas funciones una vez declaradas las podremos usar tantas veces como necesitemos.

Instrucciones para crear y usar una función propia:

1. Declaramos la función con la palabra reservada function:

2. Le damos un nombre a la función. Dicho nombre lo decidimos nosotros y debe representar de forma clara el trabajo que realizará dicha función. El nombre de la función incluye unos paréntesis al final.

3. Escribir el código o la lógica de la función.

4. Usar la función llamándola o invocándola.

Para que una función acepte parámetros de entrada, debemos definirlos en el paréntesis de la declaración de la función.

## SELECTORES DE JS:
Con los selectores de JS podemos seleccionar elementos del HTML y modificarlos, o manipularlos.

Para JS el HTML se representa en forma de árbol de nodos conocido como DOM (Document Object Model).

- La variable global document (que se genera al cargar la web automáticamente), contiene todo el HTML y podremos seleccionar diferentes elementos usando los selectores de JS.

 - getElementsByTagName() -> Selecciona uno o varios elementos que coincidan con el nombre de la etiqueta de HTML que le pasamos como parámetro a la función. 
 ESTA FUNCIÓN DEVUELVE SIEMPRE UN ARRAY.

- getElementsByTagClass() -> Selecciona los elementos por clase y devuelve un ARRAY.

- getElementsByTagId() -> Busca un id en el DOM y devuelve el elemento con ese id.

Selectores tipo query con sintaxis de CSS:

- querySelector() -> Selecciona un elemento y recibe como parámetro un selector de tipo CSS (si este selector coincide con varios elementos del HTML seleccionará el primero). PARA SELECCIONAR PARÁMETROS DE CSS:

1) SI QUIERO UN ID USAMOS UN # PRIMERO

2) SI QUIERO UNA CLASE USAMOS UN . PRIMERO

- querySelectorAll() -> Lo mismo pero para seleccionar más de un resultado, el resultado aparecerá en forma de ARRAY.

## SETTERS Y GETTERS DE JS

Tenemos en todos los elementos de HTML diferentes propiedades de las cuales podemos obetener su valor (get) o modificar y asignar nuevos valores (set). 

EVENTOS DE JS:

Los usuarios dentro de las páginas web pueden "disparar" (trigger) diferentes eventos. Mediante JS podemos "capturar" estos eventos y hacer algo en respuesta. Algunos ejemplos de eventos:

- Detectar cuando se ha cargado completamente el HTML.
- Detectar cuando el usuario hace click sobre un elemento (también existe el evento doble click).
- Detectar cuando el usuario hace scroll (sobre toda la web o sobre un elemento determinado).
- Detectar cuando un campo input cambia de valor.
- Detectar cuando el cursor pasa por encima de un elemento -> Con JS podemos diferenciar cuándo el cursor entra encima del elemento y cuándo sale del área del elemento.