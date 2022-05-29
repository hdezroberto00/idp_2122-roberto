## Servidor de actualizaciones con OpenSuse

## Servidor Web

## 1.1 Instalación

Instalo el servidor web Apache.

![](img/1.1-1.png)

Activo que apache2 al inicio.

![](img/1.1-2.png)

Compruebo el estado de apache2.

![](img/1.1-3.png)

## 1.2 Cortafuegos

Abro el puerto 80 en el cortafuegos por comandos.

![](img/1.2-1.png)

Creo el fichero /srv/www/htdocs/index.html y escribo mi nombre dentro.

![](img/1.2-2.png)

# 2 Preparar el repositorio local

## 2.1 Descargar ficheros rpm

Limpio todo lo que se haya quedado en caché de zypper.

![](img/2.1-1.png)

Descargo geany.

![](img/2.1-2.png)

Descargo nmap.

![](img/2.1-3.png)

Descargo tree.

![](img/2.1-4.png)

Veo los paquetes descargados.

![](img/2.1-5.png)

## 2.2 Copiar ficheros a nuestro repositorio.

Creo el directorio local **/srv/www/htdocs/repo/roberto01** 

![](img/2.2-1.png)

Copio directorios y ficheros desde la caché de zypper.

![](img/2.2-2.png)

Compruebo el contenido del repositorio.

![](img/2.2-3.png)

## 2.3 Crear el fichero índice

Instalo la herramienta createrepo.

![](img/2.3-1.png)

Compruebo el contenido actual del repositorio.

![](img/2.3-2.png)

Creo lo índices de mi repositorio.

![](img/2.3-3.png)

Compruebo el contenido final de mi repositorio.

![](img/2.3-4.png)

# 3. Cliente del repositorio

## 3.1 Comprobar acceso

Abro el navegador para comprobar que tengo acceso desde la MV2 a los ficheros de MV1.

![](img/3.1-1.png)

## 3.2 Añadir nuevo repositorio

Añado nuevo repositorio.

![](img/3.2-1.png)

Establezco el nombre y la URL del repositorio.

![](img/3.2-2.png)

Listado de repositorios.

![](img/3.2-3.png)

Compruebo que la configuración del repositorio nuevo está en este fichero de texto.

![](img/3.2-4.png)

## 3.3 Comprobamos el repositorio desde el cliente

Refresco los repositorios y pruebo a instalar un paquete.

![](img/3.3-1.png)

Pruebo la instalación de un paquete que no está en nuestro repositorio.

![](img/3.3-2.png)