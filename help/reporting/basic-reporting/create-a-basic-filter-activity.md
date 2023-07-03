---
title: Crear una actividad de filtro básica
description: En esta actividad, creará un filtro de proyecto llamado “Proyectos que tengo que se cierran este mes”.
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
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 100%

---

# Crear una actividad de filtro básica

En este vídeo, creará un filtro de proyecto llamado “Proyectos que tengo que se cierran este mes”. Si está vigilando muchos proyectos, este filtro puede ayudarle a centrarse en los que tiene previsto cerrar próximamente.

A continuación se incluyen las instrucciones paso a paso.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

## Respuesta

![Imagen de la pantalla para crear un nuevo filtro](assets/basic-filter-activity-updated-6-15-21.png)

1. Vaya al área de [!UICONTROL Proyectos] del [!UICONTROL Menú principal]. Muestra una lista de proyectos.
1. Haga clic en el menú **[!UICONTROL Filtro]** y seleccione **[!UICONTROL Nuevo filtro]**.
1. Asigne un nombre al filtro “Proyectos que tengo cerrados este 
mes”.
1. Haga clic en **[!UICONTROL Agregar regla de filtro]**.
1. En el campo [!UICONTROL Empezar a escribir el nombre del campo], escriba “propietario”. A continuación, seleccione [!UICONTROL ID de propietario] en el origen del campo [!UICONTROL Proyecto].
1. Deje el operador [!UICONTROL Igual] tal como está.
1. Escriba “$$” en el campo Iniciar escritura de nombre.
1. Seleccione [!UICONTROL $$USER.ID]. Este es el carácter comodín del usuario que ha iniciado sesión.
1. Haga clic en [!UICONTROL Agregar regla de filtro] de nuevo.
1. En el campo [!UICONTROL Empezar a escribir el nombre del campo], empiece a escribir “Se ha completado”. A continuación, seleccione [!UICONTROL Se ha completado] en el origen del campo Proyecto.
1. Deje el operador [!UICONTROL Igual] tal como está.
1. Seleccione “Falso”.
1. Haga clic en [!UICONTROL Agregar regla de filtro] de nuevo.
1. En el tipo de campo [!UICONTROL Empezar a escribir el nombre del campo] “planificado”, a continuación, seleccione [!UICONTROL Fecha planificada de finalización] en el origen del campo [!UICONTROL Proyecto].
1. Cambie el operador [!UICONTROL Igual] a [!UICONTROL Este mes].
1. Haga clic en **[!UICONTROL Guardar filtro]**
