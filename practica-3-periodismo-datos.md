# Práctica 3 de periodismo de datos
## Imágenes
## Explicación del proceso: terminal y Openrefine
- Para el siguiente proyecto ha sido necesario el uso de la terminal a la hora de descargar los archivos que, posteriormente, se filtrarían con el programa Openrefine. El archivo feliz.csv fue descargado a través del comando "git clone". Este comando permite que las carpetas y archivos presentes en un repositorio de Github se descarguen en el ordenador, por lo que posibilita que se pueda trabajar desde la terminal con ellos.
- Tras esto, subí el archivo a Openrefine, donde pude filtrar los datos que quería estudiar. En primer lugar, indiqué el tipo de datos con los que contabacada columna: texto, fecha, número...etc. De esta forma, Openrefine me permitía hacer uso de su sistema de visualización de datos, lo que me facilitó su selección y la eliminación de aquellos que no me eran útiles.
- A través de la función facet he podido borrar todos los datos que eran claramente erróneos. Por ejemplo: aquellos tweets que aparecían con fecha de 1970. Lo que he hecho ha sido marcar ese periodo de tiempo y eliminar todas las celdas que se correspondiesen a esa selección. Por otra parte, hay datos como los de Felipe González y Felipe VI que podría haber eliminado a través de la función facet para texto (seleccionando la categoría "Felipe VI" y eliminando todos los datos que se correspondieran con ella). Sin embargo, he optado por dejarlos ya que la finalidad de mi proyecto no se centra en la palabra "feliz" en sí misma, sino en qué tweets iniciados por "feli" fueron más vistos en el periodo de más actividad de publicaciones (junio-julio) y me resultó interesante que algunos de los más visitados estuvieran relacionadas con política y no con palabras relativas a la felicidad.
- El gráfico que he realizado trabaja con tres variables: fecha, nombre del tweet y número. El objetivo es ver qué tipo de tweets tuvieron más éxito durante la época con más actividad en la red social. Para ello he utilizadola función facet, con la que he realizado un gráfico temporal donde he señalado la época desde 2020-06-03 hasta 2020-07-30.
- Por otra parte, los datos de texto han sido filtrados a través de la función "cluster" que me permitió fusionar todos los datos que contaban con la misma información pero escrita de forma distinta. Por ejemplo: los datos como "Feliz Jueves" han sido fusionado con otros como "FelizJueves". Esto hace que las decenas de categorías textuales que propone la función "facet" se queden en 15, una cantidad mucho más manejable.
- Por último, he usado la función "facet" con la columna "número" y he marcado que se muestren únicamente los datos que cuentan con una información númérica y que no se mostraran las casillas en blanco.
- Para eliminar los Hashtags en los datos de texto y las Zs en los de fecha he utilizado la función "transform" con la fórmula "value.replace("Z","")".

## Proceso en Datawrapper
- En Datawrapper he insertado el archivo csv y posteriormente he marcado qué tipo de datos se correspondía con cada columna: fecha, texto, número.
- Posteriormente, he trabajado en la visualización, para ello he tomado las siguientes decisiones:
	- He elegido un gráfico de dispersión para mostrar mis datos.
	- He escogido colores y formas difetentes para los datos que correspondían a un mismo tweet.
	- He añadido una línea que indica el cremimiento o decrecimiento de los datos agrupados.
	- He situado los datos de fecha en el eje X y los numéricos en el eje Y.
	- He insertado etiquetas a los datos para que al pinchar encima se pueda leer a qué categoría pertenece cada dato.
	- He añadido una descripción y una fuente

## Explicación del gráfico
- 
