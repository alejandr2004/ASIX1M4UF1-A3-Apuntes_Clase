# ASIX1M4UF1-A3-Apuntes_Clase
Aquí subiré los apuntes de clase progresivamente.
Comenzaré por el bloque de Markdown.
Voy a explicar como modificar textos con diferentes tipos de letras.
Para escribir en cursiva en Markdown necesitaremos escribir dos * en forma de opertura y cierre. Un ejemplo: *Buenos dias*,*Hoy hace 
frío*
También sirve el uso de guiones bajos _ .Ejemplos: _Hoy es martes_,_Mañana nevará_.
Para escribir en negrita haremos uso de dos ** o de dos __. Ejemplos: **Buenas tardes**,__El dia es triste__.
También podemos hacer un uso combinado de las dos (negrita y cursiva).Esto lo realizamos con _* en la apertura y *_ en el cierre.Ejemplos:_*Hola*_,_*Ahí*_

En Markdown podemos hacer listas ordenadas y desordenadas(al igual que CSS).
Para realizar una lista ordenada simplemente deberemos numerar al lado del elemento y, automáticamente, el número se volverá azul
(entendiendo que es una lista).Ejemplo:

1. Primera opción de menú
2. Segunda opción de menú
3. Tercera opción de menú

Como se ve en el ejemplo deberemos ir numerando progresivamente cada elemento, de uno en uno, asegurándonos de no saltarnos ningún 
punto.

Como he dicho anteriormente, también existe la posibilidad de  crear listas desordenadas (conocidas en html con la etiqueta<ul>), estas 
están compuestas de asteriscos * o guiones -.Ejemplos:

* Primera opción de lista desordenada
* Primera opción de lista desordenada
- Primera opción de lista desordenada

Como se puede ver, no es necesario llevar ningún orden en concreto y se pueden intercalar asteriscos y guiones indistintivamente.

Se pueden intercalar listas ordenadas y desordenadas, esto puede servir para hacer índices o subpuntos.Ejemplo:

* Primera opción de lista desordenada
* Primera opción de lista desordenada
- Primera opción de lista desordenada
  1. Primer submenú
  2. Segundo submenú
 -Cuarta opcion de lista desordenada
   - Tercer submenú
   - Cuarto submenú

Como se puede ver no hay ningun problema en su uso y combinación, estas son complementarias y servirían para hacer trabajos más 
extensos.

El uso de Markdown no se quedaría aquí, tienes todavía bastantes funciones que nos pueden resultar de utilidad como, por ejemplo, las 
tablas

Las tablas son un conjunto de filas y columnas que sirvan para diversidad de cosas.Primero voy a definir como realizar columnas y, a 
continuación, filas.

Para hacer columnas utilizaremos estas barras || para delimitar la amplitud de la tabla.Con un ejemplo se verá mucho más claro:

|Primera columna|Segunda columna|3 columna|

Como podemos ver, se pueden ir añadiendo elementos a la columna como lo vayas considerando necesario.

Para hacer una tabla completa y por tanto filas, deberemos tener algunos aspectos importantes en cuenta. El primero de ellos será que 
*la anchura de la filas más largas determinará la longitud de esta*.Eso quiere decir que el esquema de la tabla se adaptará a la fila 
con más texto, esta es una medida lógica ya que, sinó, habría texto que se saldría de la propia tabla.

Para realizar las columnas necesitaremos escribir *justo en la línea debajo de otra fila*, así habrá un conjunto de filas, una encima 
de otra, que formarán un conjunto de columnas.Con un ejemplo será mucho más visual:


 |Primera columna|Segunda columna|3 columna|
 |---------------|:------------:|---------:|
 |Col 2 es|Centrada|35 euros|
 |Col 3 es |Derecha|134 euros|
 |Estilo cebra|Gris|Blanco|
 |Clase|ASIX1|M4|

Como se aprecia en el ejemplo, la primera fila es la más grande lo que delimitará la amplitud de la tabla, la segunda fila justo denajo 
nos sirve como referencia de esta amplitud y, las otras filas no deberán rebasar esta amplitud sinó se modifica la tabla.
Las demás filas y columnas son un mero ejemplo, se podría rellenar de cualquier forma y con cualquier dato de relevancia.

