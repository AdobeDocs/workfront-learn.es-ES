---
title: Comprender las tasas de facturación múltiples
description: En Workfront, un administrador de proyectos puede anular las tasas de facturación del sistema de un proyecto específico.
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
kt: 10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Comprender las tasas de facturación múltiples

Within [!DNL Workfront], un administrador de proyectos tiene la capacidad de anular las tasas de facturación del sistema dentro de un proyecto específico. Anteriormente, cuando se aplicaba la nueva tasa de facturación al proyecto, no solo afectaba a las horas futuras, sino también a las horas ya registradas en el proyecto.

con [!DNL Workfront]Con la nueva capacidad de tasa de facturación múltiple, el administrador del proyecto puede decidir qué período de tiempo se debe aplicar una tasa de facturación. De esta manera, si se ha negociado o modificado una tasa, el director del proyecto puede determinar cuándo debe aplicarse esa tasa.

## Cambiar la tasa de facturación

1. Vaya a la página de aterrizaje del proyecto. Select **[!UICONTROL Tasas de facturación]** del panel izquierdo.

   ![Una imagen de selección [!UICONTROL Tasas de facturación] en [!DNL Workfront]](assets/project-finances-1.png)

1. En el **[!UICONTROL Tasas de facturación]** , haga clic en la pestaña **[!UICONTROL Agregar tasa de facturación]** botón. Select **[!UICONTROL Nueva tasa de facturación]** en la lista desplegable .

   ![Una imagen de selección [!UICONTROL Nueva tasa de facturación] en [!DNL Workfront]](assets/project-finances-2.png)

1. La variable [!UICONTROL Nueva tasa de facturación] aparece en el cuadro de diálogo. En el **[!UICONTROL Función del trabajo]** , seleccione la función de trabajo a la que se aplicará la nueva tasa de facturación.

   ![Una imagen de la selección de funciones de trabajo en una nueva tasa de facturación en [!DNL Workfront]](assets/project-finances-3.png)

1. Una vez seleccionada la función de trabajo, la variable [!UICONTROL Tasa de facturación predeterminada] y [!UICONTROL Tipo de facturación 1] aparece. Introduzca la nueva tasa de facturación en la variable [!UICONTROL Tipo de facturación 1] campo . Si la tasa de facturación se aplica a todo el proyecto (horas pasadas, presentes y futuras registradas), haga clic en el botón **[!UICONTROL Guardar]** botón.

   ![Una imagen de cómo guardar una nueva tasa de facturación que se aplica a todo el proyecto en [!DNL Workfront]](assets/project-finances-5.png)

1. Si la nueva tasa de facturación solo se aplica durante un período de tiempo determinado, haga clic en el botón **[!UICONTROL Agregar tasa]** botón. La variable [!UICONTROL Tipo de Facturación 1 Fecha de Finalización] y [!UICONTROL Tipo de facturación 2] aparecerán. Introduzca la fecha de finalización para [!UICONTROL Tipo de facturación 1]. No puede especificar una fecha de inicio para [!UICONTROL Tipo de facturación 1] porque el sistema supone que se inició al principio del proyecto.

   ![Una imagen de la creación de una nueva tasa de facturación que se aplica a un periodo determinado, comenzando al principio del proyecto en [!DNL Workfront]](assets/project-finances-6.png)

1. Si no es así:

   * Introduzca la tasa de facturación predeterminada para [!UICONTROL Tipo de facturación 1].
   * Seleccione la fecha de finalización para [!UICONTROL Tipo de facturación 1] ([!UICONTROL Tasa de facturación predeterminada]).
   * La fecha de inicio de [!UICONTROL Tipo de facturación 2] se establecerá automáticamente en el día siguiente [!UICONTROL Tipo de facturación 1] termina.
   * Introduzca la tasa de facturación deseada en la variable [!UICONTROL Tipo de facturación 2] para obtener más información.
   * Siga agregando las tasas de facturación según sea necesario haciendo clic en el botón **[!UICONTROL Agregar tasa]** botón.
   * Cuando termine, haga clic en **[!UICONTROL Guardar]**.
   * Todas las tasas de facturación se mostrarán en la variable [!UICONTROL Tasas de facturación] en el proyecto.
   ![Una imagen de la creación de nuevas tasas de facturación que se aplican a los diferentes períodos de tiempo en [!DNL Workfront]](assets/project-finances-7.png)
