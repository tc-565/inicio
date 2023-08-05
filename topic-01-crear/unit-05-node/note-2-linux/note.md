---
icon: 
  type: ion:logo-tux
  color: e2ac08 
---
# Linux
Instalación de Node.js en Linux

## Node.js 20
Para garantizar el funcionamiento de las aplicaciones que se desean utilizar, se instalará la versión 20 de Node.js, ya que no se puede asegurar que sirvan en versiones posteriores.

### Debian / Ubuntu (apt-get)
1. Actualice sus paquetes ``sudo apt update && sudo apt upgrade``.
2. Instale cURL ``sudo apt install curl``.
3. Agregue el repositorio NodeSource para Node.js 20 LTS con ``curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -``.
4. Instale Node.js 20 ``sudo apt-get install nodejs``

### Fedora (dnf/yum)
``dnf module install nodejs:20/common``