Por último en el bloque de markdown hablaremos de _la selección de opciones_, con esto me refiero a un listado de opciones (opcion A, 
opcion B, opcion C,opcion...) en la cual seremos capaces de seleccionar una o varias de estas. Esto se hace escribiendo varias lineas 
de texto y, al incio de estas deberemos dejar corchetes vacíos []. Esto lo que indica es que esta opción está disponible para ser 
marcada, se dejarán tantos corchetes como opciones haya.
Ahora, y para marcar la opción que mas nos convenga, deberemos rellenar los corchetes con una cruz, de esta manera: [X]
Como siempre digo, con un ejemplo se verá mucho más claro:


 -[ ] Opcion A
 
 -[X] Opcion B

 -[ ] Opcion C


 Vemos un total de tres opciones guionizas y tres corchetes.En este caso,solo *uno de ellos* está  marcado con una cruzeta y los demás 
 no, pero se podrían dar diferentes casos como que todas estén marcadas o ninguna dependiendo de tus necesidades.
 Aquí veo la posibilidad de intercalar listos ordenadas y desordenadas, donde podremos marcar y desmarcar los ítems, todo queda a la 
 imaginación del usuario.Cabe decir que la mayoría de medidas se pueden COMPLEMENTAR (se puede combinar el uso de negrita con las 
 listas o tener diversas opciones  marcar en una tabla) y hay pocos procesos que solo se puedan aplicar por separado.
 
 _*Con esto doy por finalizado el bloque de Markdown.*_

 BLOQUE DE HTML

 Como el archivo README se encuentra en formato Markdown muchas etiquetas de html no estarán disponibles así que utilizaré un recurso 
 que lo interpretará como código externo pero igualmente lo mostrará todo: los accentos abiertos.Estos permiten delimitar un código 
 *que no sea de Markdown* y lo muestra como código.Lo iré utilizando en este bloque y su uso se comprenderá mejor.

 Comenzaremos con lo más básico y sencillo, TODOS los archivos tml están compuestos por un <head> y un <body>. En el head se ponen 
 archivos relativos al formato que *el usuario de la página web no podrá ver*.En ese bloque se interactua con aspectos exteriores a 
 como se verá la página web. En el bloque body SÍ se escribirá todo lo relativo a *lo que el usuario podrá ver*(texto de la página,
 enlaces,imágenes...).Es muy importante no equivocarse de bloque ya que cada uno adopta funciones MUY diferentes.

 Ahora mostraré como se ven los dos bloques en un archivo html 5 común:
 ```
 <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  </head>  
```
Como se puede ver, de fábrica, solo incluye metadatos que permiten un tipo específico de caracteres (UTF-8) y la forma de visualización 
(content="width=device-width) que muestra los datos adaptados a la amplitud de la pantalla del dispositivo.
Se pueden añadir diferentes atributos y etiquetas que veremos más adelante

```
<body>
<h1>Mi primera página HTML</h3> 
<h2 id="Índice de contenidos">Índice de contenidos</h5>
<ul>
    <li><a href=#HTML>HTML</a></li>
    <li><a href=#Laprimeraweb>La primera web</a></li>
    <li><a href=#Bibliografíayenlaces>Bibliografía y enlaces</a></li>
</ul>

<h2 id="HTML">HTML</h2>
</body>
```
La parte del body viene vacía pero en este ejemplo he añadido algunas etiquetas básicas que explicaré:
La etiqueta h1 permite establecer un texto como encabezado y le establece un tamaño.Este tamaño será más grande o más pequeño 
dependiendo del número asociado a la etiqueta h (hay de h1 a h6, de manera que h1 es la etiqueta más grande y h6 la más pequeña).
Como he dicho html funciona con *etiquetas* pero es importante saber que dentro de diversas etiquetas se pueden establecer *atributos*.
Estos, de cierta forma, se encargan de modificar una etiqueta(a continuación lo veremos claro con el ejemplo)
La etiqueta h2 en el caso del ejemplo contiene el atributo "id" que servirá para referenciar un elemento en específico que estará más 
adelante dentro de ese body.
Todas las etiquetas que hay dentro de este body las explicaré más adelante ya que el único uso que quería darle ha sido para explicar 
como sería un "body" en la práctica.

Antes de continuar debo hacer un inciso sobre las etiquetas, y es que estas tienen una opertura body y un cierre /body.Este cierre 
se hace escribiendo una barra / y el nombre de la etiqueta (cabe resaltar que también hay etiquetas autocerrables).

Ahora que sabemos como se estructura un archivo html hablaremos de sus diversas etiquetas. Comenzaremos con un elemento que también se 
hallaba en Markdown:las listas.

Estas pueden ser tanto ordenadas <ol> como desordenadas <ul>.Lo bueno de html es que conforme vayas escribiendo dentro de las etiquetas 
este se encargará de numerar u ordenar automáticamente.Ahora explicaré la diferencia entre ambas:
Las listas ordenadas <ol> *se encargarán de numerar* los ítems que haya dentro de una lista a partir del 1 de forma progresiva (1,2,3,
4...) mientras que las desordenadas <ul> *las marca con guiones o puntos*.
Es necesario aclarar que los ítems de una lista se establecerán con <li> (list items) que serán hijas de <ol> o <ul> (el concepto de 
hijo y descendiente lo explicaré más adelante).
Ejemplo de lista:
```
<ol>
    <li>Historia de la web</li>
    <br>
        <ul>
            <a href="https://www.nobbot.com/el-origen-de-la-world-wide-web-%C2%BFcuando-nace-y-quien-la-inventa/" target="_blank">○	Historia de World Wide Web: cuándo nace y quién la inventa (nobbot.com)</a>
            <br>
             <a href="https://es.wikipedia.org/wiki/Historia_de_la_World_Wide_Web" target="_blank">○ Historia de la World Wide Web - Wikipedia, la enciclopedia libre</a>
            <br>
             <a href="https://www.bbvaopenmind.com/tecnologia/visionarios/tim-berners-lee-y-el-origen-de-la-web/" target="_blank">○	Tim Berners-Lee y el origen de la Web | OpenMind (bbvaopenmind.com)</a>
            <br>
            <br>
        </ul>  
    <li>HTML</li>
        <br>
        <ul>
            <a href="https://es.wikipedia.org/wiki/HTML" target="_blank">○ HTML - Wikipedia, la enciclopedia libre</a>
            <br>
            <a href="https://developer.mozilla.org/es/docs/Learn/HTML/Introduction_to_HTML/Getting_started" target="_blank">○Empezar con HTML - Aprende desarrollo web | MDN (mozilla.org)</a></il>
        </ul>         
</ol>
```

Aprovecho para explicar un concepto bastante importante del orden dentro de un html: la sangría. Esta se encarga de establecer, de 
forma clara _para el lector_ *que orden y valor tiene una etiqueta dentro de ese html*. En el ejemplo de arriba se ve donde empieza y 
acaba cada etiqueta (no creo que sea un ejemplo perfecto pero todavía estoy aprendiendo).Esto facilita la comprensión a cualquier 
persona que quiera ver o modificar algo del código.También existe la opción de agrupar varios grupos de código en pestañas ,
esto depende de como se organice cada uno pero suele facilitar bastante la lectura en códigos largos o densos.

Antes de continuar explicaré algunas etiquetas que considero básicas dentro de html:

-La etiqueta <p> que establece el formato párrafo y que deja una linea entre el siguiente trozo de texto.

-La etiqueta <br> que establece una línea de espacio en el texto
<br>;)
-La etiqueta strong que establece el texto en negrita

