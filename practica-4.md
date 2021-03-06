# La policía actúa en Madrid
## Análisis del proceso
### OpenRefine

Para procesar los datos utilizados (extraídos en formato csv de la página datos.madrid.es) he utilizado únicamente la herramienta OpenRefine. En primer lugar, he eliminado aquellas columnas que no resultaban útiles para el análisis de datos que quería realizar. Después, he utilizado la fórmula value.replace("","") para borrar elementos innecesarios que aparecían con los datos (como algunos guiones sin sentido). Otro paso básico que he realizado ha sido marcar el tipo de datos con el que estoy trabajando (texto y número) lo que me ha permitido usar la función facet.

Después de esto he usado la función facet (text) para seleccionar las filas que no me servían para cada proyecto (también he utilizado la función star con esta finalidad). Posteriormente las he borrado con la función "remove matching rows". Por ejemplo, para muchas gráficas no necesitaba el total de actuaciones policiales, por lo que, a través de facet, he buscado el nombre "TOTAL DE ACTUACIONES", lo he señalado y posteriormente lo he eliminado. Sin embargo, en aquellos casos en los que he tenido que eliminar más de una fila, ha sido más práctico marcar las filas inservibles con star y después eliminarlas.

![Esta imagen muestra cómo se marca star en OpenRefine](/img/OpenRefine-star.PNG)

![Esta imagen muestra la función de remove matching row](/img/OpenRefine-remove-matching.PNG)  

Para relizar algunas de las gráficas, me he visto obligada a eliminar algunas celdas que, para posteriores gráficas, me eran útiles. Por lo tanto, he hecho uso de la función "undo" para recuperar los datos borrados.


