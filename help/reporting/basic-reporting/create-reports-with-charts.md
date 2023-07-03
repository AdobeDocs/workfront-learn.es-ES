---
title: Creación de informes con gráficos
description: Descubra cómo los gráficos pueden mejorar la visualización de los datos y cómo utilizar las herramientas de gráficos en Workfront.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 100%

---

# Creación de informes con gráficos

Este vídeo contiene información sobre:

* Cómo los gráficos pueden mejorar la visualización de datos
* Cómo utilizar las herramientas de gráficos de Workfront

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## Actividad: Agregar un gráfico a un informe

Se acerca el final del trimestre y usted quiere ver cómo se han ajustado a sus presupuestos los proyectos finalizados recientemente. Cree un informe que muestre el coste planificado frente al coste real de los proyectos. Solo desea ver los proyectos completados en el último trimestre. Agregue un gráfico de columnas combinado con colores personalizados.

## Respuesta

1. Seleccione **[!UICONTROL Informes]** desde el **[!UICONTROL Menú principal]**.
1. Haga clic en el menú **[!UICONTROL Nuevo informe]** y seleccione **[!UICONTROL Proyecto]**.
1. En la pestaña **[!UICONTROL Columnas (Vista)]**, haga clic en **[!UICONTROL Agregar columna]**.
1. Seleccione [!UICONTROL Proyecto] > [!UICONTROL Coste planificado] y resuma esta columna mediante **[!UICONTROL Suma]**.
1. Haga clic en **[!UICONTROL Agregar columna]** de nuevo.
1. Seleccione [!UICONTROL Proyecto] > [!UICONTROL Coste real] y resuma esta columna mediante **[!UICONTROL Suma]**.

   ![Imagen de la pantalla para agregar columnas a un informe](assets/chart-report-columns.png)

1. En la pestaña **[!UICONTROL Agrupaciones]**, configure el informe para agruparlo por [!UICONTROL Proyecto] > [!UICONTROL Nombre].

   ![Imagen de la pantalla para agregar agrupaciones a un informe](assets/chart-report-groupings.png)

1. En la pestaña **[!UICONTROL Filtros]** agregue estas dos reglas de filtro:

   * [!UICONTROL Proyecto] > [!UICONTROL Estado equivale a] > [!UICONTROL Completar]
   * [!UICONTROL Proyecto] >[!UICONTROL  Fecha de finalización real] > [!UICONTROL Último trimestre]

   ![Imagen de la pantalla para agregar filtros a un informe](assets/chart-report-filters.png)

1. En la pestaña **[!UICONTROL Gráfico]**, elija **[!UICONTROL Columna]** para el tipo de gráfico.
1. Para el [!UICONTROL Eje izquierdo (Y)], elija [!UICONTROL Proyecto] > [!UICONTROL Coste planificado].
1. Para el [!UICONTROL Eje inferior (X)], elija [!UICONTROL Proyecto] > [!UICONTROL Nombre].
1. Haga clic en el botón **[!UICONTROL Gráfico de combinación]** y seleccione [!UICONTROL Proyecto] > [!UICONTROL Coste real] en el campo **[!UICONTROL Valor]**.
1. Haga clic en la flecha situada junto a la casilla de color para cambiar el color del [!UICONTROL Coste real]. Seleccione uno de los colores que aparecen o haga clic en la casilla de la esquina inferior derecha para que aparezca la paleta de colores.
1. Haga clic en **[!UICONTROL Guardar + Cerrar]**. Cuando se le pida el nombre de un informe, escriba “Coste planificado frente a coste real por proyecto completado en el último trimestre”.

   ![Imagen de la pantalla para agregar un gráfico a un informe](assets/chart-report-chart.png)
