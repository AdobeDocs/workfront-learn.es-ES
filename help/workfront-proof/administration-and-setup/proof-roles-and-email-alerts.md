---
title: Funciones de prueba y alertas de correo electrónico
description: Obtenga información sobre cómo habilitar funciones de prueba y alertas de correo electrónico adecuadas para que los destinatarios de las pruebas tengan acceso a estas y puedan ver el trabajo que se está realizando en  [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
jira: KT-10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 77%

---

# Funciones de prueba y alertas de correo electrónico

Las funciones de prueba y las alertas de correo electrónico dirigen el flujo de trabajo de prueba, lo que garantiza que los destinatarios puedan acceder a las pruebas y ver el trabajo que se está realizando.

Revisemos la terminología básica de la prueba:

* **Función de la prueba:** define lo que un usuario puede hacer con una prueba (por ejemplo, comentar, marcar, aprobar, etc.).
* **Alerta de correo electrónico —** Correos electrónicos enviados a personas en el flujo de trabajo de prueba cuando hay actividad en la prueba.

![Una imagen de la ventana [!UICONTROL Nueva prueba] con las columnas [!UICONTROL Función de prueba] y [!UICONTROL Alertas por correo electrónico] resaltadas.](assets/proof-roles-and-email-alerts.png)

El administrador del sistema de pruebas puede establecer funciones de prueba y alertas de correo electrónico predeterminadas para los usuarios de prueba de su organización. Además, esta información se puede incorporar en las plantillas de flujo de trabajo de prueba (también conocidas como plantillas de flujo de trabajo automatizadas).

Sin embargo, puede haber ocasiones en las que necesite configurar esta información manualmente al cargar una prueba.

[!DNL Workfront] ofrece estas recomendaciones generales al asignar funciones de prueba a destinatarios de pruebas:

* **Revisor y aprobador:** estos usuarios pueden comentar las pruebas y tomar una decisión (por ejemplo, aprobar o rechazar). Utilice esta función de prueba para las principales partes interesadas internas y externas en el proceso de revisión.
* **Revisor:** algunas personas en el flujo de trabajo de prueba solo necesitan hacer comentarios; esta función es ideal para ellas. La función de revisor también se puede asignar a [!DNL Workfront] usuarios que principalmente cargan pruebas o actúan como propietarios de pruebas, pero que de lo contrario no forman parte del proceso de revisión.
* **Solo lectura:** ideal para los destinatarios que solo necesitan ver la prueba. [!UICONTROL Solo lectura] proporciona acceso de visualización y no permite comentarios.

[!DNL Workfront] ofrece estas recomendaciones generales al asignar alertas de correo electrónico a los destinatarios de pruebas:

* **Decisión final:** esto envía un correo electrónico cuando la última persona decide sobre la prueba. Asigne esto a la persona que monitoriza el flujo de trabajo de pruebas. Podría ser un administrador, un propietario o un creador de pruebas, o bien un administrador de proyectos u otro usuario de [!DNL Workfront]. [!DNL Workfront] recomienda esta alerta cuando se utiliza un flujo de trabajo básico, de modo que la persona que supervisa la prueba sepa que se han tomado todas las decisiones.
* **Decisiones:** esto envía alertas, ya que cada parte interesada del flujo de trabajo de revisión toma una decisión sobre la prueba. Esta opción es mejor cuando se utiliza un flujo de trabajo automatizado con varias decisiones. Asígnela a la persona que monitoriza el flujo de trabajo de prueba. Podría ser un administrador, un propietario o un creador de pruebas, o bien un administrador de proyectos u otro usuario de [!DNL Workfront].
* **Deshabilitado:** utilice esto para los usuarios de pruebas invitados para limitar el número de correos electrónicos que reciben. A los destinatarios se les siguen notificando de las pruebas y versiones nuevas y las pruebas tardías. Además, los usuarios de [!DNL Workfront] reciben mensajes directos con comentarios utilizando @username y los destinatarios invitados con @emailaddress.

## Su turno

1. Inicie sesión en Workfront y cree usuarios que utilicen pruebas que no haya creado anteriormente. Establezca el perfil de permisos de prueba en la configuración de usuario según la función que desempeñará la persona en los flujos de trabajo de prueba.
1. Para los usuarios que ya se han creado, edite su configuración para ajustar la selección del perfil de permisos de prueba, si es necesario.
1. Acceda al área de configuración de revisión y vaya a la pestaña Usuarios. Compruebe la configuración personal de los usuarios: idioma, zona horaria, formato de fecha, función de prueba predeterminada y alerta de correo electrónico predeterminada. Esto es importante si estos usuarios se crearon antes de que se establecieran los valores predeterminados del sistema global.

<!--
Download the proof role and email alert guides to have on hand as you start uploading proofs and assigning proof recipients.
-->

<!--
## Learn more
* Notifications for proof comments and decisions
-->

<!--
## Guides
* Proof roles
* Email alerts
-->
