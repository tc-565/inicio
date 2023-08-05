---
icon: 
  type: line-md:image
  color: 37919b 
---

# Enlaces, archivos e imágenes
Inserción de hipervínculos

## Enlaces
Para insertar un enlace se encierra entre corchetes [] el texto que 
sea desea desplegar al usuario, seguido inmediatamente con el enlace 
entre paréntesis.

~~~markdown
[Sitio web UCR](https://www.ucr.ac.cr)
~~~

[Sitio web UCR](https://www.ucr.ac.cr).

Otra manera de colocar enlaces, pero en líneas independientes es con
~~~markdown
- <https://www.ucr.ac.cr>
~~~
- <https://www.ucr.ac.cr>

## Archivos ZIP e imágenes
Usando una sintaxis similar a la de enlaces, podemos insertar imágenes y archivos ZIP. Para imágenes, se utiliza:

``![](./dirección/de/la/imagen)``

![](../note-1/note.png)

También es posible enlazar una imagen de internet:
``![](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_92x30dp.png)``

![](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_92x30dp.png)

No se debe confundir la sintaxis anterior con la de el enlace a una imagen, [enlace a una imagen](./../note-1/note.png).

Por otro lado, para archivos ZIP utilizamos:
``- [Texto que ve el usuario](dirección/del/archivo.zip)``

- [Un archivo .zip](./archivos/La_trinchera.pdf.zip)