---
title: Configuración de notificaciones de eventos
description: Obtenga información sobre cómo controlar qué notificaciones de correo electrónico y en la aplicación reciben los usuarios administrando notificaciones de eventos.
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
>Debido a un despliegue gradual, la funcionalidad que permite a los administradores de sistemas y grupos administrar las notificaciones de eventos no está disponible temporalmente para algunos [!DNL Workfront] clientes. Consulte este artículo para obtener actualizaciones sobre la versión: Desbloquear la configuración de notificaciones de eventos para grupos.

Los administradores del sistema determinan qué notificaciones deben recibir los usuarios mediante [!DNL Workfront].

![[!UICONTROL Notificaciones por correo electrónico] ventana en el [!UICONTROL Configurar] área](assets/admin-fund-notifications-1.png)

El [!UICONTROL Notificaciones de eventos] La lista está agrupada por tipo. Para cada notificación de evento enumerada, verá cinco fragmentos de información:

* **[!UICONTROL Activo] —** El [!UICONTROL Activo] permite activar o desactivar una notificación en un nivel de todo el sistema.
* **[!UICONTROL Nombre] —** Este es el nombre de la notificación en [!DNL Workfront].
* **[!UICONTROL Descripción] —** La descripción proporciona una breve explicación de qué acción se ha realizado para almacenar en déclencheur una notificación o qué acción debe realizarse en respuesta a su recepción.
* **[!UICONTROL Asunto del correo electrónico] —** Lo que se mostrará al usuario en la línea de asunto cuando se envíe el correo electrónico a los usuarios.
* **[!UICONTROL Acceso grupal] —** Desbloquee las notificaciones para que los administradores de grupos puedan administrarlas.

## Activar notificaciones

Para administrar las notificaciones a nivel de sistema global, asegúrese de que la barra de búsqueda indica [!UICONTROL Notificaciones de eventos del sistema].

Active una notificación específica para que esté disponible para todos los usuarios haciendo clic en el botón de alternancia de modo que se muestre el azul. Si el azul está oculto, la notificación está desactivada.

![[!UICONTROL Activo] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/admin-fund-notifications-2.png)

Una vez activada la notificación de eventos, los mensajes se envían instantáneamente cuando se produce el evento.

## Permitir control de administrador de grupo

Los administradores del sistema pueden conceder permiso a los administradores del grupo para personalizar aún más la lista de notificaciones en función del funcionamiento de sus grupos y subgrupos y de sus flujos de trabajo.

![[!UICONTROL Acceso grupal] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/ganotifications_01.png)

Para que los administradores de grupo puedan administrar las notificaciones de sus grupos y subgrupos, es necesario desbloquear las notificaciones en el sistema.

* Vaya a la pestaña Notificación de eventos de la página Notificaciones por correo electrónico.

* Asegúrese de que la barra de búsqueda indica Notificaciones de eventos del sistema.

* Desbloquee una sola notificación para todos los administradores del grupo haciendo clic en el botón de alternancia en la columna Acceso de grupo, de modo que aparezca el azul.

* Desbloquee varias notificaciones a la vez marcando la casilla a la izquierda de cada notificación y haciendo clic en el icono de desbloqueo en la barra de herramientas situada encima de la lista.

![[!UICONTROL Acceso grupal] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/ganotifications_02.png)

Para bloquear una notificación desbloqueada, haga clic en el botón de alternancia y aparecerá el gris. Para bloquear varias notificaciones al mismo tiempo, seleccione las casillas de verificación y haga clic en el icono de desbloqueo de la barra de herramientas.

![[!UICONTROL Acceso grupal] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/ganotifications_03.png)

Las notificaciones desbloqueadas aparecen para los administradores de grupos de nivel superior a fin de determinar si se necesita dicha notificación para sus grupos y subgrupos. Los subgrupos heredan las configuraciones de notificación de su grupo principal superior. ﻿


## Administrar notificaciones de grupo

Una vez que el administrador del sistema ha desbloqueado las opciones de notificación, los administradores del grupo pueden gestionar las notificaciones de un grupo desde la página de Grupo individual, haciendo clic en Notificaciones de eventos en el menú del panel izquierdo. A continuación, puede activar o desactivar las opciones de notificación.

![[!UICONTROL Acceso grupal] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/managegroupnotifications_01.png)

Si es necesario, los administradores del sistema pueden gestionar las notificaciones de un grupo desde la página Notificaciones introduciendo el nombre del grupo en la barra de búsqueda de la parte superior de la ventana.

![[!UICONTROL Acceso grupal] columna en [!UICONTROL Notificaciones por correo electrónico] página](assets/managegroupnotifications_02.png)

## Sugerencias profesionales

Hay algunas notificaciones [!DNL Workfront] recomienda poner a disposición de los usuarios de.

Para la mayoría de los usuarios:

* [!UICONTROL Al finalizar una tarea predecesora de una de mis tareas.]
* [!UICONTROL Alguien me incluye en una actualización dirigida]
* [!UICONTROL Alguien agrega un comentario a mi elemento de trabajo]
* [!UICONTROL Cambia la fecha límite de una tarea a la que estoy asignado]


Específicamente para jefes de proyecto:

* [!UICONTROL Se activa un proyecto en el que participo]
* [!UICONTROL Se retrasa un proyecto de mi propiedad]
* [!UICONTROL Se agrega un problema a un proyecto de mi propiedad]
* [!UICONTROL Se completa una tarea de hito en un proyecto de mi propiedad]

<!---
learn more URLs
--->
