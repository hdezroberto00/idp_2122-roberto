# Servidor PXE

# 2. Servicio DHCP

## 2.1 Instalar el servicio DHCP

Instalo el servicio DHCP.

![](img/2.1-1.png)

## 2.2 Configurar interfaz de red

Hago copia de seguridad del fichero antes de modificarlo.

![](img/2.2-1.png)

Edito el archivo **/etc/sysconfig/dhcpd**.

![](img/2.2-2.png)

## 2.3 Configurar DHCP

Hago una copia del fichero antes de modificarlo.

![](img/2.3-1.png)

Configuro DHCP.

![](img/2.3-2.png)

Configuro el servicio "dhcpd" para que se inicie automáticamente.

![](img/2.3-3.png)

# 3. Servicio TFTP

Instalo el servicio

![](img/3.1-1.png)

## 3.2 Cambiar la configuración

Edito el archivo /etc/sysconfig/atftpd

![](img/3.2-1.png)  ![](img/3.2-2.png)

Al editarlo de esta manera el servicio se ejcutará con el usuario tftp, por lo que me aseguro que existe.

![](img/3.2-3.png)

# 4. Servicio NFS

## 4.1 Instalar el servicio

Instalo **nfs-kernel-server**.

![](img/4.1-1.png)

Instalo **yast2-nfs-server**.

![](img/4.1-2.png)

## 4.2 Configurar

Descargo una iso de opensuse.

![](img/4.2-1.png)

Creo el directorio **/mnt/opensuse.iso.d**.

![](img/4.2-2.png)

Edito el fichero **/etc/fstab** para crear un punto de montaje para la iso.

![](img/4.2-3.png)

Monto las configuraciones de fstab.

![](img/4.2-4.png)

Compruebo que se ha montado.

![](img/4.2-5.png)

Añado esta línea a **/etc/exports**.

![](img/4.2-6.png)

# 5. Menú de arranque

## 5.1 Preparando el menú

Creo directorios y copio archivos.

![](img/5.1-1.png)

Añado estas líneas al archivo **default**.

![](img/5.1-2.png)

## 5.3 Probando el menú desde el cliente

Inicio la máquina cliente y compruebo que muestra el menú PXE.

![](img/5.3-1.png)

# 6. Configurar una imagen para instalar

Creo un subdirectorio para la .iso y copio archivos.

![](img/6-1.png)

Edito el fichero **/srv/tftpboot/pxelinux.cfg/default**

![](img/6-2.png)

Inicio la máquina cliente y compruebo que muestra la iso que configuré.

![](img/6-3.png)

Selecciono la ISO y compruebo que comienza la instalación.

![](img/6-5.png)

# 7. Otra ISO

Repito los pasos del apartado 6 para añadir otra iso.

![](img/6-6.png)

Compruebo que comienza la instalación.

![](img/6-7.png)