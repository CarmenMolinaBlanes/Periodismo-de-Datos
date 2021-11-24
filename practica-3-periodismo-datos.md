# Práctica 3 de periodismo de datos
## Imágenes
## Explicación del proceso: terminal y Openrefine
- Para el siguiente proyecto ha sido necesario el uso de la terminal a la hora de descargar los archivos que, posteriormente, se filtrarían con el programa Openrefine. El archivo feliz.csv fue descargado a través del comando "git clone". Este comando permite que las carpetas y archivos presentes en un repositorio de Github se descarguen en el ordenador, por lo que posibilita que se puedan trabajar desde la terminal con ellos.
- Tras esto, subí el archivo a Openrefine, donde pude filtrar los datos que quería estudiar. En primer lugar, indiqué el tipo de datos con los que contabacada columna: texto, fecha, número...etc. De esta forma, Openrefine me permitía hacer uso de su sistema de visualización de datos, lo que me facilitó su selección y la eliminación de aquellos que no me eran útiles.
- El primer gráfico que he realizado trabaja con tres variables: fecha, nombre del tweet y número. El objetivo es ver qué tipo de tweets tuvieron más éxito durante la época con más actividad en la red social. Para ello he utilizadola función facet, con la que he realizado un gráfico temporal donde he señalado la época desde 2020-06-03 hasta 2020-07-30.
- Por otra parte, los datos de texto han sido filtrados a través de la función "cluster" que me permitió fusionar todos los datos que contaban con la misma información, pero escrita de forma distinta. Por ejemplo: los datos como "Feliz Jueves" han sido fusionado con otros como "FelizJueves". Esto hace que las decenas de categorías textuales que propone la función "facet" se queden en 15, una cantidad mucho más manejable.
- Por último, he usado la función "facet" con la columna "número" y he marcado que se muestren únicamente los datos que cuentan con una información númérica y que no se mostraran las casillas en blanco.
- Para eliminar los Hashtags 
## Análisis de los gráficos
