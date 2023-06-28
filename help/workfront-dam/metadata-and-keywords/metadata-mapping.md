---
title: Configuración de la asignación de metadatos para [!UICONTROL WORKFRONT DAM]
description: Obtenga información sobre cómo configurar la asignación de metadatos para [!UICONTROL WORKFRONT DAM].
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Asignación de metadatos

[!DNL Workfront]La información relacionada con un activo se puede transferir desde [!DNL Workfront] en [!UICONTROL WORKFRONT DAM] con el recurso. La opción de asignación de metadatos en [!DNL Workfront] [!UICONTROL Configurar] permite esta transferencia de información.

Hable con su [!DNL Workfront] consultor de recomendaciones sobre prácticas recomendadas para configurar la asignación de metadatos.

Debe ser un [!DNL Workfront] administrador y un [!UICONTROL WORKFRONT DAM] para configurar la asignación de metadatos. Antes de empezar, debe conectar su [!DNL Workfront] y [!UICONTROL WORKFRONT DAM] cuentas.

## Conectar cuentas

1. Iniciar sesión en [!DNL Workfront].
1. Abra un proyecto, tarea o problema y haga clic en **[!UICONTROL Documentos]** pestaña.
1. Haga clic en **[!UICONTROL Añadir nuevo]** y seleccione **[!UICONTROL Desde Workfront DAM]** en el menú desplegable.
1. Introduzca su nombre de inicio de sesión y contraseña en la [!UICONTROL WORKFRONT DAM] cuadro de autorización que aparece.
1. A continuación, haga clic en **[!UICONTROL Sí]** para dar [!DNL Workfront] acceso a la [!UICONTROL DAM] cuenta.
1. Si es necesario, actualice la página para actualizar el acceso a [!UICONTROL WORKFRONT DAM].

Con esta conexión establecida, ahora puede empezar a asignar metadatos entre los dos sistemas. Asegúrese de que ya ha creado los campos de metadatos necesarios en [!UICONTROL WORKFRONT DAM] antes de iniciar la asignación.

## Configuración de la asignación

1. Iniciar sesión en [!DNL Workfront].
1. Seleccionar **[!UICONTROL Configurar]** desde el [!UICONTROL Menú principal].
1. Expanda el **[!UICONTROL Documentos]** del menú del panel izquierdo.
1. Luego haga clic en **[!UICONTROL Asignación de metadatos]**.
1. En el campo Workfront, escriba el origen del campo de [!DNL Workfront] campo para asignar.
1. A continuación, seleccione el destino o correspondiente **[!UICONTROL WORKFRONT DAM]** campo de metadatos.
1. Haga clic en **[!UICONTROL Agregar asignación]** botón.
1. Verá el... [!UICONTROL Origen de campo de Workfront] y [!UICONTROL Campo de destino de Workfront DAM] en el gráfico situado en la parte inferior de la ventana.
1. Repita el proceso para todos los campos de metadatos deseados.

![Captura de pantalla del [!UICONTROL Asignación de metadatos] pantalla en [!DNL Workfront]](assets/01-metadata-mapping.png)
