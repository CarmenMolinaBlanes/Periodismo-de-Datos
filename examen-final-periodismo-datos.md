# Examen Final periodismo de datos
## Preguntas obligatorias

* ¿Quién es Philip Meyer?

Philip Meyer ha sido uno de los primeros desarrolladores del que hoy conocemos como "periodismo de datos". Sin embargo, él lo llamaría "periodismo de precisión". Destaca por el uso de la asistencia de computadoras durante los disturbios de Detroit en 1967. 

* ¿Quién es Florence Nightgale?

Fue una enfermera y estatista de Gran Bretaña. A través de la estadística realizó una representación visual de las causas de mortalidad de los soldados en el hospital militar que dirigía. Fue una pionera en la representación gráfica de datos estadísticos.

## Preguntas opcionales

* Expón dos mejoras que has tenido en tu proceso de trabajocon el ordenador.

Una de las mejoras más notables que he tenido en mi proceso de trabajo con el ordenador ha sido la posibilidad de trabajar desde el ámbito local de mi ordenador sin depender de internet. Por lo tanto, no me veo obligada a utilizar herramientas de terceros (como Microsoft Office) para realizar mis proyectos, ni dependo de la conexión a internet. Al poder trabajar desde la terminal puedo generar mis propios archivos de texto y subirlos a plataformas como github con total seguridad. Por otra parte, dentro del ámbito de la Web he descubierto el significado de https, por lo tanto, al ser consciente de que la S indica "Seguro" trato de evitar entrar en páginas web con dominios que carecen de una S en su protocolo.

* ¿Qué es nano?

Nano es un editor de texto para la terminal.

* ¿Qué tipos de interfaces hay?

Encontramos dos tipos de interfaces CLI y GUI. Mientras que GUI es una interfaz gráfica (a la que el usuario habitual de tecnologías informáticas está acostumbrado), CLI es una interfaz de línea de comandos. 

* ¿Qué saberes están implicados en el periodismo de datos?

Por un lado el periodismo. Esta aseveración parece evidente, pero, ¿qué es realmente el periodismo? El periodismo busca reflejar y transmitir realidades (en muchas ocasiones complejas) a los ciudadanos. Por lo tanto, el periodismo va unido a la expresión, comunicación y sobre todo a la investigación.

Por otro lado tenemos los datos. Estos datos en la actualidad se tratan de registros electrónicos con los que se trabajan, en muchas ocasiones, con programas informáticos como OpenRefine. Los datos no tienen por qué estar estructurados, de hecho, en muchas ocasiones la labor del periodista es la de estructurar grandes cantidades de datos

Por último tenemos la visualización. Esta es funcional para diversas partes del periodismo de datos. En primer lugar, puede ser útil para el análisis de datos (ya que al poder visualizarlos en forma de gráfico o faceta puede agilizar el trabajo del periodista) y por otra parte es esencial para la comprensión de los datos por parte de la población general.

* ¿Qué medio de comunicación en inglés es fundamental para el periodismo de datos?
The Guardian. Su implicación con el periodismo de datos puede observarse en la creación en 2009 de una sección llamada DataBlog, dedicada únicamente al desarrollo de esta disciplina periodística.

* ¿Qué tipos de datos hay?
Numéricos (dentro de los numéricos podemos encontrar los integer, decimal, double, date, period), String (que son conjuntos de caractéres) y booleanos (que dan una opción binaria, por ejemplo "verdadero o falso")

* Elige una URL de una noticia de un medio de comunicación y explícala tal y como lo hicimos en clase

https://www.theguardian.com/commentisfree/2022/jan/19/dumped-fishing-gear-killing-marine-life-governments-care-scottish-trawlerman-nets

En esta URL podemos ver, en primer lugar, el protocolo con el que funciona (hhttps). Siendo http el protocolo en sí y S indicando que es una página segura. Por otra parte, el dominio debe leerse según la importancia de sus elementos (de derecha a izquierda) por lo tanto, lo más importante es .com que es un TLD (Dominio de Primer Nivel) y que ha alquilado el dominio www.theguardia.com al medio inglés. Por otra parte, el lado derecho del cominio (separado con el carácter /) indica la estructura de carpetas web de la página, llegando finalmente al archivo deseado.

* Si quiseiras ver la web theguardian.com, ¿cómo lo harías desde la línea de comandos?

lynx www.theguardian.com 

En esta estructura de comando encontramos el comando en sí y un argumento.

* ¿Cómo te descargarías la web theguardian.com desde la línea de comandos?

Con lynx -source www.theguardian.com

* Cuál es el primer comando que deberías usar en la terminal. Explica tu respuesta

pwd, ya que te indica en qué directorio te encuentras y sobre qué estás trabajando. Por otra parte, sería interesante usar whoami para conocer el nombre de tu localhost.


