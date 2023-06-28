---
title: Comprender los procesos de aprobación específicos del grupo
description: Descubra cómo los administradores de grupos pueden crear o editar procesos de aprobación para los grupos que administran.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
jira: KT-10017
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Comprender los procesos de aprobación específicos del grupo

Los administradores de sistemas y de grupos pueden crear procesos de aprobación en [!DNL Workfront]. Los administradores del sistema pueden crear procesos para utilizarlos en todo el [!DNL Workfront] o solo para un grupo específico. Los administradores de grupos solo pueden crear o editar procesos para el grupo que administran.

Para un proceso de aprobación que puedan usar todos los usuarios en [!DNL Workfront], asegúrese de que la [!UICONTROL &quot;Este proceso de aprobación lo puede utilizar&quot;] el campo está configurado como [!UICONTROL Todos los grupos].

![[!UICONTROL Editar proceso de aprobación] ventana con el campo de grupo resaltado](assets/admin-fund-approval-processes-1.png)

Los estados disponibles en la variable [!UICONTROL &quot;Iniciar el proceso de aprobación cuando el estado se defina como&quot;] El menú depende de la selección en el campo &quot;utilizado por&quot;. Con [!UICONTROL Todos los grupos] Si se selecciona, solo están disponibles los estados bloqueados de todo el sistema.

Para limitar un proceso de aprobación a un grupo específico, seleccione el nombre de ese grupo en la lista de [!UICONTROL &quot;Este proceso de aprobación lo puede utilizar&quot;] field.

![[!UICONTROL Editar proceso de aprobación] ventana con campo de grupo expandido](assets/admin-fund-approval-processes-2.png)

El [!UICONTROL Todos los grupos] Esta opción no está disponible para los administradores de grupo.

Cuando se selecciona un grupo específico, solo se muestran en la variable los estados disponibles para ese grupo [!UICONTROL &quot;Iniciar el proceso de aprobación cuando el estado se defina como&quot;] menú.

![[!UICONTROL Editar proceso de aprobación] ventana con el campo de estado resaltado](assets/admin-fund-approval-processes-3.png)

