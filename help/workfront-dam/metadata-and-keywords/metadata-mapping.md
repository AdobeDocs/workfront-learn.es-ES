---
title: Configuración de la asignación de metadatos
description: Obtenga información sobre cómo configurar la asignación de metadatos para [!UICONTROL DAM de Workfront].
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T22:32:59.006Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 276
ht-degree: 100%

---

# Configuración de la asignación de metadatos

La información relacionada con [!DNL Workfront] acerca de un recurso se puede transferir de [!DNL Workfront] a [!UICONTROL DAM de Workfront] con el recurso. La opción de asignación de metadatos en el área [!UICONTROL Configuración] de [!DNL Workfront] permite esta transferencia de información.

Hable con su consultor de [!DNL Workfront] acerca de las prácticas recomendadas sobre la configuración de la asignación de metadatos.

Debe ser administrador de [!DNL Workfront] y de [!UICONTROL DAM de Workfront] para configurar la asignación de metadatos. Antes de poder comenzar, debe conectar sus cuentas de [!DNL Workfront] y [!UICONTROL DAM de Workfront].

## Conectar cuentas

1. Iniciar sesión en [!DNL Workfront].
1. Abra un proyecto, tarea o problema y haga clic en la pestaña **[!UICONTROL Documentos]**.
1. Haga clic en el botón **[!UICONTROL Agregar nuevo]** y seleccione **[!UICONTROL Desde DAM de Workfront]** en el menú desplegable.
1. Escriba su nombre de inicio de sesión y contraseña en la casilla de autorización [!UICONTROL DAM de Workfront] que aparece.
1. A continuación, haga clic en **[!UICONTROL Sí]** para dar acceso de [!DNL Workfront] a la cuenta [!UICONTROL DAM].
1. Si es necesario, actualice la página para actualizar el acceso al [!UICONTROL DAM de Workfront].

Con esta conexión establecida, ahora puede empezar a asignar metadatos entre los dos sistemas. Asegúrese de haber creado los campos de metadatos necesarios en [!UICONTROL DAM de Workfront] antes de comenzar la asignación.

## Configuración de la asignación

1. Inicie sesión en [!DNL Workfront].
1. Seleccione **[!UICONTROL Configuración]** en el [!UICONTROL Menú principal].
1. Expanda la sección **[!UICONTROL Documentos]** en el menú del panel izquierdo.
1. A continuación, haga clic en **[!UICONTROL Asignación de metadatos]**.
1. En el campo Workfront, escriba el origen del campo de [!DNL Workfront] a asignar.
1. A continuación, seleccione el campo de metadatos de **[!UICONTROL DAM de Workfront]** correspondiente o de destino.
1. Haga clic en el botón **[!UICONTROL Agregar asignación]**.
1. Verá el [!UICONTROL Origen del campo de Workfront] y el [!UICONTROL Campo de destinatario del DAM de Workfront] en el gráfico situado en la parte inferior de la ventana.
1. Repita el proceso para todos los campos de metadatos deseados.

![Captura de pantalla de [!UICONTROL Asignación de metadatos] en [!DNL Workfront]](assets/01-metadata-mapping.png)