-La etiqueta hr (horizontal line) escribe una línea horizontal

-La etiqueta blockquote que sirve para citar

Y para comentar se escribe dentro de este bloque <!-- -->. Ejemplo <!--Mario RPG tiene una dificultad demasiado baja-->

Estas són algunas que yo conozco pero hay muchísimas más (con estas bastará para iniciar)

Por cierto, quiero aclarar ya que considero esto un aspecto básico pero también que hay que conocer, hay un par de líneas de código que 
se establecen fuera de los bloques <body> y <head>:

-<!DOCTYPE html> que indica el tipo de navegador que es.

-<html lang="en"> que indica que el contenido de esta página va a estar en inglés (esto en este caso ya que se puede cambiar)

Es importante recordar que TODOS LOS VALORES TIENEN QUE ESTAR DELIMITADOS POR LAS ETIQUETAS, es decir, se tiene que escribir entre el 
inicio de la etiqueta y el cierre (prefiero recordarlo porque es algo crucial)

Ahora explicaré un campo que funciona de manera similar en Markdown como en html así que he decidido explicarlo aquí una sola vez: 
referenciar imágenes.
Para ello usaremos la etiqueta <img> y dentro de ella usaremos el atributo src en el cual con comillas introduciremos la url de la 
imagen (en Markdown lo único que hay que hacer es escribir el nombre de la imagen y la url).

