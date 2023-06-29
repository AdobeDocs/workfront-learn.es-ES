---
title: Configurar notificaciones de eventos
description: Obtenga información sobre cómo controlar qué notificaciones por correo electrónico y en la aplicación reciben los usuarios mediante la administración de notificaciones de eventos.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '621'
ht-degree: 100%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# Configurar notificaciones de eventos

>[!NOTE]
>
>Debido a una implementación por fases, la funcionalidad que permite a los administradores de sistemas y grupos administrar las notificaciones de eventos no está disponible temporalmente para algunos clientes de [!DNL Workfront]. Siga este artículo para conocer las actualizaciones sobre la versión: desbloquee la configuración de las notificaciones de eventos para grupos.

Los administradores del sistema determinan qué notificaciones deben recibir los usuarios de [!DNL Workfront].

Ventana de ![[!UICONTROL Notificaciones por correo electrónico] en el área [!UICONTROL Configuración]](assets/admin-fund-notifications-1.png)

La lista [!UICONTROL Notificaciones de eventos] se agrupa por tipo. Para cada notificación de eventos enumerada, verá cinco fragmentos de información:

* **[!UICONTROL Activo]:** la columna [!UICONTROL Activo] permite activar o desactivar una notificación a nivel de todo el sistema.
* **[!UICONTROL Nombre]:** este es el nombre de la notificación dentro de [!DNL Workfront].
* **[!UICONTROL Descripción]:** en la descripción se explica brevemente qué medidas se han adoptado para activar una notificación o se deben adoptar en respuesta a la recepción de la notificación.
* **[!UICONTROL Asunto del correo electrónico]:** qué se mostrará al usuario en la línea de asunto cuando el correo electrónico se envíe a los usuarios.
* **[!UICONTROL Acceso a grupos]:** desbloquee las notificaciones para que los administradores del grupo puedan administrarlas.

## Activar notificaciones

Para administrar las notificaciones a nivel de sistema global, asegúrese de que la barra de búsqueda indica [!UICONTROL Notificaciones de eventos del sistema].

Active una notificación específica para que esté disponible para todos los usuarios haciendo clic en el botón de alternancia para que se muestre el color azul. Si el color azul está oculto, la notificación está desactivada.

Columna![[!UICONTROL Activo] en la página [!UICONTROL Notificaciones por correo electrónico]](assets/admin-fund-notifications-2.png)

Una vez que se activa una notificación de eventos, los mensajes se envían instantáneamente cuando se produce el evento.

## Permitir el control al administrador de grupos

Los administradores del sistema pueden conceder permiso a los administradores de grupos para personalizar aún más la lista de notificaciones en función de cómo funcionan sus grupos y subgrupos y de cuáles son sus flujos de trabajo.

Columna![[!UICONTROL Acceso a grupos] en la página [!UICONTROL Notificaciones por correo electrónico] ](assets/ganotifications_01.png)

Para que los administradores de grupo puedan administrar las notificaciones de sus grupos y subgrupos, es necesario desbloquear las notificaciones a nivel de sistema.

* Vaya a la pestaña Notificación de eventos de la página Notificaciones de correo electrónico.

* Asegúrese de que la barra de búsqueda indica Notificaciones de eventos del sistema.

* Desbloquee una sola notificación para todos los administradores de grupos haciendo clic en el botón de alternancia de la columna Acceso a grupos para que aparezca el color azul.

* Desbloquee varias notificaciones a la vez marcando la casilla a la izquierda de cada notificación y haciendo clic en el icono de desbloqueo en la barra de herramientas situada encima de la lista.

Columna ![[!UICONTROL Acceso a grupos] en la página [!UICONTROL Notificaciones por correo electrónico]](assets/ganotifications_02.png)

Para bloquear una notificación desbloqueada, haga clic en el botón de alternancia para que aparezca el gris. Para bloquear varias notificaciones al mismo tiempo, seleccione las casillas de verificación y haga clic en el icono de desbloqueo de la barra de herramientas.

Columna![[!UICONTROL Acceso a grupos] en la página [!UICONTROL Notificaciones por correo electrónico] ](assets/ganotifications_03.png)

Las notificaciones desbloqueadas aparecen para los administradores de grupos de nivel superior a fin de determinar si se necesita dicha notificación para sus grupos y subgrupos. Los subgrupos heredan las configuraciones de notificación de su grupo principal superior. ﻿


## Administrar notificaciones de grupo

Una vez que el administrador del sistema ha desbloqueado las opciones de notificación, los administradores del grupo pueden administrar las notificaciones de un grupo desde la página de grupo individual haciendo clic en Notificaciones de eventos en el menú del panel izquierdo. A continuación, puede activar o desactivar las opciones de notificación.

Columna![[!UICONTROL Acceso a grupos] en la página [!UICONTROL Notificaciones por correo electrónico]](assets/managegroupnotifications_01.png)

Si es necesario, los administradores del sistema pueden administrar las notificaciones de un grupo desde la página Notificaciones, al escribir el nombre del grupo en la barra de búsqueda de la parte superior de la ventana.

Columna ![[!UICONTROL Acceso a grupos] en la página [!UICONTROL Notificaciones por correo electrónico] ](assets/managegroupnotifications_02.png)

## Consejos profesionales

Hay algunas recomendaciones de notificaciones de [!DNL Workfront] a disposición de los usuarios.

Para la mayoría de los usuarios:

* [!UICONTROL Se completa una de mis tareas predecesoras]
* [!UICONTROL Alguien me incluye en una actualización dirigida]
* [!UICONTROL Alguien comenta sobre mi elemento de trabajo]
* [!UICONTROL Cambio de fecha límite de una tarea a la que estoy asignado]


Específicamente para los administradores del proyecto:

* [!UICONTROL Se activa un proyecto en el que participo]
* [!UICONTROL Se retrasa un proyecto de mi propiedad]
* [!UICONTROL Se agrega un problema a mi proyecto]
* [!UICONTROL La tarea de hito se ha completado en un proyecto que tengo]

<!---
learn more URLs
--->
