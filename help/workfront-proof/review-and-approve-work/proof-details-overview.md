---
title: Explicación de los detalles de la prueba
description: Profundizar en los detalles detrás de una prueba en  [!DNL  Workfront]  a través del panel de resumen y la página [!UICONTROL Detalles del documento].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
jira: KT-10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 100%

---

# Explicación de los detalles de la prueba

## Ver detalles de la prueba

Como administrador de pruebas o propietario, puede profundizar en los detalles detrás de una prueba a través del panel de resumen y la página [!UICONTROL Detalles del documento]. Comience por encontrar la prueba en la sección [!UICONTROL Documentos] de un proyecto, tarea o problema.

### Panel de resumen

El panel de resumen ofrece información general de alto nivel sobre los detalles básicos de la prueba. Utilice el icono para expandir el panel cuando lo necesite y contraerlo cuando no lo necesite. Incluso puede pasar el ratón sobre la miniatura de la prueba para abrirla o descargarla.

![Una imagen de la sección [!UICONTROL Documentos] de un proyecto con una prueba seleccionada y el panel de resumen ampliado. Tanto el icono del panel de resumen como el panel de resumen están resaltados.](assets/document-summary.png)

Nota: La sección [!UICONTROL Aprobaciones] en el panel de resumen es para las aprobaciones del **documento** y **no está** vinculado al proceso de revisión y aprobación de la prueba del que ha estado aprendiendo en este curso. Los dos procesos están separados en [!DNL Workfront].

### [!UICONTROL Detalles del documento]

Si necesita más información sobre la prueba, el vínculo [!UICONTROL Detalles del documento] le lleva a la “página” de la prueba en [!DNL Workfront].

![Una imagen de la página de la prueba en [!DNL  Workfront].](assets/document-details.png)

Es importante tener en cuenta que la capacidad de ver información relacionada con el proceso de pruebas depende de los permisos de pruebas en [!DNL Workfront].

Desde la página de la prueba, puede acceder a estas secciones desde el menú del panel izquierdo:

* **Actualizaciones:** los comentarios realizados en el visualizador de pruebas aparecen aquí, con la etiqueta “comentario de prueba”. También puede realizar comentarios sobre el archivo, como hace comentarios sobre una tarea o proyecto (estos comentarios no aparecen en el visualizador de pruebas).
* **Aprobaciones:** esta sección es para aprobaciones de documentos, no para aprobaciones de pruebas. Los dos tipos de aprobaciones son procesos independientes en [!DNL Workfront] y no se vinculan entre sí. Si utiliza flujos de trabajo de prueba para sus revisiones y aprobaciones, no precisará esta sección.
* **Todas las versiones:** rastree y administre el historial de versiones de la prueba. Puede que le resulte más fácil acceder a esta información en el panel de resumen de la lista [!UICONTROL Documentos].
* **Formularios personalizados:** los formularios personalizados se utilizan en pruebas para capturar información específica de la organización. Esta información se puede pasar con el archivo a sistemas de almacenamiento de documentos integrados, como DAM en [!DNL Workfront] o [!DNL Adobe’s] AEM. Los formularios personalizados los configura el administrador del sistema o el administrador del grupo de [!DNL Workfront]. Hable con su equipo o con sus administradores para saber si va a utilizar formularios personalizados en las pruebas.
* **Flujo de trabajo de prueba:** administre o modifique el flujo de trabajo asignado a la prueba. También puede abrir esta ventana utilizando el vínculo [!UICONTROL Flujo de trabajo de prueba] en la prueba de la lista de [!UICONTROL Documentos]. Aprenda a realizar cambios en el flujo de trabajo con el vídeo Editar un flujo de trabajo de prueba.

Veamos más de cerca dos de las secciones: [!UICONTROL Configuración del visualizador de pruebas] y [!UICONTROL Actividad de pruebas].

### [!UICONTROL Configuración del visualizador de revisión]

Esta configuración le ayuda a controlar el acceso a la propia prueba.

