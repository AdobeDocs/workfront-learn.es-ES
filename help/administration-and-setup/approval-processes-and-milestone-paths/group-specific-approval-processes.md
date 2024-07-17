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
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '212'
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

