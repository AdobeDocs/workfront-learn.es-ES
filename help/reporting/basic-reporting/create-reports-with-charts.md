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
kt: 8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Creación de informes con gráficos

En este vídeo, aprenderá lo siguiente:

* Visualización de datos mediante gráficos
* Cómo utilizar las herramientas de gráficos de Workfront

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12)

## Actividad: agregar un gráfico a un informe

Se acerca el final del trimestre y le gustaría ver hasta qué punto los proyectos finalizados recientemente se atascan en sus presupuestos. Cree un informe que muestre el costo planificado en comparación con el costo real de los proyectos. Desea ver solamente los proyectos que se completaron en el último trimestre. Agregue un gráfico de columnas combinado con colores personalizados.

## Respuesta

1. Seleccionar **[!UICONTROL Informes]** desde el **[!UICONTROL Menú principal]**.
1. Haga clic en **[!UICONTROL Nuevo informe]** y seleccione **[!UICONTROL Proyecto]**.
1. En el **[!UICONTROL Columnas (vista)]** pestaña, haga clic en **[!UICONTROL Agregar columna]**.
1. Seleccionar [!UICONTROL Proyecto] > [!UICONTROL Costo planificado] y resumir esta columna por **[!UICONTROL Sum]**.
1. Clic **[!UICONTROL Agregar columna]** otra vez.
1. Seleccionar [!UICONTROL Proyecto] > [!UICONTROL Costo real] y resumir esta columna por **[!UICONTROL Sum]**.

   ![Imagen de la pantalla para agregar columnas a un informe](assets/chart-report-columns.png)

1. En el **[!UICONTROL Agrupaciones]** pestaña, configure el informe para que se agrupe por [!UICONTROL Proyecto] > [!UICONTROL Nombre].

   ![Imagen de la pantalla para agregar agrupaciones a un informe](assets/chart-report-groupings.png)

1. En el **[!UICONTROL Filtros]** pestaña, agregue dos reglas de filtro:

   * [!UICONTROL Proyecto] > [!UICONTROL Estado igual a] > [!UICONTROL Completar]
   * [!UICONTROL Proyecto] >[!UICONTROL  Fecha real de finalización] > [!UICONTROL Último trimestre]

   ![Imagen de la pantalla para agregar filtros a un informe](assets/chart-report-filters.png)

1. En el **[!UICONTROL Gráfico]** pestaña, elija **[!UICONTROL Columna]** para el tipo de gráfico.
1. Para el [!UICONTROL Eje izquierdo (Y)], elija [!UICONTROL Proyecto] > [!UICONTROL Costo planificado].
1. Para el [!UICONTROL Eje inferior (X)], elija [!UICONTROL Proyecto] > [!UICONTROL Nombre].
1. Haga clic en **[!UICONTROL Gráfico de combinación]** y seleccione [!UICONTROL Proyecto] > [!UICONTROL Costo real] en el **[!UICONTROL Valor]** field.
1. Haga clic en la flecha situada junto al cuadro de color para cambiar el [!UICONTROL Costo real] color. Seleccione uno de los colores que aparecen o haga clic en el cuadro de la esquina inferior derecha para que aparezca la paleta de colores.
1. Haga clic en **[!UICONTROL Guardar + Cerrar]**. Cuando se le pida un nombre de informe, llámele &quot;Costo planificado contra costo real por proyecto completado el último trimestre&quot;.

   ![Imagen de la pantalla para agregar un gráfico a un informe](assets/chart-report-chart.png)
