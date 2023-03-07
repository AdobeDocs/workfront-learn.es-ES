---
title: Crear una actividad de filtro básica
description: En esta actividad creará un filtro de proyecto llamado "Proyectos de mi propiedad que cierran este mes".
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Crear una actividad de filtro básica

En este vídeo, creará un filtro de proyecto denominado &quot;Proyectos de mi propiedad que cierran este mes&quot;. Si vigila muchos proyectos, este filtro puede ayudarle a aumentar el zoom de los que se planea cerrar pronto.

A continuación se incluyen instrucciones paso a paso.

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12)

## Respuesta

![Imagen de la pantalla para crear un nuevo filtro](assets/basic-filter-activity-updated-6-15-21.png)

1. Vaya a [!UICONTROL Proyectos] del área de [!UICONTROL Menú principal]. Esto le muestra una lista de proyectos.
1. Haga clic en **[!UICONTROL Filtrar]** y seleccione **[!UICONTROL Nuevo filtro]**.
1. Asigne un nombre a su filtro &quot;Proyectos de mi propiedad que cierran este mes&quot;.
1. Clic **[!UICONTROL Agregar regla de filtro]**.
1. En el [!UICONTROL Empiece a escribir el nombre del campo] , escriba &quot;propietario&quot;. A continuación seleccione [!UICONTROL Identificador de propietario] en el [!UICONTROL Proyecto] origen del campo.
1. Deje el [!UICONTROL Igual] operador tal como está.
1. Escriba &quot;$$&quot; en el campo Empiece a escribir el nombre.
1. Seleccionar [!UICONTROL $$USER.ID]. Este es el comodín para el usuario que ha iniciado sesión.
1. Clic [!UICONTROL Agregar regla de filtro] otra vez.
1. En el [!UICONTROL Empiece a escribir el nombre del campo] , empiece a escribir &quot;Is Complete&quot;. A continuación seleccione [!UICONTROL Está completo] en el origen del campo Proyecto.
1. Deje el [!UICONTROL Igual] operador tal como está.
1. Seleccione &quot;Falso&quot;.
1. Clic [!UICONTROL Agregar regla de filtro] otra vez.
1. En el [!UICONTROL Empiece a escribir el nombre del campo] tipo de campo &quot;planificado&quot; y, a continuación, seleccione [!UICONTROL Fecha planificada de finalización] en el [!UICONTROL Proyecto] origen del campo.
1. Cambie el [!UICONTROL Igual] operador a [!UICONTROL Este mes].
1. Clic **[!UICONTROL Guardar filtro]**
