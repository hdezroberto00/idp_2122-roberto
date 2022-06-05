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

