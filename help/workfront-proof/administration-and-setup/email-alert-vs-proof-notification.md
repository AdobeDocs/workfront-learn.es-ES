---
title: Comprender las alertas de correo electrónico y las notificaciones de prueba
description: Comprenda la diferencia entre las alertas de correo electrónico y las notificaciones de prueba en  [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 65%

---

# Comprender las alertas de correo electrónico y las notificaciones de prueba

Las alertas de correo electrónico son diferentes de los correos electrónicos de notificación de prueba. Recibirá un correo electrónico de notificación de prueba cuando se le asigne una nueva prueba para su revisión, cuando una prueba esté atrasada o cuando haya una nueva versión de la prueba que pueda consultar.

![Una imagen de un correo electrónico de notificación de prueba que indica que hay una nueva prueba que revisar.](assets/email-alert-1.png)

Si desactiva la opción de notificación al cargar una prueba, nadie recibe ninguna comunicación de [!DNL Workfront] acerca de la existencia de una nueva prueba para revisar.

Las alertas de correo electrónico se establecen por revisor/aprobador, la mayoría de las veces a medida que se carga la prueba. Se puede asignar un tipo de alerta de correo electrónico predeterminado a los destinatarios de prueba, de modo que no tenga que configurarlo cada vez que cargue una prueba. Hable con el administrador del sistema para obtener estos valores predeterminados.

![Una imagen de una alerta por correo electrónico que indica que se ha tomado una decisión sobre la prueba y que hay un comentario que revisar.](assets/email-alert-2.png)

Incluso si las alertas de correo electrónico están configuradas como [!UICONTROL Deshabilitadas], los destinatarios siguen recibiendo notificaciones de una nueva prueba o versión.

## Prácticas recomendadas

| Práctica recomendada | He aquí por qué |
|---|---|
| Deshabilite la configuración &quot;Enviar correos electrónicos desde Workfront cuando se haga un comentario en una prueba&quot; en las configuraciones de Workfront | Cuando esta configuración está habilitada (que es de forma predeterminada), los usuarios pueden recibir varias notificaciones por correo electrónico para cada comentario en una prueba, una desde la funcionalidad de revisión y otra desde el propio Workfront. Estas duplicidades provocan confusión e interrupciones en los avisos por correo electrónico, así como una bandeja de entrada llena, lo que puede hacer que los usuarios ignoren las notificaciones de prueba. Lo que, a su vez, podría significar plazos incumplidos. <br> <br>Nota: Esta configuración se encuentra en el menú principal de Workfront > Configuración > Correo electrónico > Revisión y aprobación. |


