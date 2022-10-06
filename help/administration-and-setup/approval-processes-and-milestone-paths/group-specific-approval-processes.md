---
title: Explicación de los procesos de aprobación específicos de grupo
description: Descubra cómo los administradores de grupos pueden crear o editar procesos de aprobación para los grupos que administran.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
kt: 10017
exl-id: 138989b2-32d7-43e5-9660-d7b4172f232a
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Explicación de los procesos de aprobación específicos de grupo

Los administradores de sistemas y grupos pueden crear procesos de aprobación en [!DNL Workfront]. Los administradores del sistema pueden crear procesos para utilizarlos en todo el [!DNL Workfront] o solo para un grupo específico. Los administradores del grupo solo pueden crear o editar procesos para el grupo que administran.

Para un proceso de aprobación que todos puedan utilizar en [!DNL Workfront], asegúrese de que la variable [!UICONTROL &quot;Este proceso de aprobación lo puede usar&quot;] el campo está definido como [!UICONTROL Todos los grupos].

![[!UICONTROL Editar proceso de aprobación] ventana con campo de grupo resaltado](assets/admin-fund-approval-processes-1.png)

Los estados disponibles en la variable [!UICONTROL &quot;Iniciar proceso de aprobación cuando el estado esté establecido en&quot;] depende de la selección del campo &quot;usado por&quot;. con [!UICONTROL Todos los grupos] seleccionado, solo están disponibles los estados bloqueados de todo el sistema.

Para limitar un proceso de aprobación para un grupo específico, seleccione el nombre de ese grupo en la lista para [!UICONTROL &quot;Este proceso de aprobación lo puede usar&quot;] campo .

![[!UICONTROL Editar proceso de aprobación] ventana con campo de grupo expandido](assets/admin-fund-approval-processes-2.png)

La variable [!UICONTROL Todos los grupos] no está disponible para los administradores de grupos.

Cuando se selecciona un grupo específico, solo los estados disponibles para ese grupo aparecen en la [!UICONTROL &quot;Iniciar proceso de aprobación cuando el estado esté establecido en&quot;] para abrir el Navegador.

![[!UICONTROL Editar proceso de aprobación] ventana con campo de estado resaltado](assets/admin-fund-approval-processes-3.png)