* ¿Qué 3 tipos de formatos de datos hemos visto? ¿Qué similitudes y diferencias tienen?

Hemos visto XML, JSON y *SV. Las diferencias son:

- En el caso de XML su complejidad le diferencia

- JSON utiliza la sintaxis JS, funcionan de forma óptima con aplicaciones wec y permiten más complejidad que los *SV

- Los SV indican que los valores están separados de alguna forma (TSV por tabuladores y CSV por comas). Son los más sencillos u menos estandarizados.

* ¿Que tipo de dato de fecha elegirías para tus archivos? Razona tu respuesta.

Eligiría date en caso de que la fecha sea fija y no tenga que trabajar con ella más que para delimitar temporalmente el resto de datos (por ejemplo, a través de la herramienta facet en OpenRefine) o para establecer con total seguridad la fecha de un dato. Por el contrario usaría el tipo de dato period si no estuviera segura de la fecha de mis datos o el periodo de tiempo de los mismos fuera variable en el momento en el que trabajo con ellos, ya que la función period te da la opción de establecer periodos de tiempo aproximados (P -5D, por ejemplo).

* Pon un ejemplo de "wildcards"

Los wildcards son comodines o atajos en los lenguajes informáticos. Un ejemplo de wildcard sería el uso de * (asterísco) para que la terminal lea que todos los archivos que cuenten con los caracteres que van tras este asterisco están incluídos en la acción que quiero realizar. Por ejemplo, si quiero copiar todos mis archivos .CSV a una carperta haría: cp *.CSV CSV/


* ¿Qué función tiene la almohadilla en Markdown y en un programa de la shell? Razona tu respuesta.

En Markdown es el equivalente a h1 en HTML lo que indica que es un encabezamiento de primer nivel. Mientras que el la terminar la almoadilla indica que la línea escrita tras esta es un comentario del usuario y que el programa no debe leerla.

* Cómo realizas algún cambio en tu repositorio local y lo actualizas también en Github. Explica los pasos.

- Para realizar un cambio en mi repositorio local en primer lugar debo hacer uso de la terminal. Según el cambio que quiera realizar usaré unos comandos u otros (si quisiera copiar un archivo en el repositorio local usaría cp por ejemplo). 
- Para actualizarlo en github debo, en primer lugar, asegurarme de que mi repositorio local está actualizado (usando el comando git pull).
- Cuando esté actualizado utilizamos el comando git add . (el punto indica que queremos reflejar todos los cambios realizados en el repositorio local).
- Posteriormente usamos el comando git commit -m acompañado de un comentario que se añadirá a tu repositorio en Github
- Finalmente se utiliza el comando git push origin main.

* Explica los pasos para clonar en tu ordenador un repositorio de Github.

Para clonar un repositorio de github en un ordenador se utiliza el comando git clone. Esto es necesario para poder actualizar tu repositorio desde el ámbito local de tu dispositivo. El comando se estructura de la siguiente manera: git clone (el comando) http://github.com/mi-repositorio (el argumento).

* Explica al menos un error/dificultad que hayas tenido y cómo lo has abordado y, si así ha sido, resuelto.

Uno de los errores más habituales que he tenido ha sido el de intentar actualizar mi repositorio sin antes actualizar mi repositorio local con git pull. Esto al principio me generaba una situación de incomprensión ya que me preguntaba una y otra vez por qué no me funcionaba git push si no había cometigo ningún error en la redacción del comando. Pero al final acabé automatizando el proceso de realizar un git pull por si acaso antes de actualizar la terminal en Github.

* Describe los datos que estamos utilizando en el proyecto TRESCA. Qué tipo de archivo y qué tipo de datos.

TRESCA contaba con los datos de feliz.csv que, por lo que recuerdo, contaba con datos de date, number integer y string. Por otra parte era un archivo csv, lo que significa comma separated values. 

* ¿Cómo harías que OpenRefine interpretara correctamente los tipos de datos?
Se accede a la herramienta cells (desde la parte superior de la columna). Posteriormente entramos en common conversions y finalmente estableces el tipo de datos con el que estás trabajando (to date, to number o to text).

* Qué es una Faceta de texto

Facet es una herramienta presente en el programa OpenRefine (que originalmente se llamaba Google Refine) que permite la visualización de los datos para su análisis, agilizando así la labor del informático o periodista. En concreto, la facet de texto muestra qué palabras (o strings) aparecen dentro de una columna de datos y marca las veces que se repite. Esto te permite conocer: cuál es la palabra que más se repite y la que menos y seleccionar la palabra que quieras analizar o comparar con otros tipos de datos.

* Qué es una faceta temporal

