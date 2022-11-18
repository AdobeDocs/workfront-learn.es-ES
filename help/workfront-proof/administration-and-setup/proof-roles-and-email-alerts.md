---
title: Funciones de prueba y alertas de correo electrónico
description: Obtenga información sobre cómo habilitar funciones de prueba y alertas de correo electrónico adecuadas para que los destinatarios de prueba tengan acceso a pruebas y visibilidad del trabajo que se está realizando en [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
kt: 10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Funciones de prueba y alertas de correo electrónico

Las funciones de prueba y las alertas de correo electrónico ayudan a dirigir el flujo de trabajo de prueba, lo que garantiza que los destinatarios tengan el acceso correcto a las pruebas y tengan visibilidad sobre el trabajo que se está realizando.

Veamos algunos términos básicos de prueba:

* **Función de prueba —** Define lo que un usuario puede hacer con una prueba (por ejemplo, comentario, marcado, aprobación, etc.).
* **Alerta de correo electrónico —** Correos electrónicos enviados a personas en el flujo de trabajo de prueba cuando hay actividad en la prueba.

![Una imagen del [!UICONTROL Nueva prueba] con la variable [!UICONTROL Función de prueba] y [!UICONTROL Alertas de correo electrónico] columnas resaltadas.](assets/proof-roles-and-email-alerts.png)

El administrador del sistema de pruebas puede establecer funciones de prueba predeterminadas y alertas de correo electrónico para los usuarios de prueba de la organización. Además, esta información se puede incorporar en plantillas de flujo de trabajo de prueba (también conocidas como plantillas de flujo de trabajo automatizadas).

Sin embargo, puede haber ocasiones en las que necesite configurar esta información manualmente al cargar una prueba.

[!DNL Workfront] ofrece estas recomendaciones generales al asignar funciones de prueba a destinatarios de prueba:

* **Revisor y aprobador —** Estos usuarios pueden realizar comentarios sobre las pruebas y tomar una decisión (por ejemplo, aprobada o rechazada) sobre una prueba. Utilice esta función de prueba para las principales partes interesadas internas y externas en el proceso de revisión.
* **Revisor —** Algunas personas en el flujo de trabajo de prueba solo necesitan hacer comentarios, esta función es ideal para ellas. La función de revisor también se puede asignar a [!DNL Workfront] los usuarios que cargan pruebas principalmente o sirven como propietarios de pruebas pero que por lo demás no forman parte del proceso de pruebas.
* **Sólo lectura —** Ideal para destinatarios que solo necesitan ver la prueba. [!UICONTROL Solo lectura] proporciona acceso a la vista y no permite comentarios.

[!DNL Workfront] ofrece estas recomendaciones generales al asignar alertas de correo electrónico a destinatarios de prueba:

* **Decisión final —** Esto envía un correo electrónico cuando la última persona decide la prueba. Asigne esto a la persona que supervisa el flujo de trabajo de prueba. Podría ser un administrador de pruebas, un propietario de pruebas, un creador de pruebas, un administrador de proyectos u otro [!DNL Workfront] usuario. [!DNL Workfront] recomienda esta alerta al utilizar un flujo de trabajo básico, de modo que la persona que supervisa la prueba sepa que se han tomado todas las decisiones.
* **Decisiones —** Esto envía alertas, ya que cada responsable del flujo de trabajo de prueba toma una decisión sobre la prueba. Esta opción es mejor cuando se utiliza un flujo de trabajo automatizado con varias decisiones. Asigne a la persona que supervisa el flujo de trabajo de prueba. Podría ser un administrador de pruebas, un propietario de pruebas, un creador de pruebas, un administrador de proyectos u otro [!DNL Workfront] usuario.
* **Desactivado —** Utilice esto para los usuarios de prueba de invitado para limitar el número de correos electrónicos que reciben sobre la prueba. A los destinatarios se les siguen notificando nuevas pruebas, nuevas versiones y pruebas tardías, además de [!DNL Workfront] los usuarios reciben mensajes directos realizados en un comentario de prueba utilizando @username y los destinatarios invitados con @emailaddress.

## Su turno

1. Inicie sesión en Workfront y cree usuarios que usen pruebas que no haya creado anteriormente. Establezca el perfil de permisos de prueba en la configuración de usuario según la función que desempeñará la persona en los flujos de trabajo de prueba.
1. Para los usuarios que ya se han creado, edite su configuración para ajustar la selección de perfiles de permisos de y prueba, si es necesario.
1. Acceda al área de configuración de pruebas y vaya a la pestaña Usuarios . Compruebe la configuración personal de los usuarios: idioma, zona horaria, formato de fecha, función de prueba predeterminada y alerta de correo electrónico predeterminada. Esto es importante si estos usuarios se crearon antes de que se establecieran los valores predeterminados del sistema global (estos ajustes se tratan en la sección 1 de esta ruta de aprendizaje).

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
