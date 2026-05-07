---
title: Tutorial de webhooks
description: Aprenda a utilizar un webhook para crear una aplicación que determine si un cliente tiene la edad suficiente para comprar alcohol, todo en  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
recommendations: noDisplay,catalog
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:29:34.923Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 100%

---

# Tutorial de webhooks

En este escenario se crea una aplicación de tienda de conveniencia para que puedan determinar fácilmente si un cliente tiene la edad suficiente para comprar alcohol. El cajero simplemente necesita anunciar el nombre y la fecha de nacimiento del cliente Y un token de cliente verificado en una URL proporcionada. Una vez introducido, esto activará nuestro escenario para calcular la respuesta adecuada y devolverla al solicitante.

![Una imagen del uso del módulo de conmutación](assets/beyond-basic-modules-5.png)

## Tutorial de webhooks

Workfront recomienda ver el vídeo tutorial del ejercicio antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/3417944/?captions=spa&quality=12&learn=on&enablevpops=1)


## Configuración de Postman

Para seguir con el ejercicio del tutorial, debe descargar la aplicación gratuita de Postman. Siga los pasos a continuación para ir al área derecha de Postman para el ejercicio.

1. Cree un espacio de trabajo y ábralo.
1. Haga clic en la pestaña Nuevo y cree una nueva colección denominada Edad para beber.
1. Vuelva a hacer clic en la pestaña Nuevo y cree una nueva petición GET denominada GET fecha de nacimiento.
1. Cambie la acción de solicitud de GET a POST.
1. Vaya al área de subpestaña Cuerpo debajo del campo POST URL.
1. Elija los datos del formulario debajo de la subpestaña Autorización.
1. Cree tres claves para Nombre, Fecha de nacimiento y clientToken.

![Una imagen del uso del módulo de conmutación](assets/beyond-basic-modules-6.png)

## Su turno

>[!NOTE]
>
>Los ejercicios prácticos y los desafíos son opcionales y no son necesarios para completar la formación de Fusion.

Este ejercicio práctico se basa en lo aprendido en el tutorial, pero no se proporciona la solución.

Cree un wehook de Workfront que esté esperando a que se creen nuevas actualizaciones y, a continuación, registre la fecha, el nombre de la persona que realizó la actualización y lo que dice la actualización. Envíese a sí mismo esta información por correo electrónico.

**Sugerencia**: Utilice el módulo de activación de eventos de Workfront Watch para crear su webhook. Además, en Workfront las actualizaciones se denominan notas.

**Desafío**: ¿Puede encontrar y agregar la dirección URL donde se realizó la actualización para facilitar el acceso?


## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