El término faceta fue desarrollado en la pregunta anterior. Por lo que desarrollaré la utilidad de la faceta temporal en concreto en este apartado. La faceta temporal sirve para enmarcar temporalmente los datos de un proyecto. Esta te muestra una gráfica donde puedes ver: en qué fechas hay una mayor cantidad de datos y en qué periodo de tiempo estamos trabajando (periodo que podemos limitar para trabajar únicamente con los datos de un conjunto de meses, días o años).

* Para qué usas cd y cómo

El comando cd en la terminal sirve para entrar en un directorio. Es un comando que debe escribirse con una estructura compuesta donde encontramos el nombre del comando en sí y un argumento donde escribamos el nombre del directorio, por ejemplo: cd mi-repositorio/

* Para qué usas cp y cómo.

cp sirve para copiar un archivo dentro de un directorio elegido por el usuario. Al igual que cd es un comando que requiere de una estructura compuesta donde encontramos el nombre del comando en sí y un argumento donde escribimos el nombre del archivo que queremos copiar y el nombre de la carpeta donde queremos que se copie. Por ejemplo: cp examen-final-periodismo-datos.md mi-repositorio/

* Para qué usas mv

mv sirve para mover un archivo de un directorio o otro. Para usar mv debes nombrar el archivo y el lugar al que quieres moverlo, por ejemplo: mv examen-final-periodismo-datos.md mi-repositorio/. mv también sirve para cambiar el nombre de un archivo, por ejemplo: mv examen-final-periodismo-datos.md examen-final.md.

* Para qué usas mkdir y cómo

mkdir sirve para crear nuevos directorios. Para utilizarlo debes situarte en el directorio donde desees crear nuevas carpetas con el comando cd. Posteriormente escribes el comando mkdir y lo acompañas de los nombres que quieres que tengan tus nuevos directorios. Por ejemplo: mkdir csv

* ¿Por qué es importante la visualización en el análisis de datos?

Porque agiliza el tratamiento de los datos. En OpenRefine vemos un claro ejemplo de la utilidad de visualizar los datos durante su análisis. Como he explicado anteriormente en las preguntas sobre las facetas, estas permiten analizar en cuestión de segundos qué datos se repiten más en una fecha (por ejemplo) para seleccionarlos. Este trabajo, con un gran volumen de datos y sin una herramienta de visualización, tomaría horas para el periodista.

* ¿Qué lenguajes informáticos conoces?

Podemos dividir los lenguajes informáticos en dos categorías. Por un lado tenemos los lenguajes de estructuracíón, entre los que encontramos HTML. Estos lenguajes sirven para organizar visualmente la información. Por otro lado tenemos los lenguajes de programación, entre los que encontramos Java, C, C ++...etc.

* ¿Cuál es la diferencia entre Internet y la Web?
Internet es una Red de Redes que conecta a los servidores con los localhosts y que utiliza los protocolos TCP/IP. TCP es el protocolo que divide los bits en paquetes e IP es el número de identificación que representa un nodo en internet. Sin embargo, la Web es la Red dentro de internet que utiliza como protocolo de aplicación HTTP. Sin embargo, dentro de internet encontramos otras redes con otros protocolos de aplicación, como IMAP para el correo electrónico. 

* ¿Qué ha sido determinante para el nacimiento del periodismo de datos moderno?

HTML5, el software de código abierto y el Open Data.

* ¿Qué es Markdown?

Markdown es una sintaxis muy simple que al mismo tiempo es conversor en HTML. Su simplicidad limita a la sintaxis de Markdown, por lo que no se puede realizar cualquier protecto a través de esta.

* Apunta tres comandos que hayas utilizado y para qué.
Tres comandos que he utilizado han sido cd para entrar en un directorio, cd para copiar y pegar un archivo de un directorio en otro y mkdir para crear nuevos directorios. 

* ¿Que significa TSV?

TSV significa Tabular Separeted Values. Es un formato *SV que, como he explicado con anterioridad, es destacable por su simplicidad. El TSV es el precedesor del CSV "Comma Separated Values". 

* Expón dos procedimientos (comandos, funciones, herramientas, procesos) que hayas usado o que te hayan llamado la atención y coméntalos.

Una herramienta que me ha sorprendido se encuentra en OpenRefine y se trata de la herramienta cluster. Esta permite (mediante procesos lingüísticos de gran importancia para la informática) combinar aquellos datos string que sean similares por diversas razones. Por otra parte, he quedado muy sorprendida por los comandos de git: git add . git commit -m y git push. Antes de cursar Periodismo de datos no sabía que podía trasladar los archivos presentes en mi localhost a internet desde la terminal.

* ¿Qué hay que hacer para ver el valor de la variable de entorno de shell "PATH" con el comando "echo"?

echo $PATH
