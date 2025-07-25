---
title: Seguimiento del progreso de la prueba
description: Aprenda a utilizar los indicadores de [!UICONTROL SOCD], el progreso de la revisión e informes para realizar el seguimiento del progreso de una revisión en [!DNL &#x200B; Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 8ad86921177da189503211635116146e886dbd17
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 64%

---

# Seguimiento del progreso de la prueba

Como administrador de proyectos, administrador de pruebas u otra parte interesada en el proceso de revisión y aprobación, querrá rastrear el progreso de sus pruebas. Puede hacerlo con los **indicadores de progreso de la revisión integrados** de [!DNL Workfront's] en la página [!UICONTROL Documentos] o escribiendo informes personalizados.

Para ver el progreso de la revisión en [!DNL Workfront], debe tener una licencia de Plan, Trabajo o Revisión y ser usuario de revisión. Si no está seguro de que su perfil de [!DNL Workfront] cumpla estos requisitos, consulte con el administrador del sistema de revisión de su organización.

## Rastree el progreso de la revisión con indicadores de [!UICONTROL SOCD] y estado de la revisión

Obtenga una vista de alto nivel de cómo progresa la revisión a través del proceso de revisión y aprobación mediante los iconos de [!UICONTROL SOCD] en la lista de [!UICONTROL Documentos]. Estos iconos indican acciones específicas realizadas en la revisión.

![Una imagen de la lista [!UICONTROL Documentos] en un proyecto de [!DNL &#x200B; Workfront] con los iconos de [!UICONTROL SOCD] resaltados.](assets/manage-proofs-socd.png)

Los iconos indican el trabajo realizado en una revisión desde el momento en que se envía la revisión a los destinatarios hasta el momento en que toman una decisión sobre la revisión.

* **S —** La revisión se ha enviado a los destinatarios.
* **O —** La revisión se ha abierto.
* **C —** Se han hecho comentarios sobre la revisión.
* **D —** Se ha adoptado una decisión sobre la revisión (aprobada, rechazada, etc.).

Los colores indican si la acción está completa o no.

* **Blanco —** El paso aún no se ha realizado.
* **Verde —** El paso se ha completado.
* **Naranja —** El plazo de prueba es de 24 horas y no se ha dado el paso.
* **Rojo —** El plazo para la revisión ha vencido y no se ha dado el paso.

El [!UICONTROL SOCD] en la lista [!UICONTROL Documentos], en el panel de resumen o en [!UICONTROL Detalles del documento] es un resumen de alto nivel del progreso de la prueba. [!DNL Workfront] lo configura en función del destinatario que esté &quot;más atrasado&quot; en el proceso de revisión.

Por ejemplo, si hay tres revisores/aprobadores y solo dos de ellos han examinado la revisión y han hecho comentarios, entonces los iconos de [!UICONTROL SOCD] mostrarán que la revisión que se ha enviado ([!UICONTROL S]) y abierto ([!UICONTROL O]), pero no que se hayan hecho comentarios ([!UICONTROL C]).

**Una vez que se toma una decisión final** (por ejemplo, Aprobado o Rechazado) sobre una prueba, todos los indicadores de SOCD pueden aparecer en verde para los usuarios en esa etapa, incluso si no se realizaron acciones individuales (como abrir la prueba o hacer comentarios). Se trata de un comportamiento de todo el sistema diseñado para reflejar la finalización general de la fase, no la participación individual.

**Antes de que se registrara una decisión**, cada indicador SOCD refleja la actividad real del usuario (por ejemplo, blanco si no se realizó ninguna acción y verde si se completó la acción). Después de la decisión, el sistema supone la finalización del flujo de trabajo y actualiza todos los indicadores en consecuencia.

Si desea saber cómo lo está haciendo cada destinatario de revisión individual, abra el flujo de trabajo de revisión. El progreso general de la revisión se encuentra en la parte superior de la ventana. Cada etapa tiene su propio indicador de progreso en la barra gris.  Y junto a cada usuario está el progreso de ese individuo.

![Una imagen de la sección del [!UICONTROL Flujo de trabajo de revisión] de un documento.](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## Estado de la revisión

El estado de prueba se basa en el estado de los destinatarios de prueba de la fase. El estado general de la revisión es visible en la página [!UICONTROL Documentos], a la derecha de los indicadores de [!UICONTROL SOCD], para que pueda saber fácilmente si tiene una decisión sobre la revisión.

![Una imagen de la lista [!UICONTROL Documentos] en un proyecto de [!DNL &#x200B; Workfront] con el estado de revisión general resaltado.](assets/manage-proofs-overall-status.png)

Este estado de revisión indica el estado general de la revisión. Por ejemplo, si dos destinatarios aprueban la revisión, sus estados individuales muestran [!UICONTROL Aprobado]. Sin embargo, el tercer destinatario aún no ha tomado una decisión, por lo que el estado de esa persona es [!UICONTROL Pendiente]. Por lo tanto, el estado general se muestra como [!UICONTROL Pendiente].

Si se configuraron estados personalizados para su organización, se utilizarán esos estados. De lo contrario, verá las opciones de estado estándar de:

* [!UICONTROL Pendiente]
* [!UICONTROL Aprobado]
* [!UICONTROL Aprobado con cambios]
* [!UICONTROL Es necesario hacer cambios]
* [!UICONTROL No es relevante]

Abra la ventana del flujo de trabajo de revisión para ver un estado de revisión para los destinatarios asignados a las funciones de revisión [!UICONTROL Revisor y Aprobador] o [!UICONTROL Aprobador].

## Informes en [!DNL Workfront]

También puede aprovechar las funcionalidades de creación de informes de [!DNL Workfront's] para realizar el seguimiento de revisiones a medida que avanzan por el proceso de revisión y aprobación.

Un informe de aprobación de revisión le ayuda a realizar un seguimiento de las aprobaciones pendientes para asegurarse de que se cumplen los plazos.

![Una imagen de un informe de aprobación de revisión en [!DNL &#x200B; Workfront].](assets/proof-approval-report.png)

Un informe de versión del documento permite administrar y rastrear las versiones de revisión.

![Imagen de un informe de versión de documento en [!DNL &#x200B; Workfront].](assets/document-version-report.png)

Recomendamos trabajar con su consultor de [!DNL Workfront] para crear informes que cumplan los requisitos de su organización. Algunos de los informes deben estar familiarizados con el sistema de informes de modo de texto de [!DNL Workfront's].

## Su turno

Hable con su equipo o con el administrador del sistema de pruebas para averiguar qué tipo de creación de informes utilizará en Workfront para que los flujos de trabajo de prueba se ejecuten sin problemas.

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
