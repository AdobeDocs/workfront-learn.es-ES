---
title: Creación de un informe de matriz
description: Descubra cuándo puede ser útil un informe de matriz y cómo crear uno en Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: 2c9e57b8f85c74061bd3e52ef4eaea60bc4ec5bb
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 78%

---

# Creación de un informe de matriz

Este vídeo contiene información sobre:

* Cuando un informe de matriz puede resultar útil
* Y cómo crear un informe de matriz

>[!VIDEO](https://video.tv.adobe.com/v/3448186/?quality=12&learn=on&captions=spa)

## Actividades &quot;Crear un informe de matriz&quot;

### Actividad 1: Crear un informe de matriz

Cree un informe de matriz que muestre cuántas solicitudes hay en cada estado, ordenadas por la cola de solicitudes. Esto le proporciona una instantánea rápida de la cantidad de trabajo que ingresa y de lo bien que lo está llevando.

Quiere que las colas de solicitudes aparezcan en las agrupaciones de filas. El estado aparece como las agrupaciones de columnas. Asigne un nombre al informe &quot;Solicitudes por estado y colas de solicitudes&quot;.

### Respuesta 1

1. Seleccione **[!UICONTROL Informes]** desde el **[!UICONTROL Menú principal]**.
1. Haga clic en la opción **[!UICONTROL Nuevo informe]** y seleccione **[!UICONTROL Problema]**.
1. Vaya a la pestaña **[!UICONTROL Agrupaciones]** y haga clic en **[!UICONTROL Cambiar a agrupación de matriz]**.
1. Para [!UICONTROL Agrupaciones de filas], seleccione **[!UICONTROL Proyecto]** > **[!UICONTROL Nombre]**.
1. Para [!UICONTROL Agrupación de columnas], seleccione **[!UICONTROL Problema]** > **[!UICONTROL Estado]**.

   ![Una imagen de la pantalla para crear una nueva agrupación de informes de problemas](assets/matrix-report-groupings.png)

1. Vaya a la pestaña **[!UICONTROL Filtros]**.
1. Para asegurarse de que solo vea solicitudes en colas de solicitudes activas, añada las siguientes reglas de filtro:

   * [!UICONTROL Proyecto] > [!UICONTROL Estado es igual a] > [!UICONTROL Igual] > [!UICONTROL Actual]
   * [!UICONTROL Definición de cola] > [!UICONTROL Es pública] > [!UICONTROL No igual a] > [!UICONTROL Ninguna] (así sabemos que un proyecto es en realidad una cola de solicitudes, ya que la Definición de cola se asigna a una de las opciones públicas).

1. Haga clic en **[!UICONTROL Guardar + Cerrar]**. Cuando se le pida un nombre de informe, escriba &quot;Solicitudes por estado y Cola de solicitudes&quot;.

   ![Una imagen de la pantalla para crear un nuevo filtro de informe de problemas](assets/matrix-report-filters.png)
