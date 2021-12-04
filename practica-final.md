# Subida a Pandoc
## Proceso de descarga y creación de archivos .html
- Descarga de Pandoc y creación de la carpeta css/ desde la terminal (creé la carpeta con mkdir). 
- Extraigo archivo de estilo y lo añado a index.html. Este archivo se llama bootstrap.min.css y el proceso se realizó desde nano.
- He creado con mkdir un archivo llamado docs/ donde he movido (con mv) index.html y sticky-footer-navbar.css.
- Tras esto, he creado un archivo .md fuera de mi repositorio al que he llamado pandoctest.md. Este tenía la finalidad de testear la aplicación Pandoc y su utilidad para transformar md en html. 
![testeo de pandoctest.md](/img/terminal-prueba-pacdoc.PNG)
- Después he entrado en mi-repositorio y dentro de esta carpeta he convertido (con Pandoc) mis trabajos en .md en archivos .index.html. Esto lo he realizado desde la función "pandoc practica-3.md -o practica-3.index.html".
![conversión oficial](/img/terminal-oficial-pandoc.PNG) 
## Edición de index.html
- En primer lugar he modificado el título a través de nano. He cambiado el título inicial por \<title\>Mis trabajos de Github\<\/title\>
