---
title: Cómo rastrear el progreso de la prueba
description: Aprenda a utilizar [!UICONTROL SOCD] indicadores, progreso de la prueba e informes para realizar un seguimiento del progreso de una prueba en [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
kt: 10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

# Seguimiento del progreso de la prueba

Como administrador de proyectos, administrador de pruebas u otro participante en el proceso de revisión y aprobación, querrá rastrear el progreso de sus pruebas. Puede hacerlo con [!DNL Workfront’s] integrado **indicadores de progreso de prueba** en el [!UICONTROL Documentos] o escribiendo informes personalizados.

Para ver el progreso de la prueba en [!DNL Workfront], debe tener una licencia de Plan, Trabajo o Revisión y ser usuario de pruebas. Si no está seguro de su [!DNL Workfront] cumple estos requisitos, consulte con el administrador del sistema de pruebas de su organización.

## Rastree el progreso de la prueba con [!UICONTROL SOCD] indicadores y estado de prueba

Obtenga una vista de alto nivel de cómo progresa la prueba a través del proceso de revisión y aprobación mediante el [!UICONTROL SOCD] en el [!UICONTROL Documentos] lista. Estos iconos indican acciones específicas realizadas en la prueba.

![Una imagen del [!UICONTROL Documentos] en una [!DNL  Workfront] con el [!UICONTROL SOCD] iconos resaltados.](assets/manage-proofs-socd.png)

Los iconos indican el trabajo realizado en una prueba desde el momento en que se envía la prueba a los destinatarios hasta el momento en que toman una decisión sobre la prueba.

* **S —** La prueba se ha enviado a los destinatarios.
* **O —** Se ha abierto la prueba.
* **C —** Se han hecho comentarios sobre la prueba.
* **D —** Se ha adoptado una decisión sobre la prueba (aprobada, rechazada, etc.).

Los colores indican si la acción está completa o no.

* **Blanco —** El paso aún no ha ocurrido.
* **Verde —** El paso se ha completado.
* **Naranja —** La fecha límite de la prueba es de 24 horas y el paso no se ha realizado.
* **Rojo —** La fecha límite de prueba ha pasado y el paso no ha ocurrido.

La variable [!UICONTROL SOCD] en el [!UICONTROL Documentos] , en el panel de resumen o en la [!UICONTROL Detalles del documento], es un resumen de alto nivel del progreso de la prueba. [!DNL Workfront] configura esto en función del destinatario que sea el &quot;más atrasado&quot; en el proceso de prueba.

Por ejemplo, si hay tres revisores/aprobadores y solo dos de ellos han examinado la prueba y han hecho comentarios, entonces la variable [!UICONTROL SOCD] los iconos muestran la prueba que se ha enviado ([!UICONTROL S]) y abierto ([!UICONTROL O]) pero no que se hayan hecho comentarios ([!UICONTROL C]).

Si desea saber cómo está haciendo cada destinatario de prueba individual, abra el flujo de trabajo de prueba. El progreso general de la prueba se encuentra en la parte superior de la ventana. Cada etapa tiene su propio indicador de progreso en la barra gris.  Y junto a cada usuario está el progreso de ese individuo.

![Una imagen del [!UICONTROL Flujo de trabajo de prueba] de un documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Estado de la prueba

El estado de la prueba se basa en el estado de los destinatarios de prueba de la fase. El estado general de la prueba es visible en la variable [!UICONTROL Documentos] a la derecha del [!UICONTROL SOCD] , para que pueda saber fácilmente si tiene una decisión sobre la prueba.

![Una imagen del [!UICONTROL Documentos] en una [!DNL  Workfront] proyecto con el estado de prueba general resaltado.](assets/manage-proofs-overall-status.png)

Este estado de prueba indica el estado general de la prueba. Por ejemplo, si dos destinatarios aprueban la prueba, sus estados individuales muestran [!UICONTROL Aprobado]. Sin embargo, el tercer destinatario aún no ha tomado una decisión, por lo que el estado de esa persona es [!UICONTROL Pendiente]. Por lo tanto, el estado general se muestra como [!UICONTROL Pendiente].

Si se configuraron estados personalizados para su organización, se utilizarán esos estados. De lo contrario, verá las opciones de estado estándar de:

* [!UICONTROL Pendiente]
* [!UICONTROL Aprobado]
* [!UICONTROL Aprobado con cambios]
* [!UICONTROL Es necesario hacer cambios]
* [!UICONTROL No es relevante]

Abra la ventana del flujo de trabajo de pruebas para ver un estado de prueba para los destinatarios asignados a la variable [!UICONTROL Revisor y aprobador] o [!UICONTROL Aprobador ]funciones de prueba.

## Informes en [!DNL Workfront]

También puede aprovechar [!DNL Workfront’s] funciones de informes para realizar el seguimiento de pruebas a medida que avanzan por el proceso de revisión y aprobación.

Un informe de aprobación de pruebas ayuda a realizar un seguimiento de las aprobaciones pendientes para asegurarse de que se cumplen los plazos.

![Una imagen de un informe de aprobación de prueba en [!DNL  Workfront].](assets/proof-approval-report.png)

Un informe de versión del documento permite administrar y rastrear las versiones de prueba.

![Imagen de un informe de versión de documento en [!DNL  Workfront].](assets/document-version-report.png)

Recomendamos trabajar con su [!DNL Workfront] consultor para crear informes que cumplan los requisitos de su organización. Algunos de los informes deben estar familiarizados con [!DNL Workfront’s] informe de modo de texto.

## Su turno

Hable con su equipo o con el administrador del sistema de pruebas para averiguar qué tipo de informe utilizará en Workfront para mantener los flujos de trabajo de prueba funcionando sin problemas.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
