---
title: Creación de un informe de matriz
description: Descubra cuándo un informe de matriz puede ser útil y cómo crear un informe de matriz en Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Creación de un informe de matriz

En este vídeo, aprenderá lo siguiente:

* Cuando un informe de matriz puede ser útil
* Y cómo crear un informe de matriz

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## Actividad: Crear un informe de matriz

Cree un informe de matriz que muestre cuántas solicitudes hay en cada estado, ordenadas por cola de solicitudes. Esto le ofrece una visión rápida de la cantidad de trabajo que entra y de cómo lo está haciendo.

Desea que las colas de solicitudes aparezcan en las agrupaciones de filas. El estado aparece como las agrupaciones de columnas. Asigne un nombre al informe &quot;Solicitudes por estado y colas de solicitudes&quot;.

## Respuesta

1. Seleccionar **[!UICONTROL Informes]** desde el **[!UICONTROL Menú principal]**.
1. Haga clic en **[!UICONTROL Nuevo informe]** y seleccione **[!UICONTROL Problema]**.
1. Vaya a la **[!UICONTROL Agrupaciones]** y haga clic en **[!UICONTROL Cambiar a agrupación de matriz]**.
1. Para [!UICONTROL Agrupaciones de filas], seleccione **[!UICONTROL Proyecto]** > **[!UICONTROL Nombre]**.
1. Para [!UICONTROL Agrupación de columnas], seleccione **[!UICONTROL Problema]** > **[!UICONTROL Estado]**.

   ![Imagen de la pantalla para crear una nueva agrupación de informes de problemas](assets/matrix-report-groupings.png)

1. Vaya a la **[!UICONTROL Filtros]** pestaña.
1. Para asegurarse de que solo ve solicitudes en colas de solicitudes activas, agregue las siguientes reglas de filtro:

   * [!UICONTROL Proyecto] > [!UICONTROL Estado igual a] > [!UICONTROL Igual] > [!UICONTROL Actual]
   * [!UICONTROL Definición de cola] > [!UICONTROL Es público] > [!UICONTROL Distinto a] > [!UICONTROL Ninguno] (así es como sabemos que un proyecto es en realidad una cola de solicitudes, por la definición de cola que se asigna a una de las opciones públicas).

1. Haga clic en **[!UICONTROL Guardar + Cerrar]**. Cuando se le pida un nombre de informe, escriba &quot;Solicitudes por estado y Cola de solicitudes&quot;.

   ![Imagen de la pantalla para crear un nuevo filtro de informe de problemas](assets/matrix-report-filters.png)
