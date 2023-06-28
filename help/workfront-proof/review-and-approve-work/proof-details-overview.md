---
title: Comprender los detalles de prueba
description: Profundice en los detalles detrás de una prueba en [!DNL  Workfront] a través del panel de resumen y [!UICONTROL Detalles del documento] página.
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
ht-degree: 0%

---

# Comprender los detalles de prueba

## Ver detalles de revisión

Como administrador de pruebas o propietario, puede profundizar en los detalles detrás de una prueba a través del panel de resumen y la [!UICONTROL Detalles del documento] página. Comience por encontrar la prueba en la [!UICONTROL Documentos] sección de un proyecto, tarea o problema.

### Panel de resumen

El panel de resumen proporciona información general de alto nivel sobre los detalles básicos de la prueba. Utilice el icono para expandir el panel cuando lo necesite y contraerlo cuando no lo necesite. Incluso puede pasar el ratón sobre la miniatura de la prueba para abrirla o descargarla.

![Una imagen de la [!UICONTROL Documentos] de un proyecto con una prueba seleccionada y el panel de resumen expandido. Tanto el icono del panel de resumen como el panel de resumen aparecen resaltados.](assets/document-summary.png)

Nota: La [!UICONTROL Aprobaciones] de la sección del panel de resumen es para **documento** aprobaciones y **no es** vinculado al proceso de revisión y aprobación de pruebas que ha estado aprendiendo en este curso. Los dos procesos están separados en [!DNL Workfront].

### [!UICONTROL Detalles del documento]

Si necesita más información sobre la prueba, la variable [!UICONTROL Detalles del documento] le lleva a la &quot;página&quot; de la prueba en [!DNL Workfront].

![Una imagen de la página de la prueba en [!DNL  Workfront].](assets/document-details.png)

Es importante tener en cuenta que la capacidad de ver información relacionada con el proceso de revisión depende de los permisos de revisión en [!DNL Workfront].

Desde la página de la prueba, puede acceder a estas secciones desde el menú del panel izquierdo:

* **Actualizaciones —** Los comentarios realizados en el visor de pruebas se muestran aquí, con la etiqueta &quot;comentario de prueba&quot;. También puede realizar comentarios en el archivo, al igual que hace en una tarea o proyecto (estos comentarios no aparecen en el visor de pruebas).
* **Aprobaciones —** Esta sección es para aprobaciones de documentos, no para aprobaciones de revisión. Los dos tipos de aprobaciones son procesos independientes en [!DNL Workfront] y no se vinculan entre sí. Si utiliza flujos de trabajo de prueba para sus revisiones y aprobaciones, no utilizará esta sección.
* **Todas las versiones —** Rastree y administre el historial de versiones de la prueba. Puede que le resulte más fácil acceder a esta información en el panel de resumen de la [!UICONTROL Documentos] lista.
* **Forms personalizado —** Los formularios personalizados se utilizan en las pruebas para capturar información específica de la organización. Esta información se puede pasar con el archivo a sistemas integrados de almacenamiento de documentos, como [!DNL Workfront] DAM o [!DNL Adobe’s] AEM. La configuración de los formularios personalizados la realiza [!DNL Workfront] administrador del sistema o administrador del grupo. Hable con su equipo o con los administradores para saber si utilizará formularios personalizados en las pruebas.
* **Flujo de trabajo de revisión —** Administre o modifique el flujo de trabajo asignado a la prueba. Puede abrir esta ventana con el [!UICONTROL Flujo de trabajo de revisión] vínculo de la prueba en [!UICONTROL Documentos] lista, también. Aprenda a realizar cambios en el flujo de trabajo con el vídeo Editar un flujo de trabajo de prueba.

Veamos más de cerca dos de las secciones: [!UICONTROL Configuración del visor de corrección] y [!UICONTROL Actividad de corrección].

### [!UICONTROL Configuración del visor de corrección]

Esta configuración le ayuda a controlar el acceso a la propia prueba.

