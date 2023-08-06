---
icon: 
  type: material-symbols:rule
  color: e2ac08 
---
# Aspectos generales
Aspectos generales de mantenimiento

[[toc]]

## tutors
El sitio web y la generación de cursos se apoya en los paquetes de código abierto [tutors](https://github.com/tutors-sdk/tutors) para la generación de sitios web educativos. En particular se utiliza la herramienta de generación de sitios web estáticos, antiguamente [tutors-html](https://www.npmjs.com/package/tutors-html), y ahora [tutors-publish-html](https://www.npmjs.com/package/tutors-publish-html).

Este software es desarrollado por personas en su tiempo libre sin ánimo de lucro, si se encuentran problemas de compilación con el contenido de un curso y desea comunicarlo al resto de la comunidad, sea respetuoso, consulte el [código de conducta](https://github.com/tutors-sdk/tutors/blob/main/CODE_OF_CONDUCT.md), y provea la información técnica más completa posible.

El trabajo y colaboración con los contribuidores del proyecto tutors para la identificación y solución de errores fue fundamental para hacer posible la existencia de este sitio web. Recuerde que las personas que trabajan en él no son remuneradas por ello.

Se motiva a contribuir al desarrollo del proyecto del cual depende este sitio.

## ¿Cómo funciona la compilación automática del sitio web en GitHub?
Como parte de este proyecto, se empleó un script de GitHub Actions que permite la inicialización de un contenedor de Ubuntu, se establece una versión de Node a utilizar, se instala el compilador de tutors, y se ejecuta.

Luego en una rama aparte, se hace un commit con los contenidos del curso compilado. Esta rama es la que luego es desplegada en GitHub pages.

Estas acciones de compilación y despliegue no son inmediatas, pues deben esperar a ser ejecutadas dentro de recursos computacionales compartidos en la nube.

Este script puede ser consultado en [https://github.com/tc-565/plantilla/blob/main/.github/workflows/deploy.yml](https://github.com/tc-565/plantilla/blob/main/.github/workflows/deploy.yml).

**Importante:** puede que este script se deba actualizar en el futuro por la versión de Node y del compilador de cursos. De tener que hacerlo,
1. Cerciórese de que la versión de Node por la cual sustituye a la anterior sea una versión LTS, y que no genere problemas de compilación.
2. Cerciórese de que la nueva versión del compilador compile los sitios web correctamente, y tenga un ojo abierto a las regresiones, revise cuidadosamente.
3. Si hace cualquiera de los cambios anteriores, actualice correspondientemente los apartados avanzados de documentación acerca de ‘Cómo crear un curso’.

## GitHub PRO y el despliegue privado del sitio
Para mantener el sitio desplegado en la web, sea en la dirección provista por GitHub o una personalizada, mientras se tiene el repositorio en modo privado (sin acceso para usuarios sin autorización), se debe aplicar y mantener una suscripción a GitHub PRO.

Como funcionarios de la Universidad de Costa Rica, se puede asociar la cuenta con el sitio web al correo institucional correspondiente, y aplicar a los beneficios educativos de GitHub en [https://education.github.com/benefits](https://education.github.com/benefits). Se deberá proveer información fehaciente que pruebe su asociación activa con la Universidad de Costa Rica.

Los beneficios de estudiante tienen un tiempo de expiración de 1 a 2 años, plazo tras el cual deben ser renovados de la misma manera.

## Modificaciones de la plantilla
Si se hacen modificaciones en la plantilla de cursos, cerciórese de reciprocarlos en todos los cursos bajo el usuario del TCU. Estos cambios pueden ser hechos por un estudiante mediante pull requests, pero deberán ser aprobados en GitHub por el encargado de la cuenta del TCU.

Las modificaciones a reciprocar corresponden a los archivos [`.github/workflows/deploy.yml`](https://github.com/tc-565/plantilla/blob/main/.github/workflows/deploy.yml), [`.gitignore`](https://github.com/tc-565/plantilla/blob/main/.gitignore).