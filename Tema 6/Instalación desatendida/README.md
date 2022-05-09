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

aa