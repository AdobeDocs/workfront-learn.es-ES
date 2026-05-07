---
title: Comprender las alertas de correo electrónico y las notificaciones de prueba
description: Comprenda la diferencia entre las alertas de correo electrónico y las notificaciones de prueba en  [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:07:01.396Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 307
ht-degree: 100%

---

# Comprender las alertas de correo electrónico y las notificaciones de prueba

Las alertas de correo electrónico son diferentes de los correos electrónicos de notificación de prueba. Recibirá un correo electrónico de notificación de prueba cuando se le haya asignado una nueva prueba para revisarla, cuando una se haya retrasado o haya una nueva versión que pueda ver.

![Una imagen de un correo electrónico de notificación de prueba que indica que hay una nueva prueba que revisar.](assets/email-alert-1.png)

Si desactiva la opción de notificación al cargar una prueba, nadie recibe ninguna comunicación de [!DNL Workfront] acerca de la existencia de una nueva prueba para revisar.

Las alertas de correo electrónico se establecen por revisor/aprobador, la mayoría de las veces a medida que se carga la prueba. Puede asignarse un tipo de alerta de correo electrónico predeterminado a los destinatarios de su prueba para que no tenga que configurarlo cada vez que carguen una. Hable con el administrador del sistema para obtener estos valores predeterminados.

![Una imagen de una alerta por correo electrónico que indica que se ha tomado una decisión sobre la prueba y que hay un comentario que revisar.](assets/email-alert-2.png)

Incluso si las alertas de correo electrónico están configuradas como [!UICONTROL Deshabilitadas], los destinatarios siguen recibiendo notificaciones de una nueva prueba o versión.

## Prácticas recomendadas

| Práctica recomendada | He aquí por qué |
|---|---|
| Deshabilite la configuración “Enviar correos electrónicos desde Workfront cuando se haga un comentario en una prueba” en la configuración de Workfront. | Cuando esta configuración está habilitada (que es de forma predeterminada), los usuarios pueden recibir varias notificaciones por correo electrónico para cada comentario en una prueba, una desde la funcionalidad de revisión y otra desde el propio Workfront. Estas duplicidades provocan confusión e interrupciones en los avisos por correo electrónico, así como una bandeja de entrada llena, lo que puede hacer que los usuarios ignoren las notificaciones de prueba. Esto, a su vez, podría suponer el incumplimiento de los plazos.<br> <br>Nota: Este ajuste se encuentra en el menú principal de Workfront > Configuración > Correo electrónico > Revisión y aprobación. |


