---
title: Exploración de los filtros de problemas integrados
description: Obtenga información sobre cómo revisar los filtros de problemas integrados para ver cómo se crean y crear su propio filtro de problemas en Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336819.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: '2025-07-25T00:00:00.000Z'
jira: KT-9085
exl-id: c1bdea98-e70a-4e93-935c-b8f7754afa21
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: c68e30a0-f1f0-47be-a6a9-f26cd55c41a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T02:09:28.024Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 279
ht-degree: 53%

---

# Exploración de los filtros de problemas integrados

En este vídeo, aprenderá lo siguiente:

* Revise los filtros de problema integrados para ver cómo se crean
* Obtenga información sobre algunos elementos útiles de creación de informes de problemas
* Información sobre cómo crear su propio filtro de problemas

>[!VIDEO](https://video.tv.adobe.com/v/336819/?quality=12&learn=on&enablevpops=0)


## Actividades de &quot;Comprensión de los filtros de problemas integrados&quot;


### Actividad: creación de un informe de problemas

Desea ver todos los problemas que aún deben resolverse en todos los proyectos activos que posee, incluidos los problemas con un objeto de resolución. Cree un informe de problemas y asígnele el nombre &quot;Problemas no resueltos en proyectos de mi propiedad&quot;.

### Respuesta

Este es el aspecto que debería tener el filtro:

![Una imagen de la pantalla para crear un filtro de problemas](assets/opening-built-in-issue-filters-1.png)

En el filtro integrado &quot;Mis problemas abiertos&quot;, una de las reglas de filtro excluía cualquier problema en el que hubiera un objeto de resolución. El razonamiento detrás de esto es que no tienes que preocuparte por esos temas. Alguien ya ha creado un proyecto, tarea o problema que los resolverá. ¿Qué hay de qué preocuparse? Pero aún no se han resuelto, y en nuestro ejemplo los incluimos para que sean fáciles de identificar y comprobar cómo lo están haciendo.

Para ello, debe agregar una columna en la pestaña Ver para &quot;Problema >> Objeto de resolución&quot;. Muestra el nombre del objeto de resolución, si hay uno, si es un proyecto, una tarea o un problema. Al hacer clic en el nombre se accede al objeto de resolución.

Es posible que desee agrupar la lista en función del nombre del proyecto.

Este es el aspecto que debería tener el informe:

![Imagen de un informe de problemas](assets/opening-built-in-issue-filters-2.png)
