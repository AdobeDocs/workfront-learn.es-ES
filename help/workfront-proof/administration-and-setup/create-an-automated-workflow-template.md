---
title: Creación de una plantilla de flujo de trabajo automatizada
description: Aprenda a crear una plantilla de flujo de trabajo automatizada asignando destinatarios de revisión y estableciendo plazos de revisión. A continuación, comparta la plantilla con otros usuarios.
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335130.png
jira: KT-8830
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: eac89e40-d3ea-4376-82a2-16bec550d131
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:09:06.617Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 435
ht-degree: 91%

---

# Creación de una plantilla de flujo de trabajo automatizada

Este vídeo contiene información sobre:

* Cree una plantilla de flujo de trabajo automatizada para revisiones de [!DNL  Workfront]
* Asignación de destinatarios de prueba
* Establecer un plazo para el proceso de revisión y aprobación
* Comparta la plantilla de flujo de trabajo automatizado con otros usuarios

>[!VIDEO](https://video.tv.adobe.com/v/335130/?quality=12&learn=on&enablevpops=1)

## Opciones de activación de fase adicionales

Rara vez se utilizan dos opciones para determinar cuándo se debe iniciar una fase de flujo de trabajo de revisión: la opción [!UICONTROL Fecha y hora] y la opción “[!UICONTROL Cuando pasa el plazo de la fase anterior]”.

La segunda opción solo funciona en escenarios en los que tiene un gran grupo de personas revisando y no quiere esperarlas a todas. Es una especie de “Le daré una cierta cantidad de tiempo para completar su revisión y luego perderá su oportunidad”. Pero incluso esto puede ralentizar un proceso de revisión.

Si utiliza “[!UICONTROL cuando pasa el plazo de la fase anterior]” es importante recordar que puede activar manualmente un escenario en cualquier momento si no quiere esperar a que pase una fecha límite.

## Prácticas recomendadas

| Práctica recomendada | He aquí por qué |
|---|---|
| Establezca la función de prueba del creador de pruebas en el Revisor. | La función de prueba del Revisor garantiza que el creador de la prueba pueda realizar comentarios y acceder a los comentarios dejados por otros. La mayoría de las veces, el creador de la prueba no está obligado a tomar una decisión sobre una prueba que ha cargado. Las funciones de revisión Aprobador, Revisor y Aprobador, Autor, o Moderador requieren que se tome una decisión. Si al creador de pruebas se le asigna una de estas funciones de prueba, pero nunca toma una decisión, esto puede afectar negativamente a los plazos de la revisión. |
| Evite utilizar la función de revisión del Aprobador. | La función de revisión del Aprobador no permite al usuario realizar comentarios sobre esta revisión. Esto podría llevar a que un usuario rechace la revisión, sin ninguna explicación porque no puede hacer comentarios. Utilice la función de revisión del Revisor y Aprobador en su lugar para que el usuario pueda proporcionar comentarios. |
| Evite la opción de alerta de correo electrónico de revisión de todas las actividades. | Esta opción envía una notificación de correo electrónico de prueba cada vez que sucede algo con una prueba: se hace un comentario, se publica una respuesta, se toma una decisión, etc. El destinatario básicamente ve la actividad de prueba a medida que se produce.<br><br>Para los propietarios y creadores de revisiones, la alerta de correo electrónico de Decisiones funciona mejor para los flujos de trabajo de revisión en varias etapas y la Decisión final funciona mejor para los flujos de trabajo de una sola etapa. Por lo general, todos los demás pueden configurarse como Deshabilitado, a menos que deseen que se les notifique a otras personas que realicen comentarios o decisiones (en cuyo caso, una de las opciones de correo electrónico de resumen podría funcionar mejor). |
