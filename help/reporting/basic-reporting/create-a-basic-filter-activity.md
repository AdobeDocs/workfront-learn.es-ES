---
title: Creación de actividades de filtro básicas
description: En esta actividad creará un filtro de proyecto llamado "Proyectos de mi propiedad que cierran este mes".
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 32%

---

# Creación de actividades de filtro básicas

## Actividad 1: todos los proyectos del portafolio de marketing

En esta actividad creará un filtro de proyecto llamado &quot;Todos los proyectos del portafolio de marketing&quot; en el [!UICONTROL Filtro heredado] experiencia. Esto le mostrará todos los proyectos del portafolio llamados &quot;Portfolio de marketing&quot; independientemente de su estado.

A continuación se incluyen las instrucciones paso a paso.

### Respuesta a la actividad 1

![Imagen de la pantalla para crear un nuevo filtro](assets/basic-filter-activity-1.png)

1. Vaya al área de [!UICONTROL Proyectos] del [!UICONTROL Menú principal]. Muestra una lista de proyectos.
1. Haga clic en **[!UICONTROL Filtrar]** y seleccione [!UICONTROL Filtros heredados].
1. Seleccionar **[!UICONTROL Nuevo filtro]**.
1. Asigne un nombre al filtro &quot;Todos los proyectos del portafolio de marketing&quot;.
1. Haga clic en **[!UICONTROL Agregar regla de filtro]**.
1. En el [!UICONTROL Empiece a escribir el nombre del campo] campo, escriba &quot;[!UICONTROL nombre del portafolio]&quot;. A continuación seleccione [!UICONTROL Nombre] en el [!UICONTROL Portfolio] origen del campo.
1. Deje el operador [!UICONTROL Igual] tal como está.
1. Escriba &quot;[!UICONTROL marketing]&quot; en el [!UICONTROL Empiece a escribir el nombre] field.
1. Seleccionar [!UICONTROL Portfolio de marketing] suponiendo que tenga un portafolio con ese nombre por el que desee filtrar. Si no simplemente utiliza la función de escritura anticipada para encontrar el portafolio que desea.
1. Clic **[!UICONTROL Guardar filtro]**.

## Actividad 2: proyectos de los que soy propietario que cierran este mes

En este vídeo, creará un filtro de proyecto denominado &quot;Proyectos que cerraré este mes&quot; en el [!UICONTROL Filtro heredado] experiencia. Si está atento a muchos proyectos, este filtro puede ayudarle a aumentar el zoom de los que se planea cerrar pronto.

A continuación se incluyen las instrucciones paso a paso.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

### Respuesta a la actividad 2

![Imagen de la pantalla para crear un nuevo filtro](assets/basic-filter-activity-updated-6-15-21.png)

1. Vaya al área de [!UICONTROL Proyectos] del [!UICONTROL Menú principal]. Muestra una lista de proyectos.
1. Haga clic en **[!UICONTROL Filtrar]** y seleccione [!UICONTROL Filtros heredados].
1. Seleccionar **[!UICONTROL Nuevo filtro]**.
1. Asigne un nombre a su filtro &quot;Proyectos que poseo que cerrarán este mes&quot;.
1. Haga clic en **[!UICONTROL Agregar regla de filtro]**.
1. En el [!UICONTROL Empiece a escribir el nombre del campo] , escriba &quot;propietario&quot;. A continuación, seleccione [!UICONTROL ID de propietario] en el origen del campo [!UICONTROL Proyecto].
1. Deje el operador [!UICONTROL Igual] tal como está.
1. Escriba &quot;$$&quot; en la [!UICONTROL Empiece a escribir el nombre] field.
1. Seleccione [!UICONTROL $$USER.ID]. Este es el carácter comodín del usuario que ha iniciado sesión.
1. Haga clic en [!UICONTROL Agregar regla de filtro] de nuevo.
1. En el [!UICONTROL Empiece a escribir el nombre del campo] , empiece a escribir &quot;Is Complete&quot;. A continuación, seleccione [!UICONTROL Se ha completado] en el origen del campo Proyecto.
1. Deje el operador [!UICONTROL Igual] tal como está.
1. Seleccione &quot;Falso&quot;.
1. Haga clic en [!UICONTROL Agregar regla de filtro] de nuevo.
1. En el [!UICONTROL Empiece a escribir el nombre del campo] tipo de campo &quot;planificado&quot; y, a continuación, seleccione [!UICONTROL Fecha planificada de finalización] en el [!UICONTROL Proyecto] origen del campo.
1. Cambie el operador [!UICONTROL Igual] a [!UICONTROL Este mes].
1. Clic **[!UICONTROL Guardar filtro]**.
