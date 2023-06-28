---
title: Comprensión de los filtros de problema integrados
description: Obtenga información sobre cómo revisar los filtros de problemas integrados para ver cómo se crean y crear su propio filtro de problemas en Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336819.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9085
exl-id: c1bdea98-e70a-4e93-935c-b8f7754afa21
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Comprensión de los filtros de problema integrados

En este vídeo hará lo siguiente:

* Revise los filtros de problemas integrados para ver cómo se crean
* Obtenga información acerca de algunos elementos útiles de informes de problemas
* Obtenga información sobre cómo crear su propio filtro de problemas

>[!VIDEO](https://video.tv.adobe.com/v/336819/?quality=12&learn=on)

## Actividad: Crear un informe de problemas

Desea ver todos los problemas que aún deben resolverse en todos los proyectos activos que posee, incluidos los problemas con un objeto de resolución. Cree un informe de problemas y asígnele el nombre &quot;Problemas no resueltos en proyectos de mi propiedad&quot;.

## Respuesta

Este es el aspecto que debería tener el filtro:

![Imagen de la pantalla para crear un filtro de problemas](assets/opening-built-in-issue-filters-1.png)

En el filtro integrado &quot;Mis problemas abiertos&quot;, una de las reglas de filtro excluía cualquier problema en el que hubiera un objeto de resolución. El razonamiento detrás de esto es que no tiene que preocuparse por esos problemas. Alguien ya ha creado un proyecto, una tarea o un problema que los resolverá. ¿Qué hay de qué preocuparse? Pero aún no se han resuelto y, en nuestro ejemplo, los estamos incluyendo para que sean fáciles de identificar y comprobar cómo lo están haciendo.

Para ello, debe agregar una columna en la pestaña Ver para &quot;Problema >> Objeto de resolución&quot;. Muestra el nombre del objeto de resolución, si lo hay, ya sea un proyecto, una tarea o un problema. Al hacer clic en el nombre, se le redirigirá al objeto de resolución.

Es posible que desee agrupar la lista en función del nombre del proyecto.

Este es el aspecto que debería tener el informe:

![Imagen de un informe de problemas](assets/opening-built-in-issue-filters-2.png)
