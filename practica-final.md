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
- Me descargo bootstrap.bundle.min.js para mantener el diseño original del archivo index.html
- Uso la fórmula pandoc </nombre del archivo/>.md -o </nombre del archivo>.html para convertir los archivos .md en .html
- Uso el comando cat <nombre del archivo>.html <nombre del archivo 2>.html...  > metodologia.html para unir todos los archivos html
- Modifico con nano los enlaces a las imagenenes para que se muestren correctamente en el archivo. 
- Este código lo copio y lo pego con nano en el cuerpo de index.html. El cuerpo comineza después de la marca <!--Begin page content--> y el código de las prácticas las he copiado después de \<div class\=\"container\"\>  
- Para ordenar mi repositorio he creado una carpeta con mkdir llamada html/ y con el comando mv he movido los archivos *.html
