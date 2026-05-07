---
title: Explicación de los procesos de aprobación específicos del grupo
description: Información cómo los administradores de grupos pueden crear o editar procesos de aprobación para los grupos que administran.
feature: Approvals
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
hide: true
exl-id: 9986469c-b02f-48ac-b71e-055473a2855b
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:17:51.764Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 214
ht-degree: 100%

---

# Explicación de los procesos de aprobación específicos del grupo

Los administradores de sistemas y grupos pueden crear procesos de aprobación en [!DNL Workfront]. Los administradores del sistema pueden crear procesos para utilizarlos en todo el sistema de [!DNL Workfront] o solo para un grupo específico. Los administradores del grupo solo pueden crear o editar procesos para el grupo que administran.

Para un proceso de aprobación que todos puedan utilizar en [!DNL Workfront], asegúrese de que el campo [!UICONTROL “Este proceso de aprobación lo puede usar”] esté definido como [!UICONTROL Todos los grupos].

Ventana ![[!UICONTROL Editar proceso de aprobación] con campo de grupo resaltado](assets/admin-fund-approval-processes-1.png)

Los estados disponibles en el menú [!UICONTROL “Iniciar proceso de aprobación cuando el estado esté establecido en”] depende de la selección del campo “usado por”. Con [!UICONTROL Todos los grupos] seleccionado, solo están disponibles los estados bloqueados de todo el sistema.

Para limitar un proceso de aprobación para un grupo específico, seleccione el nombre de ese grupo en la lista para el campo [!UICONTROL “Este proceso de aprobación lo puede usar”].

Ventana ![[!UICONTROL Editar proceso de aprobación] con campo de grupo expandido](assets/admin-fund-approval-processes-2.png)

La opción [!UICONTROL Todos los grupos] no está disponible para los administradores de grupos.

Cuando se selecciona un grupo específico, solo los estados disponibles para ese grupo aparecen en el menú [!UICONTROL &quot;Iniciar proceso de aprobación cuando el estado esté establecido en&quot;].

Ventana ![[!UICONTROL Editar proceso de aprobación] con campo de estado resaltado](assets/admin-fund-approval-processes-3.png)