Ahora que hemos hablado de rutas y url me parece un buen momento para hablar de la estructura de carpetas.

Si tienes una imagen dentro de un archivo html será importante que la referencias utilizando su *ubicación relativa*. ¿De que trata 
esto? La ubicación relativa es aquella que hace referencia *al sitio en el que nos ubicamos a la hora de buscar la url*.Con un ejemplo 
se verá mucho más claro. Pongamos que estoy en raíz / dentro del repositorio(cabe aclarar que el primer archivo siempre será .html) y 
quiero acceder a la carpeta imágenes. En este caso debería referenciar la carpeta imágenes a partir de raíz, para marcar donde te 
ubicas en html se utiliza "./" y justo después de la barra donde te quieres dirigir, en ese caso, para acceder a la carpeta imágenes 
debería hacer lo siguiene:"./imágenes"( esto es un ejemplo pero en la realidad es importante que los nombres de las carpetas no 
contengas espacios ni accentos).
Pongamos otro ejemplo: dado el caso en el que me ubico dentro de imágenes y quiero referenciar algo del html inicial, en esta situación 
debería "salir" a una carpeta exterior,¿verdad?. Para eso utilizaremos "../" que nos permite indicar una carpeta exterior (si se 
quieren indicar varias carpetas exteriores se utilizará este recuerso varias veces.Ejemplo:../../textoejemplo.jpg). Se referenciaría de 
la siguiente manera:"../1234.html".

Ahora explicaré las diferentes formas que existen de agrupar ítems o referenciarlos.

Existen tres selectores: id (único) de clase (varios) y universal (todos).

