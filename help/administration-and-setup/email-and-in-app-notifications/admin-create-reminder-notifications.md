---
title: Configurar notificaciones de recordatorio
description: Obtenga información sobre cómo configurar notificaciones de recordatorio específicas de objetos para informar a los usuarios de cuándo el trabajo debe realizarse pronto o ha vencido.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: setupremindnote.png
jira: KT-10091
exl-id: f1ba58d7-3226-4c62-8aa4-40f88495b833
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 100%

---

<!--
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
-->

# Configurar notificaciones de recordatorio

Los administradores del sistema crean las notificaciones de recordatorio en el área [!UICONTROL Configuración]. Luego se pueden adjuntar y utilizar por los propietarios de proyectos, tareas y problemas como recordatorios para saber cuándo el trabajo debe realizarse pronto o ha vencido.

Los recordatorios son específicos del objeto y deben adjuntarse manualmente al elemento de trabajo correspondiente para poder enviar la notificación.

**Creación de una notificación de recordatorio**

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Haga clic en la sección **[!UICONTROL Correo electrónico]**.
1. Haga clic en la sección **[!UICONTROL Notificaciones]**.
1. Haga clic en la pestaña **[!UICONTROL Nuevo recordatorio]**.
1. Haga clic en el botón **[!UICONTROL +Notificación de nuevo recordatorio]**.
1. Seleccione el objeto deseado para el menú desplegable.
1. Rellene la información requerida.
1. Haga clic en **[!UICONTROL Guardar]**.

Ventana ![[!UICONTROL Nueva notificación de recordatorio] ](assets/admin-fund-reminder-notification-1.png)

Al configurar el recordatorio, hay que tener en cuenta algunos aspectos:

* **[!UICONTROL Nombre de notificación del recordatorio]:** este es el nombre que verán los administradores del proyecto cuando adjunten un recordatorio a un objeto. Asegúrese de que el nombre sea corto, pero descriptivo.
* **[!UICONTROL Período de calificación]:** cantidad de horas, días, semanas o meses antes o después de la fecha seleccionada en la sección Temporización.
* **[!UICONTROL Temporización]:** seleccione si el recordatorio debe enviarse antes o después de las fechas de inicio/finalización planificadas, previstas o reales del objeto. Las opciones para las hojas de horas están relacionadas con la fecha de inicio, la fecha de finalización o la fecha de la última actualización.
* **[!UICONTROL Criterios]:** especifique los criterios para calificar el recordatorio que se va a enviar. Las opciones varían según el recordatorio específico del objeto.
* **[!UICONTROL Destinatarios]:** seleccione a quién se debe enviar el recordatorio. Las opciones de las partes interesadas varían según el tipo de objeto seleccionado para el recordatorio.

Una vez establecida y guardada la configuración del recordatorio, los propietarios de objetos pueden utilizar la notificación del recordatorio en [!DNL Workfront].

## Personalización del correo electrónico

Las notificaciones de recordatorio utilizan un formato de correo electrónico y un mensaje predeterminados. Si desea personalizar el correo electrónico, puede crear una plantilla.

<!--
paragraph above needs a hyperlink to an article
-->

![Ventana de Nueva plantilla de correo electrónico](assets/admin-fund-email-customization.png)

<!--
learn more URLs
-->
