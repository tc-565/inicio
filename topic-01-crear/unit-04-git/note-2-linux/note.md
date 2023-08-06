---
icon: 
  type: ion:logo-tux
  color: e2ac08 
---
# Linux
Instalación de Git y GitHub Desktop en Linux

[[toc]]

## Git
### Revisar si hay una instalación existente
Antes que nada, revise si Git está instalado en su sistema con el comando ``git —version``. Si Git no está instalado, habrá un mensaje de error.

### Instalación
Siga las instrucciones de acuerdo a su distribución de Linux.

#### Debian / Ubuntu (apt-get)

Los paquetes de Git están disponibles a través de apt:

1. Desde tu terminal, instale Git utilizando apt-get:

```bash
$ sudo apt-get update
$ sudo apt-get install git
```

2. Verifique que la instalación haya sido exitosa escribiendo el siguiente comando:

```bash
$ git --version
```

3. Configure su nombre de usuario y correo electrónico de Git utilizando los siguientes comandos, reemplazando el nombre con el suyo. Estos detalles estarán asociados con los commits que vaya a crear:

```bash
$ git config --global user.name "Nombre"
$ git config --global user.email "correo@example.com"
```

#### Fedora (dnf/yum)

Los paquetes de Git están disponibles tanto en yum como en dnf:

1. Desde su terminal, instale Git utilizando dnf (o yum, en versiones anteriores de Fedora):

```bash
$ sudo dnf install git
```

o

```bash
$ sudo yum install git
```

2. Verifica que la instalación haya sido exitosa escribiendo el siguiente comando:

```bash
$ git --version
```

3. Configure su nombre de usuario y correo electrónico de Git utilizando los siguientes comandos, reemplazando el nombre con el suyo. Estos detalles estarán asociados con los commits que vaya a crear:

```bash
$ git config --global user.name "Nombre"
$ git config --global user.email "correo@example.com"
```

## GitHub Desktop
Proceda al fork de GitHub Desktop para Linux disponible en [https://github.com/shiftkey/desktop](https://github.com/shiftkey/desktop), vaya a la sección de releases, y descargue la última versión estable correspondiente a los paquetes de la distribución de Linux que utilice.

Adicionalmente, hay un [gist](https://gist.github.com/berkorbay/6feda478a00b0432d13f1fc0a50467f1) con otras opciones de instalación.