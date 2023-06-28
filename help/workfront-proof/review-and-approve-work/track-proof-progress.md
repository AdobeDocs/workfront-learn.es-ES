---
title: Seguimiento del progreso de prueba
description: Aprenda a utilizar [!UICONTROL SOCD] indicadores, progreso de prueba e informes para realizar un seguimiento del progreso de una prueba en [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 1%

---

# Seguimiento del progreso de prueba

Como administrador de proyectos, administrador de pruebas u otra parte interesada en el proceso de revisión y aprobación, querrá rastrear el progreso de sus pruebas. Puede hacer esto con [!DNL Workfront’s] incorporado **indicadores de progreso de prueba** en el [!UICONTROL Documentos] o escribiendo informes personalizados.

Para ver el progreso de la prueba en [!DNL Workfront], debe tener una licencia de planificación, de trabajo o de revisión y ser un usuario revisor. Si no está seguro de que su [!DNL Workfront] Un perfil de cumple estos requisitos. Consulte al administrador del sistema de pruebas de su organización.

## Seguimiento del progreso de prueba con [!UICONTROL SOCD] indicadores y estado de prueba

Obtenga una vista de alto nivel del progreso de la prueba a través del proceso de revisión y aprobación mediante el [!UICONTROL SOCD] iconos en la [!UICONTROL Documentos] lista. Estos iconos indican las acciones específicas realizadas en la prueba.

![Una imagen de la [!UICONTROL Documentos] lista en un [!DNL  Workfront] proyecto con el [!UICONTROL SOCD] iconos resaltados.](assets/manage-proofs-socd.png)

Los iconos indican el trabajo realizado en una prueba desde el momento en que se envía la prueba a los destinatarios hasta el momento en que toman una decisión sobre la prueba.

* **S —** La prueba se ha enviado a los destinatarios.
* **O —** Se ha abierto la revisión.
* **C —** Se han hecho comentarios sobre la prueba.
* **D —** Se ha tomado una decisión sobre la prueba (aprobada, rechazada, etc.).

Los colores indican si la acción está completa o no.

* **Blanco —** El paso aún no se ha producido.
* **Verde —** Se ha completado el paso.
* **Naranja —** El plazo de prueba es de 24 horas y no se ha realizado el paso.
* **Rojo —** La fecha límite de la prueba ha pasado y no se ha producido el paso.

El [!UICONTROL SOCD] en el [!UICONTROL Documentos] , en el panel de resumen o en la [!UICONTROL Detalles del documento], es un resumen de alto nivel del progreso de la prueba. [!DNL Workfront] lo configura en función del destinatario que esté &quot;más atrasado&quot; en el proceso de revisión.

Por ejemplo, si hay tres revisores/aprobadores y solo dos de ellos han mirado la prueba y han hecho comentarios, entonces la variable [!UICONTROL SOCD] Los iconos mostrarán que la prueba se ha enviado ([!UICONTROL S]) y abierto ([!UICONTROL O]) pero no que se hayan hecho comentarios ([!UICONTROL C]).

Si desea saber cómo funciona cada destinatario de prueba individual, abra el flujo de trabajo de prueba. El progreso general de la prueba se encuentra en la parte superior de la ventana. Cada etapa tiene su propio indicador de progreso en la barra gris.  Y junto a cada usuario está el progreso de ese individuo.

![Una imagen de la [!UICONTROL Flujo de trabajo de revisión] de un documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Estado de prueba

El estado de prueba se basa en el estado de los destinatarios de prueba de la fase. El estado general de la prueba se puede ver en la [!UICONTROL Documentos] a la derecha de la página [!UICONTROL SOCD] indicadores, para que pueda saber fácilmente si tiene una decisión sobre la prueba.

![Una imagen de la [!UICONTROL Documentos] lista en un [!DNL  Workfront] proyecto con el estado de prueba general resaltado.](assets/manage-proofs-overall-status.png)

Este estado de prueba indica el estado general de la prueba. Por ejemplo, si dos destinatarios aprobaron la prueba, se muestra su estado individual [!UICONTROL Aprobado]. Sin embargo, el tercer destinatario aún no ha tomado una decisión, por lo que el estado de esa persona es [!UICONTROL Pendiente]. Por lo tanto, el estado general se muestra como [!UICONTROL Pendiente].

Si se han configurado estados personalizados para su organización, se utilizarán esos estados. De lo contrario, verá las opciones de estado estándar de:

* [!UICONTROL Pendiente]
* [!UICONTROL Aprobado]
* [!UICONTROL Aprobado con cambios]
* [!UICONTROL Es necesario hacer cambios]
* [!UICONTROL No es relevante]

Abra la ventana de flujo de trabajo de revisión para ver un estado de prueba de los destinatarios asignados a [!UICONTROL Revisor y aprobador] o [!UICONTROL Aprobador]funciones de prueba.

## Informes en [!DNL Workfront]

También puede aprovechar [!DNL Workfront’s] capacidades de creación de informes para hacer un seguimiento de las pruebas a medida que avancen por el proceso de revisión y aprobación.

Un informe de aprobación de pruebas le ayuda a realizar un seguimiento de las aprobaciones pendientes para asegurarse de que se cumplen los plazos.

![Imagen de un informe de aprobación de pruebas en [!DNL  Workfront].](assets/proof-approval-report.png)

Un informe de versión de documento permite administrar y realizar un seguimiento de las versiones de prueba.

![Imagen de un informe de versión de documento en [!DNL  Workfront].](assets/document-version-report.png)

Recomendamos trabajar con su [!DNL Workfront] para crear informes que cumplan los requisitos de su organización. Algunos de los informes deben estar familiarizados con [!DNL Workfront’s] informes de modo de texto.

## Tu turno

Hable con su equipo o con el administrador del sistema de pruebas para averiguar qué tipo de creación de informes utilizará en Workfront para que los flujos de trabajo de prueba se ejecuten sin problemas.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
