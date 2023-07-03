---
title: Información sobre las múltiples tasas de facturación
description: Obtenga información sobre cómo anular las tasas de facturación del sistema en un proyecto.
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
ht-degree: 100%

---

# Información sobre las múltiples tasas de facturación

En [!DNL Workfront], un administrador del proyecto tiene la capacidad de anular las tasas de facturación del sistema dentro de un proyecto específico. Anteriormente, cuando se aplicaba la nueva tasa de facturación al proyecto, no solo afectaba a las horas futuras, sino también a las horas ya registradas en el proyecto.

Con la nueva funcionalidad de múltiples tasas de facturación de [!DNL Workfront], el administrador del proyecto puede decidir qué período de tiempo se debe aplicar a una tasa de facturación. De esta manera, si se ha negociado o modificado una tasa, el director del proyecto puede determinar cuándo debe aplicarse esa tasa.

## Cambiar la tasa de facturación

1. Vaya a la página de aterrizaje del proyecto. Seleccione **[!UICONTROL Tasas de facturación]** en el panel izquierdo.

   ![Una imagen seleccionando [!UICONTROL Tasas de facturación] en [!DNL Workfront]](assets/project-finances-1.png)

1. En la pestaña **[!UICONTROL Tasas de facturación]**, haga clic en el botón **[!UICONTROL Añadir tasa de facturación]**. Seleccione **[!UICONTROL Nueva tasa de facturación]** en la lista desplegable.

   ![Una imagen que muestra la selección de la [!UICONTROL Nueva tasa de facturación] en [!DNL Workfront]](assets/project-finances-2.png)

1. Aparece el cuadro de diálogo [!UICONTROL Nueva tasa de facturación]. En el menú desplegable **[!UICONTROL Función del trabajo]**, seleccione la función de trabajo a la que se aplicará la nueva tasa de facturación.

   ![Una imagen que muestra la selección de funciones de trabajo en una nueva tasa de facturación en [!DNL Workfront]](assets/project-finances-3.png)

1. Una vez seleccionada la función de trabajo, aparecen los campos [!UICONTROL Tasa de facturación predeterminada] y [!UICONTROL Tasa de facturación 1]. Introduzca la nueva tasa de facturación en el campo [!UICONTROL Tasa de facturación 1]. Si la tasa de facturación se aplica a todo el proyecto (horas pasadas, presentes y futuras registradas), haga clic en el botón **[!UICONTROL Guardar]**.

   ![Una imagen que muestra cómo guardar una nueva tasa de facturación que se aplica a todo el proyecto en [!DNL Workfront]](assets/project-finances-5.png)

1. Si la nueva tasa de facturación solo se aplica durante un período de tiempo determinado, haga clic en el botón **[!UICONTROL Añadir tasa]**. Aparecen los campos [!UICONTROL Fecha de finalización de tasa de facturación 1] y [!UICONTROL Tasa de facturación 2]. Introduzca la fecha de finalización de [!UICONTROL Tipo de facturación 1]. No puede especificar una fecha de inicio para [!UICONTROL Tipo de facturación 1], porque el sistema supone que se inició al principio del proyecto.

   ![Una imagen que muestra cómo se crea una nueva tasa de facturación que se aplica a un período determinado, a partir del inicio del proyecto en [!DNL Workfront]](assets/project-finances-6.png)

1. Si no es así, haga lo siguiente:

   * Introduzca la tasa de facturación predeterminada para [!UICONTROL Tasa de facturación 1].
   * Seleccione la fecha de finalización para [!UICONTROL Tasa de facturación 1] ([!UICONTROL Tasa de facturación predeterminada]).
   * La fecha de inicio de [!UICONTROL Tasa de facturación 2] se establecerá automáticamente en el día después de que finalice [!UICONTROL Tasa de facturación 1].
   * Introduzca la tasa de facturación deseada en la sección [!UICONTROL Tasa de facturación 2].
   * Siga añadiendo las tasas de facturación según sea necesario haciendo clic en el botón **[!UICONTROL Añadir tasa]**.
   * Cuando termine, haga clic en **[!UICONTROL Guardar]**.
   * Todas las tasas de facturación se mostrarán en la pestaña [!UICONTROL Tasas de facturación] del proyecto.

   ![Una imagen creando nuevas tasas de facturación que se aplican a los diferentes períodos de tiempo en [!DNL Workfront]](assets/project-finances-7.png)
