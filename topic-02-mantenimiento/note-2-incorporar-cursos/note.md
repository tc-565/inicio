---
icon: 
  type: gridicons:add
  color: e2ac08 
---
# Cómo incorporar cursos
Cómo incorporar (por redirección) un curso al sitio web principal

[[toc]]

## Revisión de issues
1. Diríjase a [https://github.com/tc-565/inicio/issues](https://github.com/tc-565/inicio/issues). Allí encontrará una lista de solicitudes de repositorios/cursos para ser agregados al sitio web principal.
2. **Importante:** verifique al usuario que hizo la solicitud, y que verdaderamente sea un estudiante del TCU.
3. Revise el contenido del repositorio enlazado.
4. Revise que el sitio cumpla con todo [lo que se le solicita](https://tc-565.github.io/inicio/topic-01-crear/unit-03-creacion/note-03-revision/index.html) a un creador de cursos justo antes de poner el repositorio en un issue.

## Copiar repositorio
1. Proceda al repositorio provisto en el issue, y presione `Fork` cerca del extremo superior derecho. Esto creará una copia del repositorio bajo el usuario del TCU.
2. En el repositorio copiado, siga las instrucciones bajo el título [Habilitación de GH-pages y compilación automática](https://tc-565.github.io/inicio/topic-01-crear/unit-03-creacion/note-01-clonar-plantilla/index.html#habilitación-de-gh-pages-y-compilación-automática).
3. Puede que sea necesario ir a `Settings`, luego a `Pages` en la barra lateral izquierda, y bajo el título `Build and Deplyment`, bajo `source` escoja la opción `Deploy from a branch`. Revise que esta rama sea `gh-pages`. 

## Agregar al sitio principal
En [https://github.com/tc-565/inicio/tree/main/unit-01-material](https://github.com/tc-565/inicio/tree/main/unit-01-material) agregue el enlace donde se despliega el sitio web bajo el usuario del TCU (por ejemplo https://tc-565.github.io/nuevo-curso) como un elemento de tipo `web` (esto es descrito en [https://tc-565.github.io/inicio/topic-01-crear/unit-03-creacion/note-02-estructura-curso/index.html#web])(https://tc-565.github.io/inicio/topic-01-crear/unit-03-creacion/note-02-estructura-curso/index.html#web).