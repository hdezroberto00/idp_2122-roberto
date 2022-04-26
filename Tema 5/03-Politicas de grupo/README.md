# Políticas de grupo

# 1. Aplicar directivas de Usuario

## 1.1 Crear las OU

![](img/01.png)

Creo una instantánea en la MV PDC antes de empezar la práctica por seguridad.

---

![](img/02.png)

En "Usuarios y equipos del Active Directory" creo una nueva unidad organizativa.

---

![](img/03.png)

Creo las unidades **jedi01** y **sith01**.

---

![](img/04.png)

Añado los usuarios a la unidad jedi.

---

![](img/05.png)

Añado los usuarios a la unidad sith.

---

## 1.2 Crear GPO's

![](img/06.png)

Voy a `Herramientas -> Administración de directivas de grupo` y en la OU de **jedi01** -> botón derecho -> y creo la **GPO_jedi01**.

---

![](img/07.png)

Compruebo que se han creado las GPO.

---

## 1.3 Personalizar cada GPO de forma diferente

Para la directiva **gpo_jedi01** aplico las siguientes directivas.

![](img/08.png) ![](img/09.png)

Directivas de `Menú inicio y barra de tareas` aplicada a la OU de **jedis**.

---

![](img/10.png)

Directivas de `Panel de control` aplicadas a la OU de **siths**.

---

Ahora aplico directivas a la OU de **sith01**.

![](img/11.png) ![](img/12.png)

Directivas de escritorio y explorador de windows aplicadas a la OU de **siths**.

`NOTA: en "Ocultar estas unidades específicas en Mi PC" eligo la combinación de bloquear solo las unidades A y B`

---

## 1.5 Comprobar que se aplican las directivas

![](img/13.png)

Resumen de configuración de la OU **jedi**.

---

![](img/14.png)

Resumen de configuración de la OU **sith**.