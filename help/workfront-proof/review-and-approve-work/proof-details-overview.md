---
title: Explicación de los detalles de la prueba
description: Profundizar en los detalles detrás de una prueba en [!DNL  Workfront] a través del panel de resumen y [!UICONTROL Detalles del documento] página.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
kt: 10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 0%

---

# Explicación de los detalles de la prueba

## Ver detalles de prueba

Como administrador de pruebas o propietario, puede profundizar en los detalles detrás de una prueba a través del panel de resumen y el [!UICONTROL Detalles del documento] página. Comience por encontrar la prueba en el [!UICONTROL Documentos] de un proyecto, tarea o problema.

### Panel de resumen

El panel de resumen ofrece información general de alto nivel sobre los detalles básicos de la prueba. Utilice el icono para expandir el panel cuando lo necesite y contraerlo cuando no lo necesite. Incluso puede pasar el ratón sobre la miniatura de la prueba para abrirla o descargarla.

![Una imagen del [!UICONTROL Documentos] de un proyecto con una prueba seleccionada y el panel de resumen ampliado. Tanto el icono del panel de resumen como el panel de resumen están resaltados.](assets/document-summary.png)

Nota: La variable [!UICONTROL Aprobaciones] en el panel de resumen está para **documento** aprobaciones y **no es** está vinculado al proceso de revisión y aprobación de la prueba del que ha estado aprendiendo en este curso. Los dos procesos están separados en [!DNL Workfront].

### [!UICONTROL Detalles del documento]

Si necesita más información sobre la prueba, la variable [!UICONTROL Detalles del documento] El vínculo le lleva a la &quot;página&quot; de la prueba en [!DNL Workfront].

![Una imagen de la página de la prueba en [!DNL  Workfront].](assets/document-details.png)

Es importante tener en cuenta que la capacidad de ver información relacionada con el proceso de pruebas depende de los permisos de pruebas en [!DNL Workfront].

Desde la página de la prueba, puede acceder a estas secciones desde el menú del panel izquierdo:

* **Actualizaciones —** Los comentarios realizados en el visor de pruebas aparecen aquí, con la etiqueta &quot;comentario de prueba&quot;. También puede realizar comentarios sobre el archivo, como hace comentarios sobre una tarea o proyecto (estos comentarios no aparecen en el visor de pruebas).
* **Aprobaciones —** Esta sección es para aprobaciones de documentos, no para pruebas de aprobaciones. Los dos tipos de aprobaciones son procesos independientes en [!DNL Workfront] y no se vinculan entre sí. Si utiliza flujos de trabajo de prueba para sus revisiones y aprobaciones, no utiliza esta sección.
* **Todas las versiones —** Rastree y administre el historial de versiones de la prueba. Puede que le resulte más fácil acceder a esta información en el panel de resumen del [!UICONTROL Documentos] lista.
* **Forms personalizado —** Los formularios personalizados se utilizan en pruebas para capturar información específica de la organización. Esta información se puede pasar con el archivo a sistemas de almacenamiento de documentos integrados, como [!DNL Workfront] DAM o [!DNL Adobe’s] AEM. Los formularios personalizados los configura el [!DNL Workfront] administrador del sistema o administrador del grupo. Hable con su equipo o con sus administradores para saber si va a utilizar formularios personalizados en pruebas.
* **Flujo de trabajo de prueba —** Administre o modifique el flujo de trabajo asignado a la prueba. Puede abrir esta ventana utilizando la variable [!UICONTROL Flujo de trabajo de prueba] en la prueba de [!UICONTROL Documentos] lista, también. Aprenda a realizar cambios en el flujo de trabajo con el vídeo Editar un flujo de trabajo de prueba .

Veamos más de cerca dos de las secciones: [!UICONTROL Configuración del visor de pruebas] y [!UICONTROL Actividad de prueba].

### [!UICONTROL Configuración del visor de corrección]

Esta configuración le ayuda a controlar el acceso a la propia prueba.

