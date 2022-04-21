<center>

# Cliente GNU/Linux

</center>

## Preparar el cliente

![](img/01.png)

Cambio el nombre de host de la máquina.

---

![](img/02.png)

Establezco las DNS de la máquina.

---

![](img/03.png)

Compruebo el DNS

---

## Unirse al dominio

![](img/04.png)

En `Yast -> Pertenencia a dominio de Windows` Pongo el nombre de mi dominio, activo la autenticación SMB y creo el home del usuario al iniciar sesión.

---

![](img/05.png)

Introduzco las credenciales del **Administrador** del dominio.

---


![](img/06.png)

Compruebo en el PDC que se ha unido correctamente el host.

---

## 4. Abrir sesión en el cliente

![](img/07.png)

Como superusuario, inicio sesión como el usuario **yoda** y ejecuto los comandos **whoami**, **pwd** y **cat /etc/passwd | grep yoda** para comprobar que se ha iniciado sesión correctamente en el dominio.

---

## 5. Recursos compartidos

![](img/08.png)

En el explorador de archivos de linux escribo `smb://ip-del-pdc/perfiles$`, esto me lleva a los recursos compartidos de windows server.