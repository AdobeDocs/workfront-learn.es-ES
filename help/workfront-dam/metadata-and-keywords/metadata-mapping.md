---
title: Configure la asignación de metadatos para [!UICONTROL DAM de Workfront]
description: Obtenga información sobre cómo configurar la asignación de metadatos para [!UICONTROL DAM de Workfront].
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
kt: 10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: 2e0555a45d753a56628cf748537a6007ed548206
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Asignación de metadatos

[!DNL Workfront]La información relacionada con un recurso se puede transferir de [!DNL Workfront] into [!UICONTROL DAM de Workfront] con el recurso. La opción de asignación de metadatos en la variable [!DNL Workfront] [!UICONTROL Configuración] permite esta transferencia de información.

Hable con su [!DNL Workfront] consultor de recomendaciones de prácticas recomendadas sobre la configuración de la asignación de metadatos.

Debe ser [!DNL Workfront] administrador y [!UICONTROL DAM de Workfront] administrador para configurar la asignación de metadatos. Antes de poder empezar, debe conectar su [!DNL Workfront] y [!UICONTROL DAM de Workfront] cuentas.

## Conectar cuentas

1. Iniciar sesión en [!DNL Workfront].
1. Abra un proyecto, tarea o problema y haga clic en el botón **[!UICONTROL Documentos]** pestaña .
1. Haga clic en el **[!UICONTROL Agregar nuevo]** y seleccione **[!UICONTROL Desde Workfront DAM]** en el menú desplegable.
1. Escriba su nombre de inicio de sesión y contraseña en la [!UICONTROL DAM de Workfront] que aparece.
1. A continuación, haga clic en **[!UICONTROL Sí]** para dar [!DNL Workfront] acceso al [!UICONTROL DAM] cuenta.
1. Si es necesario, actualice la página para actualizar el acceso a [!UICONTROL DAM de Workfront].

Con esta conexión establecida, ahora puede empezar a asignar metadatos entre los dos sistemas. Asegúrese de que ya ha creado los campos de metadatos necesarios en [!UICONTROL DAM de Workfront] antes de comenzar la asignación.

## Configuración de la asignación

1. Iniciar sesión en [!DNL Workfront].
1. Select **[!UICONTROL Configuración]** de la variable [!UICONTROL Menú principal].
1. Expanda el **[!UICONTROL Documentos]** en el menú del panel izquierdo.
1. A continuación, haga clic en **[!UICONTROL Asignación de metadatos]**.
1. En el campo Workfront , escriba el origen del campo de la variable [!DNL Workfront] campo a asignar.
1. A continuación, seleccione el destino o correspondiente **[!UICONTROL DAM de Workfront]** campo de metadatos.
1. Haga clic en el **[!UICONTROL Agregar asignación]** botón.
1. Verá el [!UICONTROL Fuente de campos de Workfront] y [!UICONTROL Campo de objetivo de Workfront DAM] en el gráfico situado en la parte inferior de la ventana.
1. Repita el proceso para todos los campos de metadatos deseados.

![Captura de pantalla del [!UICONTROL Asignación de metadatos] en la pantalla [!DNL Workfront]](assets/01-metadata-mapping.png)
