# Instalación desatendida

# 2 Preparativos

## Personalizamos la MV

![](img/01.png)

Instalon **inkscape**.

---

![](img/02.png)

Instalo **vlc**.

---

# 3. Fichero de respuestas

![](img/03.png)

Instalo **autoyast 2**.

---

![](img/04.png)

Clono el sistema haciendo uso del comando **/sbin/yast2 clone_system**.

---

![](img/05.png)

Hago una copia de seguridad del perfil.

---

## 3.2 Configurar USB en la MV de VirtualBox

![](img/06.png)

Añado el USB en VirtualBox.

---

## 3.3 Copiar fichero XML en pendrive

![](img/07.png)

Localizo dónde está montado el pen-drive y copio el archivo xml al usb.

---

![](img/08.png)

Creo una MV2 nueva con un tamaño de disco duro similar a la anterior.

---

![](./img/09.png)

Añado el USB a la máquina virtual.

---

![](img/10.png)

Eligo instalación y en opciones de arranque escribo **autoyast=usb:///roberto01.xml**.

---

![](img/11.png)

Se instala todo sin problema y compruebo que se guarda el usuario y toda la configuración.

---

# 5. Instalación desatendida desde ISO

## 5.1 Software para editar ficheros ISO

![](img/12.png)

Añado el repositorio para poder descargar isomaster.

---

![](img/13.png)

Instalo isomaster.

---

## 5.2 Peparar la ISO

![](img/14.png)

Inicio isomaster y añado mi archivo .xml al .iso.

---

![](img/15.png)

Grabo la iso modificada como **opensuse-roberto01.iso**.

---

## 5.3 Instalación desatendida desde la ISO

![](img/16.png)

Creo una tercera máquina virtual con el mismo tamaño de disco.

---

![](img/17.png)

Introduzco la iso en la MV3.

---

![](img/18.png)

Veo que OpenSUSE reconoce el archivo .xml.

---

![](img/19.png)

Inicio la máquina después de la instalación y compruebo que el nombre dehost es el mismo, se guarda el usuario y los programas que tenía en la anterior máquina.

---