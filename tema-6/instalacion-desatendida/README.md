# Instalación desatendida

# 2. Preparativos

## Personalizamos la MV

Instalo **inkscape**.

![](img/01.png)

Instalo **vlc**.

![](img/02.png)

# 3. Fichero de respuestas

Instalo **autoyast 2**.

![](img/03.png)

Clono el sistema haciendo uso del comando **/sbin/yast2 clone_system**.

![](img/04.png)

Hago una copia de seguridad del perfil.

![](img/05.png)

## 3.2 Configurar USB en la MV de VirtualBox

Añado el USB en VirtualBox.

![](img/06.png)

## 3.3 Copiar fichero XML en pendrive

Localizo dónde está montado el pen-drive y copio el archivo xml al usb.

![](img/07.png)

Creo una MV2 nueva con un tamaño de disco duro similar a la anterior.

![](img/08.png)

Añado el USB a la máquina virtual.

![](./img/09.png)

Elijo instalación y en opciones de arranque escribo **autoyast=usb:///roberto01.xml**.

![](img/10.png)

Se instala todo sin problema y compruebo que se guarda el usuario y toda la configuración.

![](img/11.png)

# 5. Instalación desatendida desde ISO

## 5.1 Software para editar ficheros ISO

Añado el repositorio para poder descargar isomaster.

![](img/12.png)

Instalo isomaster.

![](img/13.png)

## 5.2 Peparar la ISO

Inicio isomaster y añado mi archivo .xml al .iso.

![](img/14.png)

Grabo la iso modificada como **opensuse-roberto01.iso**.

![](img/15.png)

## 5.3 Instalación desatendida desde la ISO

Creo una tercera máquina virtual con el mismo tamaño de disco.

![](img/16.png)

Introduzco la iso en la MV3.

![](img/17.png)

Veo que OpenSUSE reconoce el archivo .xml.

![](img/18.png)

Inicio la máquina después de la instalación y compruebo que el nombre dehost es el mismo, se guarda el usuario y los programas que tenía en la anterior máquina.

![](img/19.png)
