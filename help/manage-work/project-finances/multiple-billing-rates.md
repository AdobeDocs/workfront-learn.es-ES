---
title: Comprender las tarifas de facturación múltiples
description: Obtenga información sobre cómo anular las tarifas de facturación del sistema dentro de un proyecto.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Comprender las tarifas de facturación múltiples

En [!DNL Workfront], un administrador de proyectos tiene la capacidad de anular las tarifas de facturación del sistema dentro de un proyecto específico. Anteriormente, cuando se aplicaba la nueva tasa de facturación al proyecto, no solo afectaba a las horas futuras, sino a las horas ya registradas en el proyecto.

Con [!DNL Workfront]La nueva capacidad de tarifa de facturación múltiple de, el administrador del proyecto puede decidir qué período de tiempo se debe aplicar una tarifa de facturación. De este modo, si se ha negociado o modificado una tasa, el jefe de proyecto puede determinar cuándo debe surtir efecto.

## Cambiar la tarifa de facturación

1. Vaya a la página de aterrizaje del proyecto. Seleccionar **[!UICONTROL Tarifas de facturación]** en el panel izquierdo.

   ![Una imagen de selección [!UICONTROL Tarifas de facturación] in [!DNL Workfront]](assets/project-finances-1.png)

1. Desde el **[!UICONTROL Tarifas de facturación]** , haga clic en **[!UICONTROL Agregar tarifa de facturación]** botón. Seleccionar **[!UICONTROL Nueva tarifa de facturación]** en el menú desplegable.

   ![Una imagen de selección [!UICONTROL Nueva tarifa de facturación] in [!DNL Workfront]](assets/project-finances-2.png)

1. El [!UICONTROL Nueva tarifa de facturación] aparece el cuadro de diálogo. Desde el **[!UICONTROL Rol]** , seleccione la función a la que se aplicará la nueva tarifa de facturación.

   ![Imagen de selección de funciones de trabajo en una nueva tarifa de facturación en [!DNL Workfront]](assets/project-finances-3.png)

1. Una vez seleccionada la función, la variable [!UICONTROL Tarifa de facturación predeterminada] y el [!UICONTROL Tarifa de facturación 1] campo aparecerán. Introduzca la nueva tarifa de facturación en la [!UICONTROL Tarifa de facturación 1] field. Si esa tarifa de facturación se aplica a todo el proyecto (horas registradas pasadas, presentes y futuras), haga clic en **[!UICONTROL Guardar]** botón.

   ![Imagen de un guardado de una nueva tarifa de facturación que se aplica a todo el proyecto en [!DNL Workfront]](assets/project-finances-5.png)

1. Si la nueva tarifa de facturación solo se aplica por un período de tiempo determinado, haga clic en **[!UICONTROL Agregar tarifa]** botón. El [!UICONTROL Fecha de finalización de tarifa de facturación 1] y el [!UICONTROL Tarifa de facturación 2] aparecerán los campos de. Introduzca la fecha de finalización de [!UICONTROL Tarifa de facturación 1]. No se puede introducir una fecha de inicio para [!UICONTROL Tarifa de facturación 1] porque el sistema supone que se inició al principio del proyecto.

   ![Imagen de creación de una nueva tarifa de facturación que se aplica a un período de tiempo determinado, empezando por el comienzo del proyecto en [!DNL Workfront]](assets/project-finances-6.png)

1. En caso contrario:

   * Introduzca la tarifa de facturación predeterminada para [!UICONTROL Tarifa de facturación 1].
   * Seleccione la fecha final de [!UICONTROL Tarifa de facturación 1] ([!UICONTROL Tarifa de facturación predeterminada]).
   * La fecha de inicio de [!UICONTROL Tarifa de facturación 2] se establecerá automáticamente en el día siguiente [!UICONTROL Tarifa de facturación 1] termina.
   * Introduzca la tarifa de facturación deseada en la [!UICONTROL Tarifa de facturación 2] sección.
   * Siga agregando tarifas de facturación, según sea necesario, haciendo clic en el **[!UICONTROL Agregar tarifa]** botón.
   * Cuando termine, haga clic en **[!UICONTROL Guardar]**.
   * Todas las tarifas de facturación se mostrarán en la [!UICONTROL Tarifas de facturación] en el proyecto.

   ![Una imagen de la creación de nuevas tarifas de facturación que se aplican a los diferentes períodos de tiempo en [!DNL Workfront]](assets/project-finances-7.png)
