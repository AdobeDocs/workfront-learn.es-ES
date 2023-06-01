---
title: Funciones de prueba y alertas de correo electrónico
description: Obtenga información sobre cómo habilitar las funciones de prueba y las alertas de correo electrónico adecuadas para que los destinatarios de prueba tengan acceso a las pruebas y visibilidad del trabajo realizado en [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
kt: 10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: 65bd26fefb280d12ec44a4923f6d96ac8d88d6fb
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Funciones de prueba y alertas de correo electrónico

Las funciones de prueba y las alertas de correo electrónico ayudan a dirigir el flujo de trabajo de prueba, asegurándose de que los destinatarios tengan el acceso correcto a las pruebas y tengan visibilidad del trabajo realizado.

Revisemos la terminología básica de la prueba:

* **Función de prueba —** Define lo que un usuario puede hacer con una prueba (por ejemplo, comentar, marcar, aprobar, etc.).
* **Alerta de correo electrónico —** Correos electrónicos enviados a personas en el flujo de trabajo de prueba cuando hay actividad en la prueba.

![Una imagen de la [!UICONTROL Nueva revisión] ventana con el [!UICONTROL Función de prueba] y [!UICONTROL Alertas de correo electrónico] columnas resaltadas.](assets/proof-roles-and-email-alerts.png)

El administrador del sistema de pruebas puede establecer funciones de prueba y alertas de correo electrónico predeterminadas para los usuarios de prueba de su organización. Además, esta información se puede incorporar en plantillas de flujo de trabajo de prueba (también conocidas como plantillas de flujo de trabajo automatizadas).

Sin embargo, puede haber ocasiones en que necesite configurar esta información manualmente al cargar una prueba.

[!DNL Workfront] ofrece las siguientes recomendaciones generales al asignar funciones de prueba a destinatarios de prueba:

* **Revisor y aprobador —** Estos usuarios pueden realizar comentarios en las pruebas y tomar una decisión (como aprobada o rechazada) al respecto. Utilice esta función de prueba para las partes interesadas internas y externas clave en el proceso de revisión.
* **Revisor —** Algunas personas del flujo de trabajo de prueba solo necesitan realizar comentarios; esta función es ideal para ellas. La función de revisor también se puede asignar a [!DNL Workfront] usuarios que principalmente cargan pruebas o actúan como propietarios de pruebas, pero que de lo contrario no forman parte del proceso de revisión.
* **Solo lectura —** Ideal para destinatarios que solo necesitan ver la prueba. [!UICONTROL Solo lectura] proporciona acceso de visualización y no permite comentarios.

[!DNL Workfront] ofrece las siguientes recomendaciones generales al asignar alertas de correo electrónico a destinatarios de prueba:

* **Decisión final —** Esto envía un correo electrónico cuando la última persona toma una decisión sobre la prueba. Asigne esto a la persona que supervisa el flujo de trabajo de prueba. Puede ser un administrador de pruebas, un propietario de pruebas, un creador de pruebas, un administrador de proyectos u otro [!DNL Workfront] usuario. [!DNL Workfront] recomienda esta alerta cuando se utiliza un flujo de trabajo básico, para que la persona que supervisa la prueba sepa que se han tomado todas las decisiones.
* **Decisiones —** Esto envía alertas a medida que cada parte interesada del flujo de trabajo de prueba toma una decisión sobre la prueba. Esta opción es mejor cuando se utiliza un flujo de trabajo automatizado, con varias decisiones. Asigne a la persona que supervisa el flujo de trabajo de prueba. Puede ser un administrador de pruebas, un propietario de pruebas, un creador de pruebas, un administrador de proyectos u otro [!DNL Workfront] usuario.
* **Desactivado —** Utilícelo para que los usuarios de pruebas invitados limiten el número de correos electrónicos que reciben sobre la prueba. Los destinatarios siguen recibiendo notificaciones sobre nuevas pruebas, nuevas versiones y pruebas tardías, además de [!DNL Workfront] los usuarios reciben mensajes directos realizados en un comentario de prueba mediante @username y destinatarios invitados con @emailaddress.

## Tu turno

1. Inicie sesión en Workfront y cree usuarios que utilicen pruebas que no haya creado anteriormente. Establezca el perfil de permisos de prueba en su configuración de usuario según la función que la persona desempeñará en los flujos de trabajo de prueba.
1. Para los usuarios que ya se han creado, edite su configuración para ajustar la selección del perfil de permisos de prueba, si es necesario.
1. Acceda al área de configuraciones de revisión y vaya a la pestaña Usuarios. Compruebe la configuración personal de los usuarios: idioma, zona horaria, formato de fecha, función de prueba predeterminada y alerta de correo electrónico predeterminada. Esto es importante si estos usuarios se crearon antes de que se establecieran los valores predeterminados del sistema global.

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
