---
title: Configuración del proyecto predeterminado global
description: Obtenga información sobre cómo cambiar un estado personalizado, establecer las preferencias globales del proyecto y crear programaciones que sean ajustes predeterminados globales.
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
kt: 8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Configuración de los ajustes predeterminados del proyecto global

<!---
21.4 updates have been made
--->

En este vídeo, aprenderá a:

* Cambiar un estado personalizado
* Definir preferencias globales del proyecto
* Crear y utilizar programaciones

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12&learn=on)

## Configuración de proyecto, tarea y problema global y de grupo

Al abrir el [!UICONTROL Proyectos] configuración de [!DNL Workfront], notará que dice &quot;[!UICONTROL Preferencias del proyecto del sistema]&quot; en la barra de búsqueda de la parte superior de la ventana. Esto le permite saber que esta configuración afecta a todos los [!DNL Workfront] sistema — es una configuración global.

![[!UICONTROL Preferencias de proyecto] en [!UICONTROL Configuración]](assets/admin-fund-system-project-preferences-1.png)

Verá algo similar cuando abra el [!UICONTROL Tareas y problemas] configuración.

![[!UICONTROL Preferencias de tareas y problemas] en [!UICONTROL Configuración]](assets/admin-fund-task-issue-preferences-2.png)

Sin embargo, es posible que no todos los grupos de [!DNL Workfront] necesita las mismas preferencias de proyecto, tarea y problema. Por ejemplo, el grupo de marketing quiere que el nuevo estado del proyecto sea Planning, mientras que el grupo del administrador del proyecto prefiere el estado Solicitud .

[!DNL Workfront] permite a los administradores de grupos ajustar determinadas preferencias de proyecto, tarea y problema de sus grupos. Las preferencias que se pueden ajustar están determinadas por la variable [!DNL Workfront] administrador del sistema mediante las conmutaciones de bloqueo/desbloqueo.

Para empezar, vaya a la [!UICONTROL Configuración] área:

1. Select **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expandir **[!UICONTROL Preferencias de proyecto]** en el menú de la izquierda.
1. Select **[!UICONTROL Proyectos]** o **[!UICONTROL Tareas y problemas]**, según la configuración que desee modificar.

Bloquee una preferencia para evitar que los administradores del grupo ajusten esa configuración para su grupo.

![Mensaje de preferencias bloqueado](assets/admin-fund-preferences-locked-3.png)

Desbloquee la preferencia para que esté disponible para que los administradores de grupos la personalicen.

![Mensaje de preferencia desbloqueado](assets/admin-fund-preferences-unlocked-4.png)

Algunos ajustes no se pueden desbloquear y siguen siendo ajustes globales del sistema.

![Mensaje de preferencias bloqueado](assets/admin-fund-preferences-always-locked-5.png)

### Definir preferencias de grupo y subgrupo

Para cualquier configuración desbloqueada por el administrador del sistema, los administradores del grupo pueden realizar ajustes para los grupos que administran y para cualquier subgrupo anidado en esos grupos. Además, los administradores de grupos pueden controlar qué configuración pueden modificar los administradores de subgrupos.

1. Select **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Haga clic en **[!DNL Groups]** en el menú de la izquierda.
1. Haga clic en el nombre del grupo o subgrupo para abrirlo.
1. Select **[!UICONTROL Preferencias de proyecto]** o **[!UICONTROL Preferencias de Tareas y problemas]** en el menú de la izquierda.
1. Realice los cambios necesarios para cada una de las preferencias que se han desbloqueado.
1. Select **[!UICONTROL Guardar]**.

![[!UICONTROL Estado del proyecto] sección [!UICONTROL Grupo] página](assets/admin-fund-group-preferences.png)

Si su organización no utiliza administradores de grupo, el administrador del sistema puede administrar la configuración de preferencias de los distintos grupos.

<!---
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
--->
