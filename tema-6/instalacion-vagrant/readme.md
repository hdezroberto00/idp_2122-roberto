# Instalación desatendida con vagrant

# 1. Proyecto: Añadir cajas

## 1.1 Imagen, caja o box

Añado la box de vagrant llamada **ubuntu/bionic64**.

![](./img/01.png)

Compruebo que se ha añadido la box.

![](./img/02.png)

## 1.2 Directorio

Creo el directorio **roberto01-va1box.d**

![](./img/03.png)

Dentro de esta carpeta creo el archivo **Vagrantfile** y escribo esto en su interior.

![](img/04.png)

## 1.3 Comprobar

Inicio una nueva instancia de la máquina virtual.

![](img/05.png)

Entro a la MV usando SSH.

![](img/06.png)

## 1.4 Elimianmos la MV

Salgo de la MV, la paro y le elimino.

![](img/07.png)

# 3. Proyecto: Redirección de puertos

## 3.1 Creamos los ficheros

Completo el archivo Vagrantfile para que tenga 2048 MiB de ram y para que el sistema sea enrutado al puerto 80.

![](img/08.png)

## 3.2 Entramos en la MV

Entro en la MV e instalo Apache2.

![](img/09.png)

## 3.3 Comprobar

Veo la redirección de puertos de la máquina Vagrant.

![](img/10.png)

Accedo al puerto 80 del sistema virtualizado.

![](img/11.png)

## 3.4 Eliminar la MV

Elimino la MV.

![](img/12.png)

# 4. Proyecto: Suministro mediante shell script

## 4.1 Crear ficheros

Creo el fichero **index.html** y escribo dentro de él.

![](img/13.png)

Creo un script.

![](img/14.png)

## 4.2 Vagrantfile

Creo el fichero **Vagrantfile** y lo configuro.

![](img/15.png)

## 4.3 Comprobamos

Compruebo que funcionó el apache.

![](img/16.png)

# 5. Proyecto: Suministro mediante Puppet

## 5.1 Preparativos

Creo la carpeta.

![](img/17.png)

Creo y modifico el archivo **Vagrantfile**.

![](img/21.png)

Creo la carpeta **manifests**.

![](img/19.png)

Creo el archivo roberto01.pp y lo modifico.

![](img/20.png)

## 5.3 Comprobamos

Inicio la máquina.

![](img/22.png)

Entro en la MV y compruebo que se ha instalado el software.

![](img/23.png)

# 6. Proyecto: Caja personalizada

## 6.1 Preparar la MV VirtualBox

Utilizo una MV que ya tenía creada.

![](img/24.png)

Creo el usuario **vagrant** y le pongo de contraseña **vagrant**.

![](img/25.png) ![](img/26.png)

Descargo la clave pública.

![](img/27.png)

Modifico los permisos y el propietario de la carpeta.

![](img/28.png)

Añado esta línea a /etc/sudoers.

![](img/29.png)

# 6.2 Crear la caja Vagrant

Creo la carpeta para este paso, veo la lista de MV que tengo en VirtualBox y creo mi propia caja.

![](./img/30.png)

Añado la nueva caja al repositorio local de cajas de vagrant.

![](img/31.png)

Compruebo la lista de cajas vagrant.

![](img/32.png)

## 6.3 Vagrantfile

Edito el fichero Vagrantfile

![](img/33.png)

Inicio la máquina.

![](img/34.png)

Me conecto a la MV por ssh.

![](img/35.png)