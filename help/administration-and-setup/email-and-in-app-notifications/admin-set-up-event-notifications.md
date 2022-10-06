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
kt: 10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 4%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# Configuración de notificaciones de eventos

>[!NOTE]
>
>Debido a una implementación por fases, la funcionalidad que permite a los administradores de sistemas y grupos administrar las notificaciones de eventos no está disponible temporalmente para algunos [!DNL Workfront] clientes. Siga este artículo para conocer las actualizaciones sobre la versión: Desbloquee la configuración de las notificaciones de eventos para grupos.

Los administradores del sistema determinan qué notificaciones deben recibir los usuarios [!DNL Workfront].

![[!UICONTROL Notificaciones por correo electrónico] en la ventana [!UICONTROL Configuración] area](assets/admin-fund-notifications-1.png)

La variable [!UICONTROL Notificaciones de eventos] se agrupa por tipo. Para cada notificación de evento enumerada, verá cinco fragmentos de información:

* **[!UICONTROL Activo] —** La variable [!UICONTROL Activo] permite activar o desactivar una notificación a nivel de todo el sistema.
* **[!UICONTROL Nombre] —** Este es el nombre de la notificación dentro de [!DNL Workfront].
* **[!UICONTROL Descripción] —** En la descripción se explica brevemente qué medidas se han adoptado para dar déclencheur a una notificación o se deben adoptar en respuesta a la recepción de la notificación.
* **[!UICONTROL Asunto del correo electrónico] —** Qué se mostrará al usuario en la línea de asunto cuando el correo electrónico se envíe a los usuarios.
* **[!UICONTROL Acceso a grupos] —** Desbloquee las notificaciones para que los administradores del grupo puedan administrarlas.

## Activar notificaciones

Para administrar las notificaciones a nivel de sistema global, asegúrese de que la barra de búsqueda indica [!UICONTROL Notificaciones de eventos del sistema].

Active una notificación específica para que esté disponible para todos los usuarios haciendo clic en el botón de alternancia para que se muestre el color azul. Si el azul está oculto, la notificación está desactivada.

![[!UICONTROL Activo] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/admin-fund-notifications-2.png)

Una vez que se activa una notificación de evento, los mensajes se envían instantáneamente cuando se produce el evento.

## Permitir el control del administrador del grupo

Los administradores del sistema pueden conceder permiso a los administradores del grupo para personalizar aún más la lista de notificaciones en función de cómo funcionan sus grupos y subgrupos y de cuáles son sus flujos de trabajo.

![[!UICONTROL Acceso a grupos] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/ganotifications_01.png)

Para que los administradores de grupo puedan administrar las notificaciones de sus grupos y subgrupos, es necesario desbloquear las notificaciones a nivel de sistema.

* Vaya a la pestaña Notificación de eventos de la página Notificaciones de correo electrónico .

* Asegúrese de que la barra de búsqueda indica Notificaciones de eventos del sistema.

* Desbloquee una sola notificación para todos los administradores de grupos haciendo clic en el botón de alternancia de la columna Acceso a grupos para que aparezca el color azul.

* Desbloquee varias notificaciones a la vez marcando la casilla a la izquierda de cada notificación y haciendo clic en el icono de desbloqueo en la barra de herramientas situada encima de la lista.

![[!UICONTROL Acceso a grupos] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/ganotifications_02.png)

Para bloquear una notificación desbloqueada, haga clic en el botón de alternancia para que aparezca el gris. Para bloquear varias notificaciones al mismo tiempo, seleccione las casillas de verificación y haga clic en el icono de desbloqueo de la barra de herramientas.

![[!UICONTROL Acceso a grupos] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/ganotifications_03.png)

Las notificaciones desbloqueadas aparecen para los administradores de grupos de nivel superior a fin de determinar si se necesita dicha notificación para sus grupos y subgrupos. Los subgrupos heredan las configuraciones de notificación de su grupo principal superior. ﻿


## Administrar notificaciones de grupo

Una vez que el administrador del sistema ha desbloqueado las opciones de notificación, los administradores del grupo pueden administrar las notificaciones de un grupo desde la página de grupo individual haciendo clic en Notificaciones de eventos en el menú del panel izquierdo. A continuación, puede activar o desactivar las opciones de notificación.

![[!UICONTROL Acceso a grupos] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/managegroupnotifications_01.png)

Si es necesario, los administradores del sistema pueden administrar las notificaciones de un grupo desde la página Notificaciones introduciendo el nombre del grupo en la barra de búsqueda de la parte superior de la ventana.

![[!UICONTROL Acceso a grupos] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/managegroupnotifications_02.png)

## Consejos Pro

Hay algunas notificaciones [!DNL Workfront] recomienda poner a disposición de los usuarios.

Para la mayoría de los usuarios:

* [!UICONTROL Al finalizar una tarea predecesora de una de mis tareas.]
* [!UICONTROL Alguien me incluye en una actualización dirigida]
* [!UICONTROL Alguien comenta sobre mi elemento de trabajo]
* [!UICONTROL La fecha de vencimiento cambia en una tarea a la que estoy asignado]


Específicamente para los administradores de proyectos:

* [!UICONTROL Un proyecto en el que estoy se activa]
* [!UICONTROL Se retrasa un proyecto de mi propiedad]
* [!UICONTROL Se agrega un problema a un proyecto de mi propiedad]
* [!UICONTROL La tarea Milestone se completa en un proyecto que yo mismo]

<!---
learn more URLs
--->
