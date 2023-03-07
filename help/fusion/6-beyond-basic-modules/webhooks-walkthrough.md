---
title: Tutorial de Webhooks
description: Aprenda a utilizar un webhook para crear una aplicación que determine si un cliente tiene la edad suficiente para comprar alcohol o no, todo en [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Tutorial de Webhooks

## Información general

En este escenario se crea una aplicación de una tienda de conveniencia para que puedan determinar fácilmente si un cliente tiene la edad suficiente para comprar alcohol o no. El cajero solo tiene que publicar el nombre y la fecha de nacimiento del cliente Y un token de cliente verificado en una URL que se haya proporcionado. Una vez introducido, esto almacenará en déclencheur nuestro escenario para calcular la respuesta adecuada y devolvérsela al solicitante.

![Una imagen mediante el módulo de conmutación](assets/beyond-basic-modules-5.png)

## Tutorial de Webhooks

Workfront recomienda ver el vídeo del tutorial de ejercicios antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>Para obtener instrucciones paso a paso sobre cómo completar el tutorial, vaya a la [Tutorial de Webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) hacer ejercicio.

## Configuración de Postman

Para continuar con el ejercicio de introducción, debe descargar la aplicación gratuita de Postman. Siga los pasos a continuación para desplazarse al área derecha de Postman para el ejercicio.

1. Cree un espacio de trabajo y, a continuación, ábralo.
1. Haga clic en la pestaña New y cree una nueva colección llamada Drinking Age.
1. Vuelva a hacer clic en la pestaña Nuevo y cree una nueva solicitud de GET denominada cumpleaños de GET.
1. Cambie la acción de solicitud de GET a POST.
1. Vaya al área de la subpestaña Body debajo del campo POST URL.
1. Seleccione form-data en la subpestaña Authorization.
1. Cree tres claves para Name, Birthdate y clientToken.

![Una imagen mediante el módulo de conmutación](assets/beyond-basic-modules-6.png)

## Tu turno

>[!NOTE]
>
>Los ejercicios y desafíos de práctica son opcionales y no son necesarios para completar el entrenamiento de Fusion.

Este ejercicio práctico se basa en lo que ha aprendido en el tutorial, pero no se proporciona la solución.

Cree un webhook de Workfront que esté esperando nuevas actualizaciones creadas y luego registre la fecha, el nombre de la persona que realizó la actualización y lo que indica la actualización. Envíese esta información por correo electrónico.

**Sugerencia**: utilice el módulo déclencheur de Workfront Watch Events para crear el webhook. Además, en Workfront las actualizaciones se denominan notas.

**Desafío**: ¿Puede encontrar y agregar la dirección URL donde se realizó la actualización para facilitar el acceso?


## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
