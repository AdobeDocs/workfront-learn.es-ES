---
title: Tutorial de enrutadores
description: Aprenda a utilizar un enrutador para pasar paquetes de Pokémon frente a superhéroes por la ruta correcta en [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Tutorial de enrutadores

## Información general

Use un enrutador para pasar paquetes de Pokemon vs. superhéroes por la ruta correcta y luego cree una tarea para cada personaje.

![Una imagen del escenario de Fusion](assets/universal-connectors-and-routing-2.png)

## Tutorial de enrutadores

Workfront recomienda ver el vídeo del tutorial de ejercicios antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12)

## URL del ejercicio

* Sitio web de la API Superhero: `https://www.superheroapi.com/`
* Primera URL del ejercicio: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* Segunda URL para el ejercicio: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

Si tiene problemas para acceder a su propio token de superhéroe, puede utilizar este token compartido: 10110256647253588. Tenga en cuenta cuántas veces llama a la API de superhéroes para que este token compartido siga funcionando para todos.

>[!TIP]
>
>Para obtener instrucciones paso a paso sobre cómo completar el tutorial, vaya a la [Tutorial de enrutadores](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) hacer ejercicio.


## Buscar elementos en el panel de asignación

El campo Buscar elementos en la parte superior de los paneles de asignación le ayuda a encontrar rápidamente campos en el panel, incluso si están anidados en matrices. La búsqueda no distingue entre mayúsculas y minúsculas.

![Imagen del primer panel de búsqueda](assets/universal-connectors-and-routing-3.png)

![Imagen del segundo panel de búsqueda](assets/universal-connectors-and-routing-4.png)

## Sugerencias y trucos para trabajar con API

Hasta este momento, ha trabajado con una API muy sencilla (interfaz de programación de aplicaciones) que no requiere autenticación adicional para extraer la información necesaria en el escenario. A continuación se proporcionan algunas sugerencias para ayudarle a navegar trabajando con API y conectores universales.

## Paso 1: Determinar el tipo de API

Workfront y muchos sistemas de software se crean mediante una API de REST (transferencia de estado representacional), que es el tipo de API más fácil y estándar de la actualidad. Sin embargo, hay algunos otros, como:

* SOAP (Protocolo simple de acceso a objetos) (la API de Workfront Proof se basa en SOAP)
* FTP (Protocolo de transferencia de archivos)
* SFTP (Protocolo seguro de transferencia de archivos)
* Para obtener más información, realice una búsqueda web de tipos de API y palabras clave de interés.

>[!NOTE]
>
>Al conectarse a plataformas más grandes como Salesforce, diferentes áreas de esas plataformas proporcionarán diferentes API. Asegúrese de encontrar el adecuado para el servicio al que desea conectarse.

## Paso 2: Determinar el tipo de autenticación requerida por la API

La autenticación de API es una forma de identificación que se utiliza para controlar el acceso a un servicio, como cuando intenta conectarse a través de Workfront Fusion. Le ayuda a probar a otro sistema que está autorizado a acceder al sistema. OAuth 2 es el tipo de autenticación más común utilizado en la actualidad. Obtenga más información con una búsqueda en Internet acerca de la autenticación de API.

La autenticación puede ser el aspecto más difícil de trabajar con una API. Una de las funciones más valiosas de los conectores universales de Workfront Fusion es que Workfront Fusion puede gestionar la autenticación por usted cuando se utilizan métodos de autenticación comunes como la autenticación básica, como OAuth 2, clave de API y otros. Una vez que haya creado una conexión utilizando el módulo Workfront Fusion apropiado para su método de autenticación (por ejemplo, OAuth 2), Workfront Fusion generará continuamente claves de API y/o tokens cada vez que quiera ejecutar su escenario.

Obtenga información acerca de los diferentes tipos de autenticación que proporciona Workfront en el artículo de información general sobre la autenticación mejorada en Experience League.

## Paso 3: Lea la documentación de la API y busque los extremos necesarios

Cuando una API interactúa con otro sistema, los puntos de contacto de esta comunicación se consideran extremos. Un punto final es el lugar donde las API envían solicitudes y donde se encuentra el recurso.

Al interactuar con una API mediante un conector universal, debe comprender qué extremos admite la API y qué datos se requieren para cada solicitud. La documentación de la API debe describir los puntos finales de una API y cómo realizar operaciones comunes como crear, leer, actualizar o eliminar. La realización de estas llamadas requiere cierta práctica, especialmente si es la primera vez que realiza llamadas de API o que trabaja con una nueva API.

Obtenga más información sobre los conectores universales de Workfront Fusion y cómo configurarlos para conectarse con las API que necesite en Experience League.

## Nota final

Puede comprobar la lista completa de nuestros conectores de aplicación creados previamente en Experience League. Si desea sugerir un nuevo conector de aplicación al equipo de productos de Workfront Fusion, envíe su idea a Innovation Lab. Si no lo ha enviado antes, obtenga más información sobre el Laboratorio de innovación, además de cómo puede votar por ideas y participar en la priorización de la tabla de clasificación dos veces al año. Si ya tiene acceso al laboratorio de innovación, inicie sesión y envíe sus ideas.

## Tu turno

>[!NOTE]
>
>Los ejercicios y desafíos de práctica son opcionales y no son necesarios para completar el entrenamiento de Fusion.

Este ejercicio práctico se basa en lo que ha aprendido en el tutorial, pero no se proporciona la solución.

En el módulo Establecer múltiples variables para caracteres Pokemon, cree una variable llamada &quot;Stat (Level)&quot;. Asigne el nombre de Pokemon Stats a esta variable. Utilice la capacidad de valor de matriz para cambiar la forma en que se muestra la matriz, de modo que cada estadística sea una nueva línea como se muestra a continuación.

**Sugerencia:** Solo hay seis estadísticas diferentes de Pokémon con un nivel correspondiente.

![Una imagen de Stats](assets/universal-connectors-and-routing-5.png)

**Reto:** Vea si puede utilizar las fórmulas de matriz para obtener las capacidades de mostrar de la misma manera que arriba como filas diferentes en lugar de una cadena de valores separados por una coma. Hay una pista en la captura de pantalla a continuación.

![Imagen del nombre de una matriz](assets/universal-connectors-and-routing-6.png)

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
