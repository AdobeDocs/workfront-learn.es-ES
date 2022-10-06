---
title: Creación de informes con gráficos
description: En este vídeo, aprenderá cómo los gráficos pueden mejorar la visualización de los datos y cómo utilizar las herramientas de gráficos en [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
kt: 8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
source-git-commit: f4000878d453c58fabf34308a8e3ab31d9667a1f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Creación de informes con gráficos

En este vídeo, aprenderá:

* Cómo pueden mejorar los gráficos la visualización de datos
* Cómo utilizar las herramientas de gráficos de Workfront

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12)

## Actividad: Agregar un gráfico a un informe

Se acerca el final del trimestre y querrá ver cómo los proyectos completados recientemente se atascan a sus presupuestos. Cree un informe que muestre el coste planeado frente al coste real de los proyectos. Solo desea ver los proyectos completados en el último trimestre. Agregue un gráfico de columnas combinado con colores personalizados.

## Respuesta

1. Select **[!UICONTROL Informes]** de la variable **[!UICONTROL Menú principal]**.
1. Haga clic en el **[!UICONTROL Nuevo informe]** y seleccione **[!UICONTROL Proyecto]**.
1. En el **[!UICONTROL Columnas (Vista)]** , haga clic en **[!UICONTROL Agregar columna]**.
1. Select [!UICONTROL Proyecto] > [!UICONTROL Coste planificado] y resume esta columna por **[!UICONTROL Sum]**.
1. Haga clic en **[!UICONTROL Agregar columna]** de nuevo.
1. Select [!UICONTROL Proyecto] > [!UICONTROL Costo real] y resume esta columna por **[!UICONTROL Sum]**.

   ![Imagen de la pantalla para agregar columnas a un informe](assets/chart-report-columns.png)

1. En el **[!UICONTROL Agrupaciones]** , configure el informe para agruparlo por [!UICONTROL Proyecto] > [!UICONTROL Nombre].

   ![Imagen de la pantalla para agregar agrupaciones a un informe](assets/chart-report-groupings.png)

1. En el **[!UICONTROL Filtros]** , agregue dos reglas de filtro:

   * [!UICONTROL Proyecto] > [!UICONTROL Estado es igual a con] > [!UICONTROL Completar]
   * [!UICONTROL Proyecto] >[!UICONTROL  Fecha de finalización real] > [!UICONTROL Último trimestre]

   ![Imagen de la pantalla para agregar filtros a un informe](assets/chart-report-filters.png)

1. En el **[!UICONTROL Gráfico]** , elija **[!UICONTROL Columna]** para el tipo de gráfico.
1. Para la variable [!UICONTROL Eje izquierdo (Y)], elija [!UICONTROL Proyecto] > [!UICONTROL Coste planificado].
1. Para la variable [!UICONTROL Eje inferior (X)], elija [!UICONTROL Proyecto] > [!UICONTROL Nombre].
1. Haga clic en el **[!UICONTROL Gráfico de combinación]** y seleccione [!UICONTROL Proyecto] > [!UICONTROL Costo real] en el **[!UICONTROL Valor]** campo .
1. Haga clic en la flecha situada junto al cuadro de color para cambiar la [!UICONTROL Costo real] color. Seleccione uno de los colores que aparecen o haga clic en el cuadro de la esquina inferior derecha para que aparezca la paleta de colores.
1. Haga clic en **[!UICONTROL Guardar + Cerrar]**. Cuando se le pida el nombre de un informe, llámele &quot;Costo planeado frente a costo real por proyecto completado en el último trimestre&quot;.

   ![Imagen de la pantalla para agregar un gráfico a un informe](assets/chart-report-chart.png)
