---
title: Personalización de los estados de problemas en todo el sistema
description: Obtenga información sobre cómo cambiar los nombres de estado de los problemas, controlar los tipos de problemas para los que se utiliza un estado y bloquear/desbloquear estados para la personalización en el nivel de grupo.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
TQID: https://experienceleague.adobe.com/Wo7ObQJmkrsaYDXxaPMYQvDFfQx8wtC8qYi3Nvc6DkY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 392
ht-degree: 100%

---

# Personalización de estados en todo el sistema

[!DNL Workfront] proporciona una variedad de estados predeterminados para dar cabida a los flujos de trabajo de administración de problemas de su organización. Se puede cambiar el nombre de estos estados para que coincidan con la terminología de la organización. Y los estados y se pueden asignar a tipos de problemas específicos.

Se pueden crear estados adicionales, si es necesario. Solo los administradores del sistema pueden crear estados para todo el sistema. Además, los administradores del sistema controlan qué estados pueden ser editados por los administradores del grupo.

Pestaña ![[!UICONTROL Problemas] en la página [!UICONTROL Estados] en [!UICONTROL Configuración]](assets/admin-fund-all-issue-statuses.png)

## Modificación de los estados existentes

[!DNL Workfront] recomienda un número mínimo de estados. Esto facilita la elección del estado correcto para los usuarios y reduce la lista de estados que deben mantenerse.

Puede editar un estado existente para cambiar el nombre, los tipos de problema a los que está asignado, el color relacionado, etc.

![Lista de estados de problemas con la opción [!UICONTROL Editar] resaltada](assets/admin-fund-edit-issue-status.png)

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expanda la sección de **[!UICONTROL Preferencias del proyecto]** en el panel de menú de la izquierda.
1. Seleccione **[!UICONTROL Estados]**.
1. Seleccione la pestaña **[!UICONTROL Problemas]** y asegúrese de que [!UICONTROL Estados del sistema] se muestra en el ángulo superior derecho.
1. Seleccione **[!UICONTROL Lista principal]** para ver los estados de todos los tipos de problemas. Aquí es donde crea o modifica un estado de problema.
1. Pase el puntero por encima del lado derecho del estado cuyo nombre desea cambiar y haga clic en **[!UICONTROL Editar]**.
1. Asigne un nuevo nombre al estado o cambie cualquiera de la otra información, como desee.
1. Bloquee el estado si esta configuración debe aplicarse a todos los usuarios de su instancia [!DNL Workfront].
1. Desbloquee el estado para permitir que los administradores de grupos editen el estado solo para sus grupos.
1. Marque las casillas para el tipo de problema al que se debe aplicar el estado.
1. Haga clic en **[!UICONTROL Guardar]**.

![Ventana para crear un nuevo estado](assets/admin-fund-edit-issue-status-2.png)

### Asignaciones de estado

Es posible que no todos los estados se asignen a todos los tipos de problemas. La página [!UICONTROL Estados] tiene columnas que muestran el tipo de problema para el que se puede utilizar cada estado.

![Solicitud de cambio resaltada en la pestaña Problemas de la página Estados](assets/admin-fund-issue-type-statuses.png)


Para ver solo los estados asignados a un tipo de problema específico, haga clic en el nombre del tipo de problema en la parte superior de la ventana.

Pestaña ![[!UICONTROL Problema] de la página [!UICONTROL Estado] con columnas resaltadas](assets/admin-fund-statuses-issue-type.png)

Desde aquí, puede arrastrar y soltar los problemas en el orden en el que desee que aparezcan en el menú desplegable [!UICONTROL Estado].

Para editar los estados, debe volver a la [!UICONTROL Lista principal].
