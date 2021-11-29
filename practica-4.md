# La policía actúa en Madrid
## Análisis del proceso
### OpenRefine

Para procesar los datos utilizados (extraídos en formato csv de la página datos.madrid.es) he utilizado únicamente la herramienta OpenRefine. En primer lugar, he eliminado aquellas columnas que no resultaban útiles para el análisis de datos que quería realizar. Después, he utilizado la fórmula value.replace("","") para borrar elementos innecesarios que aparecían con los datos (como algunos guiones sin sentido). Otro paso básico que he realizado ha sido marcar el tipo de datos con el que estoy trabajando (texto y número) lo que me ha permitido usar la función facet.

Después de esto he usado la función facet (text) para seleccionar las filas que no me servían para cada proyecto (también he utilizado la función star con esta finalidad). Posteriormente las he borrado con la función "remove matching rows". Por ejemplo, para muchas gráficas no necesitaba el total de actuaciones policiales, por lo que, a través de facet, he buscado el nombre "TOTAL DE ACTUACIONES", lo he señalado y posteriormente lo he eliminado. Sin embargo, en aquellos casos en los que he tenido que eliminar más de una fila, ha sido más práctico marcar las filas inservibles con star y después eliminarlas.

![Esta imagen muestra cómo se marca star en OpenRefine](/img/OpenRefine-star.PNG)

![Esta imagen muestra la función de remove matching row](/img/OpenRefineremove-catching.PNG)  

Para relizar algunas de las gráficas, me he visto obligada a eliminar algunas celdas que, para posteriores gráficas, me eran útiles. Por lo tanto, he hecho uso de la función "undo" para recuperar los datos borrados.


En el caso del análisis de los accidentes con víctimas y sin víctimas he hecho uso del recuento de datos de texto creando una columna con:
- value = value.strip().lower()
if "con víctimas" in value: return "Accidente con víctimas" 
- 

Una función que he utilizado con bastante asiduidad ha sido "sort". a través de esta función he podido hallar, por ejemplo, cuáles son las cuatro zonas de Madrid con más actuaciones policiales en términos de conflictos entre personas (por ejemplo). 

Otra forma en la que he utilizado la función facet ha sido para seleccionar rangos numéricos. Por ejemplo, en la gráfica donde muestro de forma comparativa los distritos con más de 200 casos de actuaciones policiales por consumo de alcohol en la vía pública por parte de adultos y con menos de 1000.

![Esta imagen muestra el uso de facet en OpenRefine](/img/OpenRefine-facet.PNG)

### Datawrapper

En Datawrapper he realizado un total de 6 gráficos. Para ello, he tenido que seleccionar dentro de la propia aplicación cuáles de las columnas me eran útiles y cuales no. Por otra parte, he seleccionado qué tipo de dato se correspondía con cada columna (texto y número).

Por otra parte, 