Si tenemos un título en una etiqueta h1 y queremos que este se vea de color azul (más adelante explicaré todo lo referente a estilos) 
deberemos referenciarlo de alguna forma esto lo haremos gracias a "id".Este es un *identificador único* en el que deberemos introducir 
con una almoadilla # como queremos que se reconozca. Ejemplo: tenemos un id=patata, para referenciarlo deberemos utilizar la almodilla 
(a href=#patata).

Una vez explicado el id, los otros dos selectores serán mucho más fáciles de entender.

El selector de clase permite agrupar varios elementos con un solo identificador. Simplemente deberemos escribir "." delante de el 
nombre al cual haremos referencia. Después de esto aplicaremos los cambios referenciando a ese identificador.

Por último el selector universal es el más simple. Consta de un "*" que afecta a TODO el archivo.

En nuestros archivos html muchas veces podemos sentirnos limitados por la escasa personalización de los elementos, esto se puede 
solucionar muy facilmente implementando elementos externos que permitan cambiar o dar algo de estilo a nuestros archivos.
Esto normalmente se consigue referenciando el recurso externo al <head> para así poder aplicar esos recursos a nuestro archivo base, 
ahora explicaré a que me refiero.
Estoy hablando de modificadores de formato, ya sea el uso de *favicons*, uso de fuentes de texto diferentes (google fonts es un 
ejemplo) entre otros.

Los favicons son, básicamente, el ícono que sale al lado de la pestaña de la página web abierta. Este se puede configurar en el <head> 
de la siguiente manera:
```
 <link rel="icon" href="/Imagenes/favicon.png" type="image/x-icon">
 ```

 Como podemos ver está establecido como "icon" (los favicons deben tener este formato), está referenciado dentro de ese html y el tipo 
 (type) es una imagen.
 Explico esto porque los favicons se pueden obtener también de páginas externas como puede ser "fontawesome".Ahora adjuntaré como se 
 vería en código.
 ```
 <script src="https://kit.fontawesome.com/c411388166.js" crossorigin="anonymous"></script>
 ```

 Aquí he utilizado un script de fontawesome que me permitía poner una flechita que luego yo configuré en mi html para que te regresase 
 al inicio.El script está puesto en el <head> y ahora me permitirá utilizar ese recurso en el <body>

Ahora explicaré un concepto que es bastante amplio y que afecta a muchos lenguajes de programación y no solo a html. Las etiquetas 
descendientes.

Muchas veces en nuestro código veremos que una etiqueta engloba a otra. Estos es algo normal ya que, normalmente, necesitaremos de un 
conjunto de etiquetas en un mismo código para lograr alguna función en específico. Cuando una etiqueta *está contenida por otra* la 
llamamos etiqueta hijo. Esto quiere decir que todo cambio que hagamos en la etiqueta padre (la que la contiene) también afectará a la 
etiqueta hijo. Es algo muy importante a tener en cuenta ya que puede modificar la estructura de nuestro html significativamente si no 
entendemos muy bien como funciona.
Se puede dar otro caso, cuando tenemos un conjunto de etiquetas que siguen al hijo, (es decir, están englobadas por la etiqueta hijo)
las llamamos descendientes. Pueden haber un conjunto de descendientes muy elevado, pero el único que recibe el nombre de hijo es aquel 
que es englobado del padre. Este es un concepto muy importante a la hora de referenciar dentro de un texto, ahora enseñaré por qué y 
como en un ejemplo:

```
body > div > p strong {
    background-color: rgba(255, 255, 255, 0.719);
    border-radius: 3px;
}
```

Ignoremos el contenido de las etiquetas, lo explicaré más adelante en estilos CSS. Vemos que la etiqueta <body> es la "padre" o la que 
engloba a todas. Dentro de ella está la etiqueta <div> que es la etiqueta hijo y, dentro de esta p y strong, las etiquetas 
descendientes. El signo mayor que > indica que aquello que viene después PERTENECE A LA ETIQUETA ANTERIOR, es decir <body> es poseedor 
de todas las demás etiquetas, en este caso.
Vemos que esta sintaxis no aplica en strong, y esto tiene un significado. Lo que está indicando es, TODO LO QUE CONTENGA LA ETIQUETA 
strong RESULTARÁ AFECTADO.Si esto sucediera en la etiqueta <div> estariamos indicando que, INDEPENDIENTEMENTE DEL ORDEN DE 
DESCENDENCIA (a partir de esa asignación), todas las etiquetas <div> sean afectadas.


En html y ,como también existe en Markdown, existen las tablas, aunque su sintaxis es bastante diferente.

Una tabla, en html, está compuesta por tres etiquetas esenciales: <thead>, <tbody> y <tfoot>

La etiqueta <thead> pertenecerá a todo aquello relacionado al encabezado de una tabla, <tbody> al cuerpo o contenido de esta y <tfoot> 
al pie de página o de la tabla por así decirlo.

Cada elemento que vayamos a escribir dentro de la tabla deberá contener la etiqueta <tr>, esto servirá de indicador para saber que esa línea de texto *pertenece a esa tabla*.
Una vez dicho esto deberemos estructurar cada <tr> en función de donde creas que  vaya a pertenecer dentro de la tabla.

Para que los elementos introducidos dentro de una tabla salgan bien estructurados y ordenados deberemos utilizar una etiqueta que 
variará en función de donde las ubiquemos (head, body o foot). Se utilizará  <th> tanto para el <thead> como para el <tfoot>, de esta 
manera, si queremos escribir elementos dentro de la etiqueta <tr> de forma secuencial y ordenada utilizaremos esa etiqueta. Ahora y 
para el <tbody> la cosa cambia un poco ya que la etiqueta utilizada será <td>.



Muchas veces nuestro código se ve saturado por el uso de demasiadas líneas de código dentro de un solo archivo html. Esto puede 
provocar que nos confundamos, cometamos errores o no entendamos muy bien como está estructurado. Sí, existen diferentes recursos dentro 
del propio html ( como los bloques de código que nos permiten plegar o despegar la información como queramos) pero muchas veces estos 
recursos se quedan cortos.

Hay un método para solucionar esto, evitar muchas líneas de código referenciando a un grupo o identificador dentro del head o del body, 
y esta es una de las funciones que cumplen los CSS externos.

CSS o Cascading Style Sheets es un archivo externo que nos permite hacer modificaciones dentro de cualquier archivo html que tengamos 
simplemente con referenciarlo en el head de nuestro archivo. Esto nos permite ahorrar muchas líneas de código dentro del html original 
y afectar a diferentes etiquetas sin tener que referenciarlas dentro del mismo archivo.


```
/* Regla 1 */
body {
    margin: 0;
    padding: 0 230px;
    font-family: Arial, sans-serif;
    background-image: url('https://piks.eldesmarque.com/bin/esports/2019/10/Banner_Preseason-1_dwfwpnp0byzkpe2hk65v.jpg');
    color: white;
    text-align: center;
    background-repeat: no-repeat;
    background-size: cover;
}
```


Esto de aquí es un ejemplo que saqué de un ejercicio en el que tenía que cumplir ciertas reglas para cambiar el estilo de un html. Como 
he dicho se trata de un archivo externo, y estas modificaciones afectarán al archivo al que se vincule. En este caso quise afectar a la 
etiqueta <body> con una serie de atributos, me centraré en explicar la lógica detrás y no el significado de los atributos: todos estos 
cambios que han sido realizados en el body afectarán a la etiqueta body del html interno en cuanto vincule el CSS con el archivo.

Para referenciar un archivo CSS haremos lo siguiente:

```

<link rel="stylesheet" href="./hojaexterna.css">

```

Esto se hará dentro del <head> del archivo. Aquí vemos que es una "stylesheet" u hoja de estilos y después su referencia dentro de mi directorio.


Gracias a este recurso podemos implementar "frameworks" que son trozos de código compilados por otros usuarios que nos pueden servir 
como ayuda o para ahorrar tiempo en nuestros proyectos.
En el caso de CSS tenemos Bootstrap, que nos permite integrar hojas CSS con una cantidad de clases definidas enorme, así nos ahorramos 
de crearlas (eso sí, deberemos saber que nombre recibe cada clase y que es lo que hace con exactitud para no equivocarnos con su 
funcionamiento). 

Muchas veces nos encontraremos que la personalización de nuestras páginas web es muy poco atractiva, esto se puede remediar con 
diferentes etiquetas que permiten modificar de muchas formas nuestras páginas web dotándolas de una presentación visual mucho más 
agradable.


```
/* Regla 10 */
.contenedor1 {
    background-color: rgba(255, 91, 91, 255);
    border: 2px solid black;
    border-radius: 5px;
    padding: 30px;
    margin-top: 20px;
    margin-bottom: 20px;
    color: black;
    line-height: 25px;
}
```

He vuelto a coger un fragmento de código de uno de mis trabajos, voy a explicar cada una de las etiquetas en el orden que se muestran:

-background-color: establece un color de fondo. Se puede definir escribiéndolo directamente después de los dos puntos
"background-colour:blue" o con rgb(red,green,blue) y sus diversas escalas de tonalidad que escalan de 0 a 255 "background-colour:rgb(0,
0,255)".Las dos son formas diferentes de expresar lo mismo:"background-colour:blue"= "background-colour:rgb(0,0,255)"

