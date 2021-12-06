# Subida a Pandoc
## Proceso de descarga y creación de archivos .html
- He descargado pandoc a través de apt-cyg install (en cygwin, aunque use de forma habitual git bash). He descomprimido la carpeta sticky-footer-navbar/ y he creado dentro de ella una carpeta llamada css/ desde la terminal (creé la carpeta con mkdir). 
- Después extraí el archivo de estilo y lo añadí a index.html. Este archivo se llama bootstrap.min.css y el proceso se realizó desde nano.
- He creado con mkdir un archivo llamado docs/ donde he movido (con el comando mv) index.html y sticky-footer-navbar.css.

- Tras esto, he creado un archivo .md fuera de mi repositorio al que he llamado pandoctest.md. Este tenía la finalidad de testear la aplicación Pandoc y su utilidad para transformar md en html. 
![testeo de pandoctest.md](/img/terminal-prueba-pacdoc.PNG)
- Después he entrado en mi-repositorio desde la terminal y dentro de esta carpeta he convertido (con Pandoc) mis trabajos .md en archivos .html. Esto lo he realizado desde la función "pandoc practica-3.md -o practica-3.index.html".Otra forma de convertir archivos .md en .html es "pandoc -f practica-3.md -t practica-3.html". 

![conversión oficial](/img/terminal-oficial-pandoc.PNG) 
## Edición de index.html
- En primer lugar he modificado el título a través de nano. He cambiado el título inicial por \<title\>Mis trabajos de Github\<\/title\>
- Después me he descargado bootstrap.bundle.min.js para mantener el diseño original del archivo index.html
- Usé el comando cat <nombre del archivo>.html <nombre del archivo 2>.html...  > everything.html para unir todos los archivos html en uno solo que simplificara y compilara los trabajos para facilitar su copiado y pegado.
- Tras esto he modificado con nano los enlaces a las imagenenes para que se muestren correctamente en el archivo. Para ello además ha sido necesario insertar la carpeta img/ dentro de la carpeta docs/. 
- El código html presente en el archivo everything.html lo copio y lo pego con nano en el cuerpo de index.html. El cuerpo comineza después de la marca <!--Begin page content--> y el código de las prácticas lo he copiado después de \<div class\=\"container\"\>  
- Para ordenar mi repositorio he creado una carpeta con mkdir llamada html/ y con el comando mv he movido los archivos *.html. Posteriormente y a petición del profesor, he usado el comando mv para mover la carpeta html/ dentro de la carpeta docs/. Por último, he cambiado los nombres de los archivos .html que aparecían como .index.html con el comando mv.
