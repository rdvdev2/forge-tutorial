---
layout: page
title: Preparar el entorno de trabajo
order: 1
permalink: /tutorial/entorno
---
Antes de empezar a trabajar con Minecraft Forge, debemos preparar nustro ordenador para ello. Es posible que ya hayas hecho alguna de estas tareas antes si trabajas con Java. Estos pasos solo los tendrás que siguir una vez.
## Instalar el Java Development Kit (JDK)
El JDK es el set de herramientas que nos permitirá compliar y ejecutar codigo Java (Minecraft está escrito en este lenguaje). El proceso para conseguirlo varia un poco según el sistema operativo.
### Windows
Para empezar nos dirigiremos a la [página de descargas de Java](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) y aceptaremos los términos y condiciones del JDK. Una vez aceptados, buscaremos en la lista de descargas la correspondiente a nuestro sistema: Windows x86 (32 bits) o Windows x64 (64 bits). El link de la derecha descargará el instalador correspondiente, el cual ejecutaremos. A partir de aquí el proceso es tan sencillo como seguir los pasos del instaldor. Cuando finalize, avanza a la sección *Instalar un IDE*.
![La página de descargas de Java](/assets/img/jdk_win.jpg)
### Linux basado en Debian (Ubuntu)
En este caso instalaremos el OpenJDK, una distribución del JDK de codigo libre. Para ello ejecutaremos los siguientes  comandos en la consola:
```shell
sudo add-apt-repository ppa:openjdk-r/ppa
sudo apt install openjdk-8-jdk openjdk-8-jre
```
Acabada la instalación, dirigete a la sección *Instalar un IDE*
### Otras distribuciones Linux
El primer paso será obtener el gestor de paquetes `yum`, proceso que varia según la distribución. Una vez obtenido, simplemente ejecuta el siguiente comando en la consola:
```shell
su -c "yum install java-1.8.0-openjdk-devel"
```
## Instalar un IDE
Una vez nuestro ordenador disponga del JDK, el siguiente paso es instalar un IDE (Integrated Development Environment o Entorno de Desarrollo Integrado). Tener un IDE no es obligatorio para desarrollar mods, aunque si muy recomendado, ya que nos facilitará muchas tareas. Cualquier IDE compatible con Java nos servirà pero Minecraft Forge da soporte a dos: *Eclipse* y *IntelliJ IDEA*. Aquí explicaré como instalar el último, ya que és el que yo uso y más recomiendo.

![Página de descargas de *IntelliJ IDEA*](/assets/img/idea.jpg)

Antes de instalar *Intellij IDEA* deberemos elegir una de las dos ediciones que ofrece: *Comunity* o *Ultimate*. La última incluye bastantes funciones adicionales y es de pago, aunque la empresa ofrece bastantes descuentos, e incluso ofrece el programa gratis a los estudiantes. Una vez elegida la edición, nos dirigiremos a la [página de descargas de *IntelliJ IDEA*](https://www.jetbrains.com/idea/download/). Aquí elegiremos la edición y empezará la descarga. Si estamos usando Windows solo tendremos que arrancar el ejecutable y seguir las instrucciones del instalador. Si, por otra parte, estamos usando linux, deberemos empezar por descomprimir el archivo:
```shell
tar -xzf idea-xxxx.x.x.tar.gz
```
Despues entraremos a la carpeta donde hemos descomprimido el archivo y ejecutaremos el programa:
```shell
cd idea-xxxx.x.x/bin
chmod +x ./idea.sh
./idea.sh
```
A partir de aquí el proceso de instalación es igual al de Windows: seguir las instrucciones hasta finalizar la instalación.
## Para acabar
Una vez instalado el JDK i el IDE, ya tenemos nuestro ordenador listo para meternos de lleno en el *modding*. El primer paso por tanto serà [crear un nuevo proyecto](#).