![Una imagen del [!UICONTROL Configuración del visor de pruebas] de la página de la prueba con la variable [!UICONTROL Configuración del visor de pruebas] en el menú del panel izquierdo.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Inicio de sesión obligatorio. Esta prueba no se puede compartir con usuarios invitados] —** La prueba solo se puede compartir con personas que tengan un [!DNL Workfront] licencia de prueba.
* **[!UICONTROL Requiere que las decisiones se firmen electrónicamente] —** Al compartir una prueba, esto requiere que el destinatario tenga permisos de prueba en [!DNL Workfront] y les hace &quot;firmar electrónicamente&quot; la prueba introduciendo su contraseña de prueba cuando toman una decisión de prueba. (Nota: La contraseña de prueba es diferente de la [!DNL Workfront] contraseña. La contraseña de prueba no es fácilmente accesible, por lo que la mayoría de los destinatarios no conocerán esta contraseña). [!DNL Workfront] recomienda hablar con su [!DNL Workfront] antes de usar esta función.
* **[!UICONTROL Bloquear la prueba cuando se toman todas las decisiones necesarias ]—** Esto bloquea la prueba de cualquier otro comentario, respuesta, decisión, etc., una vez que se haya tomado una decisión sobre la prueba. Esto bloquea la versión de prueba completa, no solo una fase específica del flujo de trabajo de pruebas.
* **[!UICONTROL Permitir la descarga del archivo original] —** Los destinatarios de la prueba pueden descargar el archivo de origen original de la prueba desde el visor de pruebas (la opción está en el menú del panel derecho).
* **[!UICONTROL Permitir el uso compartido de pruebas mediante una URL pública o código incrustado] —** Los destinatarios de la prueba pueden compartir un vínculo de prueba accesible al público con cualquier persona.
* **[!UICONTROL Permitir la suscripción a la prueba a través de una URL pública o código incrustado] —** Cualquier persona a la que se envíe la URL pública puede agregarse a la prueba con su dirección de correo electrónico y su nombre (si no es un usuario de prueba) o su dirección de correo electrónico y contraseña de prueba (si es un usuario de prueba). (Nota: La contraseña de prueba no es la misma que una [!DNL Workfront] contraseña).

Esta misma configuración se puede establecer cuando la prueba se carga en la variable [!UICONTROL Configuración de prueba] , en la parte inferior de la ventana de carga.

![Una imagen del [!UICONTROL Configuración de prueba] en la parte inferior de la ventana de carga.](assets/proof-settings-on-upload-page.png)

### [!UICONTROL Actividad de prueba]

Esta página realiza un seguimiento de toda la actividad que se ha producido en la prueba, además de los mensajes de correo electrónico que se han enviado con respecto a esta prueba.

![Una imagen del [!UICONTROL Actividad de prueba] de la página de la prueba con el [!UICONTROL Actividad de prueba] en el menú del panel izquierdo.](assets/proofing-activity-in-details.png)

La variable [!UICONTROL Actividad] marcas de tiempo de sección cuando se realizaron comentarios y decisiones, además de quién los hizo. También realiza un seguimiento de las fases de prueba del flujo de trabajo iniciadas, cuándo un destinatario abrió una prueba por primera vez y otra información que un administrador de pruebas o propietario desea conocer. Estos detalles pueden resultar útiles cuando intenta averiguar cosas como por ejemplo por qué una etapa de flujo de trabajo de prueba nunca se inició, por ejemplo.

La variable [!UICONTROL Mensajes] marcas de hora de sección cuando se enviaron alertas de correo electrónico y mensajes a los destinatarios, quiénes los enviaron y el contenido del mensaje. Esto puede resultar útil a la hora de solucionar problemas si alguien dice que no ha recibido un correo electrónico sobre una prueba. Puede comprobar si y cuándo se ha enviado un correo electrónico.

[!DNL Workfront] recomienda que el administrador de pruebas y el propietario de la prueba se familiaricen con la información de estas dos secciones. Cuando combina esta información con la comprensión de cómo leer la variable [!UICONTROL SOCD] barra de progreso, puede comprender y administrar realmente sus pruebas, independientemente de dónde se encuentren en el flujo de trabajo de pruebas.

Una vez que haya terminado de trabajar en [!UICONTROL Detalles del documento] , utilice la ruta de exploración para volver al [!UICONTROL Documentos] del proyecto, la tarea o el problema al que se adjunta la prueba.

![Imagen de la ruta de exploración en el encabezado.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
