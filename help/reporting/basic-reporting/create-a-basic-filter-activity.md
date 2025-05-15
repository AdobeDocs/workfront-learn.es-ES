---
title: Creación de actividades de filtro básicas
description: En esta actividad creará un filtro de proyecto denominado "Todos los proyectos del portafolio de marketing" y otro filtro de proyecto denominado "Proyectos de mi propiedad que cierran este mes".
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
last-substantial-update: 2025-05-15T00:00:00Z
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 0755d62240ab307d3759c47c4561264cb4baadab
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 64%

---

# Creación de actividades de filtro básicas


## Actividad 1: todos los proyectos del portafolio de marketing

En esta actividad creará un filtro de proyecto denominado “Todos los proyectos del portafolio de marketing” en la experiencia de [!UICONTROL Filtro heredado]. Esto le mostrará todos los proyectos del portafolio denominados “Portafolio de marketing” independientemente de su estado.

A continuación se incluyen las instrucciones paso a paso.

## Respuesta a la actividad 1

![Imagen de la pantalla para crear un nuevo filtro](assets/basic-filter-activity-1.png)

1. Vaya al área de [!UICONTROL Proyectos] del [!UICONTROL Menú principal]. Muestra una lista de proyectos.
1. Haga clic en el menú **[!UICONTROL Filtro]** y seleccione [!UICONTROL Filtros heredados] si aún no está seleccionado.
1. Seleccione **[!UICONTROL Nuevo filtro]**.
1. Asigne un nombre al filtro “Todos los proyectos del portafolio de marketing”.
1. Haga clic en **[!UICONTROL Agregar regla de filtro]**.
1. Haga clic en el campo **Seleccionar un campo** y empiece a escribir las palabras &quot;[!UICONTROL nombre del portafolio]&quot;. A continuación, seleccione [!UICONTROL Nombre] en el origen del campo [!UICONTROL Proyecto].
1. Deje el operador [!UICONTROL Igual] tal como está.
1. Escriba &quot;[!UICONTROL marketing]&quot; en el campo de búsqueda.
1. Seleccione [!UICONTROL portafolio de marketing] en el supuesto que tenga un portafolio con ese nombre por el que desee filtrar. Si no, utilice simplemente la función de escritura anticipada para encontrar el portafolio que desea.
1. Haga clic en **[!UICONTROL Guardar filtro]**.

## Actividad 2: proyectos que tengo que se cierran este mes

En este vídeo, creará un filtro de proyecto denominado “Proyectos que tengo que se cierran este mes” en la experiencia de [!UICONTROL Filtro heredado]. Si está pendiente de muchos proyectos, este filtro puede ayudarle a centrarse en los que tiene previsto cerrar próximamente.

A continuación se incluyen las instrucciones paso a paso.

>[!VIDEO](https://video.tv.adobe.com/v/3443382/?quality=12&learn=on&enablevpops&captions=spa)

## Respuesta a la actividad 2

![Imagen de la pantalla para crear un nuevo filtro](assets/basic-filter-activity-2.png)

1. Vaya al área de [!UICONTROL Proyectos] del [!UICONTROL Menú principal]. Muestra una lista de proyectos.
1. Haga clic en el menú **[!UICONTROL Filtro]** y seleccione [!UICONTROL Filtros heredados] si aún no está seleccionado.
1. Seleccione **[!UICONTROL Nuevo filtro]**.
1. Asigne un nombre al filtro “Proyectos que tengo que se cierran este mes”.
1. Haga clic en **[!UICONTROL Agregar regla de filtro]**.
1. Haga clic en el campo **Seleccione un campo** y empiece a escribir la palabra &quot;Propietario&quot;. Ahora haga clic en el identificador de propietario en el origen del campo [!UICONTROL Proyecto].
1. Deje el operador [!UICONTROL Igual] tal como está.
1. Escriba &quot;$$&quot; en el campo de búsqueda.
1. Seleccione [!UICONTROL $$USER.ID]. Este es el carácter comodín del usuario que ha iniciado sesión.
1. Haga clic en agregar otra regla de filtro.
1. Haga clic en el campo **Seleccione un campo** y empiece a escribir la palabra &quot;Está completo&quot;. Ahora haga clic en &quot;Está completo&quot; en el origen del campo [!UICONTROL Proyecto].
1. Deje el operador [!UICONTROL Igual] tal como está.
1. Seleccione “Falso”.
1. Haga clic en volver a añadir otra regla de filtro.
1. Haga clic en el campo **Seleccione un campo** y empiece a escribir la palabra &quot;Planificado&quot;. Ahora haga clic en &quot;Fecha planificada de finalización&quot; bajo el origen de campo [!UICONTROL Proyecto].
1. Cambie el operador [!UICONTROL Igual] a [!UICONTROL Este mes].
1. Haga clic en **[!UICONTROL Guardar filtro]**.
