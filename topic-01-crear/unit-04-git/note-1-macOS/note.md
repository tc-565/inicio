---
icon: 
  type: ic:baseline-apple
  color: e2ac08 
---
# macOS
Instalación de Git y GitHub Desktop en macOS

[[toc]]

## Homebrew
Para instalar Git y GitHub Desktop, y posteriormente Node, lo mejor es instalar el reconocido gestor de paquetes Homebrew para macOS.

Navegue al sitio de Homebrew, [https://brew.sh](https://brew.sh), y siga la instrucciones de instalación.

## Git
Una vez con Homebrew instalado, git se habrá instalado automáticamente al instalar Xcode Command Line Tools, una colección oficial de utilitarios proporcionada por Apple.

En la terminal, configure su nombre de usuario y correo electrónico de Git utilizando los siguientes comandos, reemplazando el nombre con el suyo. Estos detalles estarán asociados con los commits que vaya a crear:

```bash
$ git config --global user.name "Nombre"
$ git config --global user.email "correo@example.com"
```

## GitHub Desktop
Proceda a la aplicación ``Terminal``, e ingrese el comando
~~~
brew install --cask github
~~~

Podrá encontrar la aplicación GitHub Desktop en la carpeta de Aplicaciones y en el Launchpad.