-border: puedes establecer diferentes propiedades del borde después de los dos puntos. En el caso del ejemplo establecí el grosor del 
borde (2px), el tipo de borde (solid) y el color (black).

-border-radius: establece el tamaño radial del borde.

Ahora quiero definir tres conceptos que pueden resultar confusos si no se explican correctamente:

-Border (explicación conceptual): elemento que define el perímetro.

-Margin: espacio de separación entre dos elementos.

-Padding: relleno.

Aclararo esto, continuemos con la explicación de la lista de conceptos anterior:

-margin-top: establece un espacio entre nuestro elemento y la parte de arriba.

-margin-bottom: establece un espacio entre nuestro elemento y la parte de abajo.

-color: cambia o establece un color.

-line-height: altura o tamaño de las líneas.

También podemos cambiar el tipo de letra (como expliqué antes se podría realizar perfectamente con un recurso de Google Fonts) 
utilizando "font-family".Ejemplo:

```

font-family: Arial, sans-serif;

```
Esto según donde lo apliques dentro del HTML podrá modificar una parte del texto en específico o toda



FLOAT Y DISPLAY FLEX


Estas son dos estructuras que nos permiten ordenar contenedores o "divs" a nuestro antojo.
Float permite seleccionar la estructura en la cual se irán posicionando los contenedores, pueden ser uno delante de otro, hacia abajo, hacia arriba...

En cambio, la propiedad display, nos permite crear filas con su atributo "flex" el cual creará una fila en la cual podremos ir posicionando los contenedores en el orden que queramos gracias a la anterior propiedad float.

Estas estructuras son muy útiles para crear páginas web más serias y bien estructuradas, podríamos combinarlo con enlaces que nos lleven a diferentes contenedores o páginas de nuestro sitio web.

También puede resultar de utilidad combinarlo con los recursos de Bootstrap y su gran hoja CSS con clases YA CREADAS, simplemente has de investigar un poco en su documentación que hace cada cosa y así te ahorrarás una cantidad de tiempo enorme.