En el caso del análisis de los accidentes con víctimas y sin víctimas he hecho uso del recuento de datos de texto creando una columna con:
- value = value.strip().lower()
if "con víctimas" in value: return "Accidente con víctimas" 
- row.record.cells["Accidente con víctimas].value.sum() 

Una función que he utilizado con bastante asiduidad ha sido "sort". a través de esta función he podido hallar, por ejemplo, cuáles son las cuatro zonas de Madrid con más actuaciones policiales en términos de conflictos entre personas (por ejemplo). 

Otra forma en la que he utilizado la función facet ha sido para seleccionar rangos numéricos. Por ejemplo, en la gráfica donde muestro de forma comparativa los distritos con más de 200 casos de actuaciones policiales por consumo de alcohol en la vía pública por parte de adultos y con menos de 1000.

![Esta imagen muestra el uso de facet en OpenRefine](/img/OpenRefine-facet.PNG)

### Datawrapper

En Datawrapper he realizado un total de 6 gráficos. Para ello, he tenido que seleccionar dentro de la propia aplicación cuáles de las columnas me eran útiles y cuales no. Por otra parte, he seleccionado qué tipo de dato se correspondía con cada columna (texto y número).

Por otra parte, he usado diversos tipos de gráfico, ya que Datawrapper da una amplia posibilidad de elección dentro de su aplicación. Entre ellos he utilizado: mapas, gráficos de dispersión, gráficos de barras, un pie chart...etc. La selección está ligada al tipo de datos que quiero visualizar:
- En caso de querer mostrar una gran cantidad de datos textuales (con finalidad comparativa) y dos tipos de datos numéricos he usado un gráfico de dispersión;
- mientras que he usado el modelo del mapa para visualizar de forma espacial algún dato numérico concreto (por ejemplo, las actuaciones policiales por tenencia de drogas). 
- Sin embargo, para no generar una sensación de monotonía en el artículo, solo he elaborado un mapa, por lo que he utilizado también gráficos de barras para reflejar comparativamente algún dato numérico concreto por distritos.
- Por otra parte, para comparar dos o varios distritos diferentes he utilizado tanto el pie chart y la columna apilada. 

A la hora de elaborar las visualizaciones, he utilizado principalmente el cambio de colores, las etiquetas...etc.

Por último, he hecho uso de la función de "insertar título" e "insertar descripción" para que los gráficos puedan comprenderse mejor.


### Análisis

![actuaciones policiales por tenencia de armas por distritos](/img/actuaciones-policiales-por-tenencia-de-armas-octubre-2021-madrid-.png)

En esta imagen he analizado los datos de tenencia de armas por distritos de Madrid. El uso de un gráfico de columnas permite que se visualice fácilmente cuáles son las zonas donde se ha cometido este delito con más frecuencia. 

Al ser la posesión de armas una fuente de peligro, he dividido los colores según el nivel de peligrosidad de la zona. El rojo, el naranja, el amarillo y el verde son los colores que he utilizado para representar el concepto de la peligrosidad. Esto se debe a que, naturalmente, identificamos el rojo, el amarillo y el verde con grados de peligro. Esto se utiliza tanto en gráficos de meteorología como en los propios semáforos.

En este gráfico, podemos observar que en Octubre de 2021 las zonas con más actuaciones policiales por tenencia de armas fueron Puente de Vallecas y Centro.

![mapa de actuaciones policiales por tenencia de drogas por distritos de Madrid](/img/tenencia-de-drogas-en-madrid-por-distritos.png)

En este mapa podemos ver, con tonalidades de azul, las zonas donde ha habido más actuaciones policiales por tenencia de drogas (en azul más oscuro) y las  zonas en las que ha habido menos (azul más claro, llegando incluso a parecer color pistacho). 

He etiquetado únicamente las zonas más grandes del mapa para que el lector habitante de Madrid pueda ubicarse en el mapa. 

![gráfico de dispersión que compara las actuaciones por tenencia de drogas y por consumo](/img/relaci-n-entre-las-detenciones-por-consumo-y-tenencia-de-drogas.png)

En este gráfico de dispersión he utilizado diversos elementos a analizar:
- El primero es el uso de una línea de frecuencia, que evidencia que la relación entre las actuaciones policiales por tenencia de drogas no son directamente proporcionales a las de consumo de las mismas. Esto se debe a que hay una gran cantidad de zonas (ćomo Villa de Vallecas, Arganzuela o Chamberí) donde la presencia de delitos por tenencia de drogas es muy baja, mientras que los delitos por consumo de las mismas son llamativamente altos. Es por ello que la línea no es continua, sino que genera una forma convexa.
- Por otra parte, es destacable el cambio de colores en los datos de la gráfica. Este trata de mostrar con más intensidad aquellos datos con mayor incidencia de ambas variables (o aquellos que tienen una incidencia muy notable de una sola, como Villa de Vallecas, Arganzuela o Chamberí). Además, estos datos son los únicos que vienen acompañados de un nombre, lo que ayuda a que resalten aún más.

![actuaciones policiales en los cuatro distritos con más incidentes](/img/actuaciones-policiales-en-los-cuatro-distritos-con-m-s-incidentes-octubre-2021-madrid.png)

En este gráfico podemos observar de forma diferenciada el volumen de actuaciones policiales en los cuatro distritos de Madrid con más incidencia y la causa de las mismas. Para ello, he marcado cada distrito con un color diferente (todos tonalidades del azul) mostrando la tonalidad más oscura aquel distrioto con mayor incidencia de delitos (el centro, que aparece en azul oscuro), mientras que la tonalidad más clara muestra el distrito con menor incidencia (San Blas). 

Por otra parte, he marcado que se muestren los datos exactos de cada variable. Ya que, de lo contrario, es posible visualizar un volumen aproximado, pero no la exactitud que corresponde a cada distrito. 


![consumo de alcohol en la vía pública por distritos](/img/consumo-de-alcohol-en-la-v-a-p-blica-por-distritos.png)

En este gráfico muestro las zonas con casos consumo de alcohol en la vía pública que oscilan entre los 200 y los 1000. Estos datos están divididos por distritos y muestran la cifra exacta de infricciones por zona. El uso de este tipo de gráfico se debe a la cantidad de distritos analizados, que se pueden visualizar de forma rápida en forma de circunfefrencia. Por otra parte, vuelvo a utiliar tonalidades de azul para distinguir las distintas zonas y evitar la monocromía. Auqnue estos colores son medianamente azarosos ya que hay algunos en celeste con cifras de hasta 792 delitos y otros en azul oscuro con solo 256.


![actuaciones policiales por accidentes de tráfico](/img/actuaciones-policiales-por-accidentes-de-coche-octubre-2021-madrid-.png)

