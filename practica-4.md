# OpenRefine
- Subir datos a OpenRefine
- En OpenRefine usar value.Replace ("","") para borrar elementos innecesarios que aparecía con los datos. 
- Usar facet para seleccionar las filas que no me servían y luego borrarlas con "remove matching rows"
- Poner que los datos de números eran de números, los de texto de texto...
- Uso del undo para recuperar los datos borrados para una gráfica
- En el caso de los accidentes con víctimas y sin víctimas, uso del recuento de datos de texto creando una columna con value = value.strip().lower()
if "con víctimas" in value: return "Accidente con víctimas" y 
- fUNCIÓN SORT PARA VER QUÉ distritos  habían necesitado más actuaciones policiales 