![Una imagen de la [!UICONTROL Configuración del visor de corrección] desde la página de la prueba con el [!UICONTROL Configuración del visor de corrección] opción resaltada en el menú del panel izquierdo.](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL Inicio de sesión obligatorio. Esta revisión no se puede compartir con usuarios invitados] —** La prueba solo se puede compartir con personas que tengan un [!DNL Workfront] licencia de revisión.
* **[!UICONTROL Requerir que las decisiones se firmen electrónicamente] —** Al compartir una prueba, esto requiere que el destinatario tenga permisos de revisión en [!DNL Workfront] y les hace &quot;firmar electrónicamente&quot; la prueba introduciendo su contraseña de prueba cuando toman una decisión sobre la prueba. (Nota: La contraseña de revisión es diferente de la [!DNL Workfront] contraseña. La contraseña de revisión no es fácilmente accesible, por lo que la mayoría de los destinatarios no sabrán esta contraseña). [!DNL Workfront] recomienda hablar con su [!DNL Workfront] antes de utilizar esta función.
* **[!UICONTROL Bloquear la revisión cuando se tomen todas las decisiones necesarias]—** Esto bloquea la prueba a cualquier comentario, respuesta, decisión, etc., una vez que se ha tomado cada decisión sobre la prueba. Esto bloquea toda la versión de prueba, no solo una fase específica del flujo de trabajo de prueba.
* **[!UICONTROL Permitir la descarga del archivo original] —** Los destinatarios de la prueba pueden descargar el archivo de origen original de la prueba desde el visualizador de pruebas (la opción se encuentra en el menú del panel derecho).
* **[!UICONTROL Permitir que se comparta la revisión mediante una dirección URL pública o código para insertar] —** Los destinatarios de la prueba pueden compartir un vínculo de prueba accesible públicamente con cualquier persona.
* **[!UICONTROL Permitir la suscripción a la revisión mediante una dirección URL pública o código para insertar] —** Cualquier persona a la que se envíe la URL pública puede añadirse a la prueba con su dirección de correo electrónico y nombre (si no es un usuario de prueba) o su dirección de correo electrónico y contraseña de prueba (si es un usuario de prueba). (Nota: La contraseña de revisión no es la misma que una [!DNL Workfront] contraseña.)

Esta misma configuración se puede establecer cuando la prueba se carga en [!UICONTROL Configuración de revisión] , en la parte inferior de la ventana de carga.

![Una imagen de la [!UICONTROL Configuración de revisión] en la parte inferior de la ventana de carga.](assets/proof-settings-on-upload-page.png)

### [!UICONTROL Actividad de corrección]

Esta página realiza un seguimiento de toda la actividad que se ha producido en la prueba, además de los mensajes de correo electrónico enviados en relación con esta prueba.

![Una imagen de la [!UICONTROL Actividad de corrección] de la página de la prueba con el [!UICONTROL Actividad de corrección] opción resaltada en el menú del panel izquierdo.](assets/proofing-activity-in-details.png)

El [!UICONTROL Actividad] marcas de tiempo de la sección cuándo se realizaron los comentarios y las decisiones, además de quién los hizo. También registra cuándo se iniciaron las fases del flujo de trabajo de pruebas, cuándo un destinatario abrió por primera vez una prueba y otra información que un administrador o propietario de pruebas querrá conocer. Estos detalles pueden resultar útiles para averiguar cosas como, por ejemplo, por qué nunca se inició una fase del flujo de trabajo de revisión.

El [!UICONTROL Mensajes] La sección muestra marcas de hora de cuándo se enviaron alertas y mensajes de correo electrónico a los destinatarios, quién los envió y el contenido del mensaje. Esto puede resultar útil para solucionar problemas si alguien dice que no recibió un correo electrónico sobre una prueba. Puede comprobar si se ha enviado un correo electrónico y cuándo hacerlo.

[!DNL Workfront] recomienda que el administrador y el propietario de la prueba se familiaricen con la información de estas dos secciones. Cuando combina esta información con la comprensión de cómo leer el [!UICONTROL SOCD] barra de progreso, puede comprender y administrar verdaderamente las pruebas, independientemente de su ubicación en el flujo de trabajo de pruebas.

Una vez que haya terminado de trabajar en [!UICONTROL Detalles del documento] sección, utilice la ruta de exploración para volver al [!UICONTROL Documentos] del proyecto, tarea o problema al que está adjunta la prueba.

![Imagen del rastro de ruta de exploración en el encabezado.](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