Por último, si queremos que toda nuestra estructura de contenedores y filas "encaje" deberemos utilizar la propiedad "box-sizing:box". En clase no hemos recibido una mayor explicaciób de sus usos.


DISEÑO RESPONSIVE


Este diseño nos permite adaptar el formato en el que se verá nuestro sitio web según la pantalla del dispositivo (por ejemplo, si tenemos un smartphone habrá filas que quedarán muy compactas y si tenemos una televisión gigante puede que la integridad se vea afectada.)

Para evitar esto utilizaremos la propiedad "media query", la cual nos permite aplicar ciertos atributos o estilos según el tamaño de nuestra pantalla, así podremos trastear según el tipo de pantalla y adaptar nuestro html según nos sea conveniente.

Para delimitar el tamaño del dispositivo al que queremos modificar lo único que deberemos hacer es cambiar el tamaño (en pixeles o en la medida de preferencia) al lado de la propiedad media query, todo lo que se escriba a partir de ahí influirá a ese tipo de visualización en específico.




BLOQUE DE GITHUB

Github es un lugar en el cual podremos pasar nuestros archivos realizados en visual studio code. Esto es de suma importancia ya que es 
un sitio que permite que otras personas puedan ver nuestros repositorios, editarlos e, incluso, colaborar en ellos.

Nos será muy útil para subir nuestros proyectos a la nube  o compartirlos mediante un enlace al sitio web, a esto le añadimos que si 
nuestra copia en local se corrompe o daña siempre la podremos rescatar de nuestra copia sincronizada en GitHub.

Para utilizar GitHub necesitaremos crear una cuenta nueva, una vez creada veremos que tenemos diversas opciones, entre ellas, podremos 
crear directorios nuevos (pongámonos en este caso). Una vez que crees tu directorio verás que tiene una especie de enlace que nos 
servirá para clonar el archivo en local, esto se hará de la siguiente manera: 

Crearemos una carpeta que almacene los repositorios en local ( a más cerca de raíz este la carpeta, mejor), una vez creada deberemos 
acceder al "cmd" e inicializar GitHub con el comando "Git init" (todos los comandos de GitHub comienzan con "Git"). Una vez 
inicializado deberemos utilizar el comando "Git clone" (GitHub no es "key sensitive", no importará si se escriben los comandos con 
mayúsculas iniciales o  no) para así clonarlo en local.

Ahora deberemos seleccionar los cambios que queremos sobreescribir con el "Git add", como es la primera vez que usamos  este directorio 
deberemos sincronizarla todo (esto se logra con el asterisco)

Una vez hecho esto  deberemos guardar los cambios con el comando "Git commit" y, a continuación el nombre que recibirá esa 
actualización de datos, esta se hará con "-m". Ejemplo:

-Git commit -m "Actualización 1"

Este proceso nos servirá para guardar y sincronizar todos los repositorios que queramos.

Para compartir un repositorio deberemos compartir el enlace de la página del repositorio de GitHub pero, si solo queremos mostrar el 
contenido deberemos hacer uso de GitHub Pages. Esta herramienta dentro de la configuración nos permite acceder a la visualización del 
contenido de un repositorio a través de un enlace generado por la propia página. Muy útil a la hora de realizar una entrega o presentar 
algún proyecto.

En cuanto a la estructura de repositorios es importante que estos se encuentren organizados jerárquicamente y de forma ordenada y 
entendible, también deben tener nombres claros y sin espacios en blanco o mayúsculas ya que podrían generar algún error en la sintaxis 
del código.

En la creación de un archivo podremos seleccionar si este será público (todo el mundo podrá ver, modificar o interactuar con el archivo 
si tú lo deseas) o privado (tú serás el único con acceso a ese archivo). Esta decisión es importante ya que será permanente y no se 
podrá modificar más adelante. Si los usuarios tienen acceso o no a tus archivos determinará si puedes colaborar con ellos, así que 
piénsalo bien para adaptarte a tus necesidades.

Ahora hablaremos de las ramas de desarrollo. Cuanto estes editando un archivo estarás por defecto en la rama "main". Eso significa que 
tu eres el único capaz de modificar ese archivo y hacer los cambios pertinentes. Si quieres que varias personas colaboren en tu archivo 
deberás modificar la rama de desarrollo para que varias personas también puedan influir en tu trabajo. Como he dicho antes si tienes el 
archivo en privado la opción de modificar la rama estará desabilitada y solo podrás trabajar en "main".
