![Una imagen de la [!UICONTROL Configuración del visualizador de pruebas] de la página de la prueba con la opción [!UICONTROL Configuración del visualizador de pruebas] en el menú del panel izquierdo.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Inicio de sesión obligatorio. Esta prueba no se puede compartir con usuarios invitados]:** la prueba solo se puede compartir con personas que tengan una licencia de prueba de [!DNL Workfront].
* **[!UICONTROL Requiere que las decisiones se firmen electrónicamente]:** al compartir una prueba, esto requiere que el destinatario tenga permisos de prueba en [!DNL Workfront] y les hace “firmar electrónicamente” la prueba con su contraseña cuando toman una decisión sobre la revisión. (Nota: La contraseña de revisión debe ser diferente de la contraseña de [!DNL Workfront]. No se puede acceder fácilmente a la contraseña de revisión, por lo que la mayoría de los destinatarios no conocen esta contraseña). [!DNL Workfront] recomienda hablar con su consultor de [!DNL Workfront] antes de usar esta función.
* **[!UICONTROL Bloquear la prueba cuando se toman todas las decisiones necesarias]:** esto bloquea la prueba de cualquier otro comentario, respuesta, decisión, etc., una vez que se haya tomado una decisión sobre la prueba. Esto bloquea la versión de prueba completa, no solo una fase específica del flujo de trabajo de revisión.
* **[!UICONTROL Permitir la descarga del archivo original]:** los destinatarios de la prueba pueden descargar el archivo de origen original de la prueba desde el visualizador de pruebas (la opción está en el menú del panel derecho).
* **[!UICONTROL Permitir el uso compartido de pruebas mediante una URL pública o código incrustado]:** los destinatarios de la prueba pueden compartir un vínculo de prueba accesible al público con cualquier persona.
* **[!UICONTROL Permitir la suscripción a la prueba a través de una URL pública o código incrustado]:** cualquier persona a la que se le envíe la URL pública puede agregarse a la prueba con su dirección de correo electrónico y su nombre (si no es un usuario de revisión) o su dirección de correo electrónico y contraseña de revisión (si es un usuario de revisión). (Nota: La contraseña de la revisión no es la misma que la contraseña de [!DNL Workfront]).

Esta misma configuración se puede establecer cuando la prueba se carga en la sección [!UICONTROL Configuración de prueba], en la parte inferior de la ventana de carga.

![Una imagen de la sección [!UICONTROL Configuración de prueba] en la parte inferior de la ventana de carga.](assets/proof-settings-on-upload-page.png)

### [!UICONTROL Actividad de revisión]

Esta página sigue toda la actividad que se ha producido en la prueba, además de los mensajes de correo electrónico que se enviaron en relación con ella.

![Una imagen de la sección [!UICONTROL Actividad de revisión] de la página de la prueba con la opción [!UICONTROL Actividad de revisión] resaltada en el menú del panel izquierdo.](assets/proofing-activity-in-details.png)

La sección [!UICONTROL Actividad] registra cuándo se hicieron los comentarios y se tomaron las decisiones, además de quién fue. También rastrea cuándo se iniciaron las fases del flujo de trabajo de revisión, cuándo un destinatario abrió una prueba por primera vez y otra información que un administrador o propietario de pruebas querrá saber. Estos detalles pueden resultar útiles cuando intenta averiguar cosas como, por ejemplo, por qué una etapa de flujo de trabajo de revisión nunca se inició.

La sección [!UICONTROL Mensajes] registra el momento en que se enviaron alertas y mensajes de correo electrónico a los destinatarios, quién los mandó y el contenido. Esto puede resultar útil a la hora de solucionar problemas si alguien dice que no ha recibido un correo electrónico acerca de una prueba. Puede consultar si se ha enviado un correo electrónico y cuándo.

[!DNL Workfront] recomienda que el administrador y el propietario de la prueba se familiaricen con la información de estas dos secciones. Si combina esta información con la comprensión de cómo leer la barra de progreso de [!UICONTROL SOCD], podrá entender y administrar de verdad sus pruebas, sin importar en qué punto del flujo de trabajo de revisión se encuentren.

Cuando haya terminado de trabajar en la sección [!UICONTROL Detalles del documento], use la ruta de exploración para volver a la sección [!UICONTROL Documentos] del proyecto, la tarea o el problema asociados a la prueba.

![Una imagen de la ruta de exploración en el encabezado.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
