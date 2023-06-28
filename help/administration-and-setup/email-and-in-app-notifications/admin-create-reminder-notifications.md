---
title: Configurar notificaciones de recordatorio
description: Obtenga información sobre cómo configurar notificaciones de recordatorio específicas del objeto para que los usuarios sepan cuándo vence el trabajo pronto o con retraso.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: setupremindnote.png
jira: KT-10091
exl-id: f1ba58d7-3226-4c62-8aa4-40f88495b833
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

# Configuración de notificaciones de recordatorio

Los administradores del sistema crean las notificaciones de recordatorio en el [!UICONTROL Configurar] área. A continuación, los propietarios de proyecto, tarea y problema pueden adjuntarlos y utilizarlos como recordatorios de cuándo vence el trabajo pronto o ha vencido.

Los recordatorios son específicos del objeto y deben adjuntarse manualmente al elemento de trabajo correspondiente para poder enviar la notificación.

**Crear una notificación de recordatorio**

1. Clic **[!UICONTROL Configurar]** en el **[!UICONTROL Menú principal]**.
1. Haga clic en **[!UICONTROL Correo electrónico]** sección.
1. Haga clic en **[!UICONTROL Notificaciones]** sección.
1. Haga clic en **[!UICONTROL Nuevo recordatorio]** pestaña.
1. Haga clic en **[!UICONTROL +Nueva notificación de recordatorio]** botón.
1. Seleccione el objeto que desee en el menú desplegable.
1. Rellene la información requerida.
1. Haga clic en **[!UICONTROL Guardar]**.

![[!UICONTROL Nueva notificación de recordatorio] ventana](assets/admin-fund-reminder-notification-1.png)

Al configurar el recordatorio, hay que tener en cuenta lo siguiente:

* **[!UICONTROL Nombre de notificación de recordatorio] —** Nombre que verán los jefes de proyecto cuando adjunten un aviso a un objeto. Asegúrese de que el nombre sea sucinto pero descriptivo.
* **[!UICONTROL Período de calificación] —** Número de horas, días, semanas o meses antes o después de la fecha seleccionada en la sección Intervalo.
* **[!UICONTROL Programación] —** Seleccione si el recordatorio debe enviarse antes o después de las fechas de inicio/finalización planificadas, proyectadas o reales del objeto. Las opciones para las hojas de horas están relacionadas con la fecha de inicio, la fecha de finalización o la fecha de la última actualización.
* **[!UICONTROL Criterios] —** Especifique los criterios para calificar el recordatorio que se va a enviar. Las opciones varían según el recordatorio específico del objeto.
* **[!UICONTROL Destinatarios] —** Seleccione a quién debe enviarse el recordatorio. Las opciones de la parte interesada varían según el tipo de objeto seleccionado para el recordatorio.

Una vez establecida y guardada la configuración del recordatorio, la notificación de recordatorio está disponible para que los propietarios de objetos la utilicen en [!DNL Workfront].

## Personalización de correo electrónico

Las notificaciones de recordatorio utilizan un formato de correo electrónico y un mensaje predeterminados. Si desea personalizar el correo electrónico, puede crear una plantilla.

<!---
paragraph above needs a hyperlink to an article
--->

![Ventana Nueva plantilla de correo electrónico](assets/admin-fund-email-customization.png)

<!---
learn more URLs
--->
