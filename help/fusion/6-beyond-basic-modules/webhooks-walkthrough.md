---
title: Recorrido por Webhooks
description: Aprenda a utilizar un weblink para crear una aplicación que determine si un cliente tiene la edad suficiente para comprar alcohol, todo en [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
doc-type: video
source-git-commit: 57b112921738c01fe4222e50403c8953c412a0f7
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Recorrido por Webhooks

En este escenario se crea una aplicación de tienda de conveniencia para que puedan determinar fácilmente si un cliente tiene la edad suficiente para comprar alcohol. El cajero simplemente necesita anunciar el nombre y la fecha de nacimiento del cliente Y un testigo de cliente verificado en una URL proporcionada. Una vez introducido, esto déclencheur nuestro escenario para calcular la respuesta adecuada y devolverla al solicitante.

![Una imagen que utiliza el módulo de conmutación](assets/beyond-basic-modules-5.png)

## Recorrido por Webhooks

Workfront recomienda ver el vídeo tutorial del ejercicio antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on)

>[!TIP]
>
>Para obtener instrucciones paso a paso sobre cómo completar el tutorial, vaya a la [Recorrido por Webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) ejercicio.

## Configuración de Postman

Para seguir con el ejercicio de tutorial, debe descargar la aplicación gratuita de Postman. Siga los pasos a continuación para ir al área derecha de Postman para el ejercicio.

1. Cree un espacio de trabajo y ábralo.
1. Haga clic en la pestaña New y cree una nueva colección denominada Drying Age.
1. Vuelva a hacer clic en la pestaña New y cree una nueva solicitud de GET denominada GET cumpleaños.
1. Cambie la acción de solicitud de GET a POST.
1. Vaya al área de subficha Cuerpo debajo del campo URL del POST.
1. Elija los datos del formulario debajo de la subficha Autorización .
1. Cree tres claves para Name, Birthdate y clientToken.

![Una imagen que utiliza el módulo de conmutación](assets/beyond-basic-modules-6.png)

## Su turno

>[!NOTE]
>
>Los ejercicios prácticos y los desafíos son opcionales y no son necesarios para completar la formación de Fusion.

Este ejercicio de práctica se basa en lo aprendido en el tutorial, pero no se proporciona la solución.

Cree un vínculo web de Workfront que esté esperando a que se creen nuevas actualizaciones y, a continuación, registre la fecha, el nombre de la persona que realizó la actualización y lo que dice la actualización. Envíe esta información por correo electrónico.

**Sugerencia**: Utilice el módulo de déclencheur de eventos de Workfront Watch para crear su vínculo web. Además, en Workfront las actualizaciones se denominan notas.

**Desafío**: ¿Puede encontrar y agregar la dirección URL donde se realizó la actualización para facilitar el acceso?


## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
