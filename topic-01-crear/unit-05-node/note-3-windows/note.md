---
icon: 
  type: ri:windows-fill
  color: e2ac08 
---
# Windows
Instalación de Node.js en Windows

[[toc]]

## Node.js 20
Para garantizar el funcionamiento de las aplicaciones que se desean utilizar, se instalará la versión 20 de Node.js, ya que no se puede asegurar que sirvan en versiones posteriores.

1. Ingrese al siguiente [sitio](https://nodejs.org/dist/) con todas las versiones de Node.js. En dicha página encontrará diversos directorios con instaladores de Node. Seleccione el más reciente de la forma ``v20.yy.y``, y luego seleccione ``node-v20.yy.y-x64.msi``.
2. Una vez descargado el archivo .msi, haga doble clic para iniciarlo e iniciar el instalador de Node.js.
3. Se abrirá una ventana de instalación. Haga clic en "Next" o "Siguiente" para comenzar con la instalación.
4. Aceptar el acuerdo de licencia y hacer clic en "Next" o "Siguiente".
5. El instalador le permitirá seleccionar los componentes que desea instalar. Normalmente, deje seleccionadas todas las opciones predeterminadas y luego haga clic en "Next" o "Siguiente".
6. El siguiente paso es elegir la ubicación de instalación. Por lo general, se recomienda dejar la ubicación predeterminada y hacer clic en "Next" o "Siguiente".
7. A continuación, el instalador le preguntará si desea agregar Node.js al PATH del sistema. Marque esta opción para que puedas usar Node.js y npm desde la línea de comandos sin tener que especificar la ruta completa. Después de seleccionar la opción, haga clic en "Next" o "Siguiente".
8. Haga clic en "Install" o "Instalar" para comenzar el proceso de instalación.
9. Una vez que la instalación se complete, haga clic en "Finish" o "Finalizar".
10. Para verificar si la instalación fue exitosa, abra la línea de comandos (CMD) o PowerShell y escriba los siguientes comandos:
```
node -v
npm -v
```
Estos comandos mostrarán la versión de Node.js y npm instalados en el sistema. Si ve las versiones correspondientes, la instalación fue exitosa.