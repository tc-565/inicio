---
icon: 
  type: simple-icons:moleculer
  color: e2ac08 
---
# Elementos de creación de cursos

Descripción de los objetos en un curso

La mayoría de objetos que vamos a describir, se nombrarán colectivamente como “tarjetas”. La metáfora de las tarjetas se utiliza en Tutors como una característica visual simple para representar una variedad de recursos de aprendizaje. En general, el contenido de una tarjeta se extrae de lo siguiente:

- Un archivo Markdown que contiene el título del recurso y un breve resumen.
- Una imagen en formato png, jpg, gif o svg.

El título, la imagen y el resumen se presentarán en la tarjeta, junto con un ícono adecuado.

Los recursos de aprendizaje generalmente se nombran para que coincidan con el contexto y se encuentren en una carpeta cuyo nombre tiene una estructura que codifica el tipo de recurso de aprendizaje.

El uso y visualización de las características descritas en este documento puede ser consultado en la [plantilla](https://github.com/tc-565/plantilla) y su [despliegue](https://tc-565.github.io/plantilla) respectivamente.

[toc]

## Nombres de recursos

Los nombres de las carpetas transmiten el tipo de recurso de aprendizaje contenido en la carpeta, y las primeras letras determinan su tipo. Las carpetas que comienzan con los siguientes nombres tienen un significado para el compilador de cursos:

|  Ejemplo                                                                                        | Fuente |
| ----------------------------------------------------------------------------------------------- | ------------------------------------------  |
| [Topic](https://tc-565.github.io/plantilla/topic-01-sin-unidades/index.html)                       | [Tópico de curso de nivel superior](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades) |
| [Unit](https://tc-565.github.io/plantilla/topic-02-con-unidades/index.html)                      | [Grupo de objetos de aprendizaje dentro de un Topic](https://github.com/tc-565/plantilla/tree/main/topic-02-con-unidades/unit-02-ordenado)|
| [archive](https://tc-565.github.io/plantilla)                               | [Archivo zip descargable](https://github.com/tc-565/plantilla/tree/main/archive-01-logo)|
| [github](https://tc-565.github.io/plantilla)                             | [Enlace a un repositorio de GitHub](https://github.com/tc-565/plantilla/tree/main/github-1-repositorio)|
| [note](https://tc-565.github.io/plantilla/topic-01-sin-unidades/note-01-nota/index.html)       | [Página simple de texto escrito en Markdown](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/note-01-nota)|
| [paneltalk](https://tc-565.github.io/plantilla/topic-04-panel-talk/index.html)            | [Presentación en PDF de nivel superior](https://github.com/tc-565/plantilla/tree/main/topic-04-panel-talk)|
| [paneltalk](https://tc-565.github.io/plantilla/paneltalk-01-presentacion/presentacion.pdf)            | [Presentación en PDF de nivel superior de pantalla completa](https://github.com/tc-565/plantilla/tree/main/paneltalk-01-presentacion)|
| [panelnote](https://tc-565.github.io/plantilla/topic-03-panel-note/index.html)            | [Notas de pantalla completa](https://github.com/tc-565/plantilla/tree/main/topic-03-panel-note/unit) |
| [talk](https://tc-565.github.io/plantilla/topic-01-sin-unidades//talk-01-presentacion/talk.pdf) | [Presentación estándar en formato PDF](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/talk-01-presentacion)|
| [web](https://github.com/tc-565/plantilla/tree/main/unit-01-unidad)                       | [Enlace a un sitio externo](https://github.com/tc-565/plantilla/tree/main/unit-01-unidad/web-1-tcu) |

 Para ordenar los objetos alfabéticamente, conviene agregar números. Para facilitar la comprensión del contexto del código fuente de otro lector, o nosotros en el futuro, es útil agregar también palabras clave al nombre de los directorios. Por ejemplo:

| Nombre de directorio   |
| ---------------------- |
| topic-01-intro         |
| topic-02-desarrollo-1  |

Para todos los nombres de archivo y directorios, evite usar espacios a la hora de nombrarlos

| Sí                     | No
| ---------------------- | -------------------- |
| topic-01-intro         | Topic 01 Intro
| topic-02-desarrollo-1  | Topic 02 Desarrollo 1

### Nombres de archivo

Normalmente, cada recurso tiene los siguientes archivos:

| Archivo                | Propósito                                                    |
| ---------------------- | ------------------------------------------------------------ |
| nombre-del-recurso.md  | Un archivo markdown que normalmente contiene un título y una breve descripción para el recurso |
| nombre-del-recurso.png | Imagen con la que se muestra el recurso. Su nombre debe coincidir con el del archivo .md. La imagen puede estar en cualquiera de los formatos .png, .jpg. .jpeg, .gif |

Los siguientes nombres de archivo están reservados:

| File name       | Description                   |
| --------------- | ----------------------------- |
| course.md       | Título del curso (obligatorio)|
| properties.yaml | Propiedades del curso (obligatorio) |
| course.png      | Imagen del curso              |
| weburl          | enlace a un sitio web externo |
| githubid        | enlace a un repositorio de GitHub |

## Estructura de un curso

Un curso es un folder con recursos de aprendizaje que se nombran con las convenciones descritas en este documento.

| Ejemplo de curso | Visualización | 
| ---------------- | ------- | 
| [Plantilla de referencia](https://github.com/tc-565/plantilla) | [Plantilla de referencia](https://tc-565.github.io/plantilla/) |

Los mínimos requisitos para un curso son que el directorio contenga los siguientes archivos:

| Nombre de archivo | Propósito |  
| -------------- | ------------ | 
| course.md      | Título del curso + información general del curso
| course.png     | Imagen del curso
| properies.yaml | Propiedades del curso

#### course.md

Es un archivo markdown estructurado de la siguiente manera:

~~~markdown
Título del curso

Información del curso - un resumen del curso, descripción o cualquier otra información relevante. Puede tener cualquier longitud.
~~~

#### properties.yaml

Metadatos del curso en formato yaml. Debe contener al menos la siguiente línea:

~~~yaml
credits: Autor del curso (o si quiere una descripción del curso)
~~~

Los créditos aparecerán como un subtítulo en la barra de título del curso.

También puede contener otras propiedades. Vea [properties.yaml](https://github.com/tc-565/plantilla/blob/main/properties.yaml) para ver algunas propiedades aplicables.

Un directorio/folder de curso normalmente contendrá Topics, el objeto descrito en la siguiente sección. Ocasionalmente también se pueden colocar unidades directamente en el directorio del curso.

### Topic

Recurso de aprendizaje de orden superior de un curso.

| Ejemplo del recurso | Visualización | 
| ---------------- | ------- | 
| [topic-01-sin-unidades](https://tc-565.github.io/plantilla/topic-01-sin-unidades/index.html) | [Topic sin unidades](https://tc-565.github.io/plantilla/topic-01-sin-unidades) |

Se requieren dos archivos:

| Archivos  | Propósito  |
| --------------- | ------------ |
| topic.md  | Título del Topic + resumen. Puede usar cualquier nombre de archivo, y tiene que tener extensión .md |
| topic.png | Imagen para el Topic. El nombre del archivo debe coincidir con el del archivo .md. El tipo de archivo puede ser .png, .jpg, o .jpeg|

#### topic.md

El título y subtítulo son extraídos del archivo .md, por ejemplo:

~~~~markdown
Título

Recursos simples de aprendizaje
~~~~

Además del título, subtítulo y el archivo de imagen mencionados anteriormente, un Topic puede contener cualquier número de unidades (ver la siguiente sección) y recursos de aprendizaje.

### Unit

Una Unit encapsula recursos de aprendizaje enmarcados con un título. Las unidades pueden estar dentro de un Topic, o colocarse directamente en el directorio base del curso.

| Ejemplo del recurso | Visualización |
| ---------------- | ------- | 
| [unit-02-ordenado](https://github.com/tc-565/plantilla/tree/main/topic-02-con-unidades/unit-02-ordenado) | [Unidad ordenada](https://tc-565.github.io/plantilla/topic-02-con-unidades) |

Se requiere un archivo .md:

| Archivos| Propósito                                                    |
| ------- | ------------------------------------------------------------ |
| unit.md | Título de la unidad. Se puede usar cualquier nombre de archivo, pero tiene que tener extensión .md |


El título es especificado en una sola linea del archivo markdown:

#### unit.md

~~~markdown
Título de la unidad
~~~

Una unidad puede contener cualquier número de recursos de aprendizaje.

## Recursos de aprendizaje

Hay dos tipos generales de recursos de aprenizaje:

- Recursos de tipo carta
- Recursos de tipo panel

Normalmente, una carta o un panel son recursos de aprendizaje que son subdirectorios dentro de un Topic o una Unit.

## Recursos tipo carta

Estos son recursos que están representados por cartas simples dentro de un Topic o una Unit:

| Ejemplo del recurso | Visualización |
| ---------------- | ------- |
| [Presentación estándar en formato PDF](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/talk-01-presentacion)             | [Presentación 1](https://tc-565.github.io/plantilla/topic-01-sin-unidades//talk-01-presentacion/talk.pdf) |
| [Página web escrita en markdown](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/note-01-nota)                | [Nota](https://tc-565.github.io/plantilla/topic-01-sin-unidades/note-01-nota/index.html)          |
| [Enlace a un sitio web](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/web-1-tcu)       | [Sitio web TC-565](https://quimica.ucr.ac.cr/2019/09/07/promocion-de-las-ciencias-educacion-costarricense/) |                                                                 
| [Archivo .zip descargable](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/archive-01-logo)                      | [Recurso 1](https://tc-565.github.io/plantilla/topic-01-sin-unidades/index.html)                              |
| [Enlace a un repositorio de GitHub](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/github-1-repositorio)                                       | [Código fuente del sitio](https://github.com/tc-565/inicio)                                             |

### Talk 

El objeto talk es una presentación en PDF, documento o cualquier otro recurso en formato PDF.

| Ejemplo del recurso | Visualización |
| ---------------- | ------- |
| [Presentación estándar en formato PDF](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/talk-01-presentacion) | [Presentación 1](https://tc-565.github.io/plantilla/topic-01-sin-unidades//talk-01-presentacion/talk.pdf) |

El archivo PDF, la descripción y título en markdown y la imagen deben tener todos el mismo nombre, que puede ser arbitrario.

| Archivos         | Propósito                                                    |
| ---------------- | ------------------------------------------------------------ |
| intro.md         | Título y breve resumen de la presentación. El archivo puede tener un nombre arbitrario, pero tiene que tener extensión .md |
| intro.png        | Imagen de la carta. El nombre del archivo debe ser el mismo que el del archivo .md. La extensión puede ser .png, .jpg, o .jpeg |
| intro.pdf        | PDF a ser renderizado si la carta es seleccionada. Su nombre debe coincidir con el del archivo .md. |

El archivo .md provee el título y subtítulo de la carta:

~~~markdown
Presentación 1

Un breve resumen de los contenidos.
~~~

### Note 

Un objeto note es una página web escrita en markdown.

| Ejemplo del recurso | Visualización |
| ---------------- | ------- |
| [Página web escrita en markdown](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/note-01-nota)                | [Nota](https://tc-565.github.io/plantilla/topic-01-sin-unidades/note-01-nota/index.html)          |

Para referencias de sintaxis de markdown, puede revisar cualquiera de los siguientes recursos:

- <https://www.markdownguide.org/basic-syntax/>
- <https://tc-565.github.io//homepage/public-site/topic-01-crear/index.html>

Es importante resaltar que en internet encontrará diversas variantes de markdown que no son compatibles entre sí, así que en caso de duda, cíñase únicamente a las guías descritas arriba.

Si desea incluir imágenes locales o enlaces a archivos, y quiere distribuirlos en la nota, inclúyalos en los directorios específicos descritos a continuación:

| Recurso    | Propósito|
| ---------- | -------- |
| note.md    | Contenido de la nota. El archivo puede tener un nombre arbitrario, pero tiene que tener extensión .md |
| intro.png  | Imagen de la carta. El nombre del archivo debe ser el mismo que el del archivo .md. La extensión puede ser .png, .jpg, o .jpeg |
| img        | Folder que contiene las imágenes referenciadas en el texto |
| archives   | Folder que contiene los archivos referenciados en el texto |

### Web 

Un enlace sencillo a un recurso web externo.

| Ejemplo del recurso | Visualización |
| ------------------- | ------------- |
| [Enlace a un sitio web](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/web-1-tcu)       | [Sitio web TC-565](https://quimica.ucr.ac.cr/2019/09/07/promocion-de-las-ciencias-educacion-costarricense/) | 

Los archivos requeridos son:

| Recurso    | Propósito|
| ---------- | -------- |
| web-link.md  | Título y breve descripción del enlace. El archivo puede tener un nombre arbitrario, pero tiene que tener extensión .md |
| web-link.png | Imagen de la carta. El nombre del archivo debe ser el mismo que el del archivo .md. La extensión puede ser .png, .jpg, o .jpeg |
| weburl | Archivo de texto sin extensión que contiene el enlace del sitio web en cuestión |

### Archive  

Un enlace a un archivo descargable (.zip).

| Ejemplo del recurso | Visualización |
| ---------------- | ------- |
| [Archivo .zip descargable](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/archive-01-logo)                      | [Recurso 1](https://tc-565.github.io/plantilla/topic-01-sin-unidades/index.html)|

Este archivo viene incluido en la fuente del curso, y es alojado junto a los recursos del sitio web.

| Recurso    | Propósito|
| ---------- | -------- |
| archvivo.md  | Título y breve descripción del archivo. El archivo puede tener un nombre arbitrario, pero tiene que tener extensión .md |
| archivo.png | Imagen de la carta. El nombre del archivo debe ser el mismo que el del archivo .md. La extensión puede ser .png, .jpg, o .jpeg |
| archivo.zip | Archivo que será descargado si la carta es seleccionada |

### Github 

Enlace a un repositorio de GitHub.

| Ejemplo del recurso | Visualización |
| ---------------- | ------- |
| [Enlace a un repositorio de GitHub](https://github.com/tc-565/plantilla/tree/main/topic-01-sin-unidades/github-1-repositorio)                                       | [Código fuente del sitio](https://github.com/tc-565/inicio)                                             |

Los archivos requeridos son:

| Recurso    | Propósito|
| ---------- | -------- |
| github.md  | Título y breve descripción del repositorio de GitHub. El archivo puede tener un nombre arbitrario, pero tiene que tener extensión .md |
| github.png | Imagen de la carta. El nombre del archivo debe ser el mismo que el del archivo .md. La extensión puede ser .png, .jpg, o .jpeg |
| githubid   | Enlace completo al repositorio en cuestión |

## Recursos tipo panel

Los paneles aparecen directamente en una unidad o tópico, y no son representados por una carta independiente. Sus contenidos son renderizados directamente en el padre, sea Topic o Unit.

| Ejemplo del recurso | Visualización |
| ---------------- | ------- | 
| [Presentación en PDF de nivel superior](https://github.com/tc-565/plantilla/tree/main/topic-04-panel-talk) | [Panel Talk](https://tc-565.github.io/plantilla/topic-04-panel-talk/index.html)|
| [Notas de pantalla completa](https://github.com/tc-565/plantilla/tree/main/topic-03-panel-note/unit) | [Panel-note (Título de la nota)](https://tc-565.github.io/plantilla/topic-03-panel-note/index.html) |

### Paneltalk 

Un documento PDF que puede ser desplegado directamente en el padre, Unidad o Topic.

| Ejemplo del recurso | Visualización |
| ---------------- | ------- | 
| [Presentación en PDF de nivel superior](https://github.com/tc-565/plantilla/tree/main/topic-04-panel-talk) | [Panel Talk](https://tc-565.github.io/plantilla/topic-04-panel-talk/index.html)| 

Se requieren dos archivos:

| Archivos         | Propósito                                                    |
| ---------------- | ------------------------------------------------------------ |
| intro.md         | Título y breve resumen de la presentación. El archivo puede tener un nombre arbitrario, pero tiene que tener extensión .md |
| intro.pdf        | PDF a ser renderizado si la carta es seleccionada. Su nombre debe coincidir con el del archivo .md. |


### Panelnote 

Un panel note es una página web completa escrita en markdown que se despliega directamente en el padre, Unidad o Topic.

| Ejemplo del recurso | Visualización |
| ---------------- | ------- | 
| [Notas de pantalla completa](https://github.com/tc-565/plantilla/tree/main/topic-03-panel-note/unit) | [Panel-note (Título de la nota)](https://tc-565.github.io/plantilla/topic-03-panel-note/index.html) | 

Para referencias de sintaxis de markdown, puede revisar cualquiera de los siguientes recursos:

- <https://www.markdownguide.org/basic-syntax/>
- <https://tc-565.github.io//homepage/public-site/topic-01-crear/index.html>

Es importante resaltar que en internet encontrará diversas variantes de markdown que no son compatibles entre sí, así que en caso de duda, cíñase únicamente a las guías descritas arriba.

Si desea incluir imágenes locales o enlaces a archivos, y quiere distribuirlos en la nota, inclúyalos en los directorios específicos descritos a continuación:

| Recurso    | Propósito|
| ---------- | -------- |
| note.md    | Contenido de la nota. El archivo puede tener un nombre arbitrario, pero tiene que tener extensión .md |
| img        | Folder que contiene las imágenes referenciadas en el texto |
| archives   | Folder que contiene los archivos referenciados en el texto |


## Ordenando recursos de aprendizaje (opcional)

Para un tópico o unidad, el orden predeterminado es el siguiente:

- talk
- lab
- note
- web
- github
- archive

Este puede ser personalizado por medio de la introducción de secciones [FrontMatter](https://docs.zettlr.com/en/core/yaml-frontmatter/) en los archivos markdown correspondientes. 

| Recurso    | Propósito|
| ---------------- | ------- | 
| [Ordenado](https://tc-565.github.io/plantilla/topic-02-con-unidades/index.html)| [Unidad ordenada](https://tc-565.github.io/plantilla/topic-02-con-unidades/index.html) | 

Esta sección debe contener un número de orden, que dicta la secuencia de las cartas.

~~~yaml
---
order: 1
---
~~~

Revise el ejemplo enlazado anteriormente para darse una mejor idea de cómo ordenar cartas. `order: 0` manda la carta al final.

## Íconos SVG (opcional)

Si no se encuentra un archivo de imagen en el recurso, el compilador de curso [tutors](https://github.com/tutors-sdk/tutors) buscará si se especificó un ícono SVG. Este ícono se consigue de la colección Iconify:

- <https://icon-sets.iconify.design/>


| Ejemplo del recurso                                          | Visualización                                                |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Plantilla](https://github.com/tc-565/plantilla) | [Iconos SVG en la plantilla](https://tc-565.github.io/plantilla/index.html) |

En Iconify hay una barra de búsqueda, donde se pueden buscar varios íconos en el formato vectorial SVG. Incluya la referencia en el archivo markdown, y agregué un color. Por ejemplo:

~~~markdown
---
icon:
  type: vscode-icons:file-type-pdf2
---
~~~

El ícono mencionado en el bloque de código anterior se obtiene del siguiente lugar:

- <https://icon-sets.iconify.design/vscode-icons/file-type-pdf2/>

Para íconos monocromáticos se puede especificar el color con su nombre en inglés:

~~~markdown
---
icon:
  type: bi:filetype-pptx
  color: green
---
~~~

## Properties.yaml

Este es un archivo en [formato YAML](https://circleci.com/blog/what-is-yaml-a-beginner-s-guide/) que contiene una colección de parámetros para todo el curso. Este define, entre otros, los siguientes aspectos:

- Descripción/crédito del curso
- Ícono del curso

### Descripción del curso, atribución del curso

Los créditos son una entrada que se presenta como subtítulo en la barra superior de la página de inicio del curso. En nuestro caso, los usaremos para dar una descripción de los contenidos del curso.

~~~yaml
credits: Breve descripción del curso
~~~

El contenido de `credits` puede ser cualquier cadena de texto. Cerciórese de poner todo el texto en una sola línea, de lo contrario el curso no podrá compilarse.

### Imagen o ícono de curso

La imagen de un curso puede ser especificada con una imagen en el directorio del curso:

- course.png

Alternativamente, se puede especificar un ícono SVG. Seleccione un ícono de Iconify:

- <https://icon-sets.iconify.design/>

Especifique el ícono en `properties.yaml` de la siguiente manera:

~~~yaml
icon :
  type: fa-solid:code-branch
  color: FFD601
~~~

El ícono anterior se obtiene del siguiente lugar:

- <https://icon-sets.iconify.design/fa-solid/code-branch/>

## Redimensionamiento de imágenes

Puede que algunas imágenes sean de muy alta resolución, por lo que aparecerían muy grandes en el sitio web. Esto puede suceder a menudo con capturas de pantalla. Puede utilizar el siguiente servicio para solventar el problema y redimensionar las imágenes a un tamaño adecuado:

- <https://nodeca.github.io/pica/demo>

## Plantilla y curso de referencia

El curso y plantilla de referencia puede ser consultado en:

- <https://github.com/tc-565/plantilla>

Y está publicado en:

- <https://tc-565.github.io/plantilla>

Este curso ilustra la mayoría de las funcionalidades descritas en este documento, y puede ser descargado en:

- <https://github.com/tc-565/plantilla/archive/refs/heads/main.zip>
