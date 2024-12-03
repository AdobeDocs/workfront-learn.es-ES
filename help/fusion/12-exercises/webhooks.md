---
title: Ejercicio de webhooks
description: Obtenga información sobre cómo crear, activar y administrar escenarios iniciados por los webhooks.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
recommendations: noDisplay,catalog
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 100%

---

# Ejercicio de webhooks

Obtenga información sobre cómo crear, activar y administrar escenarios iniciados por los webhooks.

## Información general del ejercicio

El objetivo de este escenario es crear una aplicación para vender a tiendas de conveniencia, de modo que puedan determinar fácilmente si un cliente tiene o no la edad suficiente para comprar alcohol. El cajero simplemente necesita anunciar el nombre y la fecha de nacimiento del cliente en una URL que se le haya proporcionado. Esta publicación activará el escenario que calculará la respuesta y la devolverá al solicitante.

1. El escenario consta de tres webhooks.
1. El módulo de activación es un webhook personalizado que escucha una publicación.
1. Cuando reciba una publicación, la enviará a uno de los siguientes módulos.
1. El siguiente módulo devuelve una respuesta al solicitante.

   ![Imagen de webhooks 1](../12-exercises/assets/webhooks-walkthrough-1.png)

## Pasos a seguir

**Configurar el webhook del activador.**

1. Cree un nuevo escenario y asígnele el nombre “Usando los webhooks”.
1. Para el activador, añada el módulo de webhook personalizado desde la aplicación Webhooks.
1. Haga clic en Añadir para crear un nuevo Webhook.
1. Escriba el nombre del Webhook en “Aplicación de edad para beber”.
1. Deje las restricciones de IP en blanco, lo que significa que cualquier persona puede enviarle datos.
1. Haga clic en Guardar.


   ![Imagen de webhooks 2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. De nuevo, en el panel de asignación de webhooks, se ha creado una URL para este webhook específico. Haga clic en “Copiar dirección al portapapeles” para copiar esa dirección URL.
1. Haga clic en Aceptar.
1. Haga clic en Ejecutar una vez.
1. Use la URL de Postman para enviar un nombre y una fecha de nacimiento a su webhook personalizado. Para obtener instrucciones sobre la configuración de Postman, consulte el [Tutorial de Webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=es).

   **El panel del módulo Webhooks debería tener este aspecto:**

   ![Imagen de Webhooks 3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **El webhook ahora está en un estado en el que está escuchando datos para determinar la estructura de datos.**

1. Puede definir la estructura de datos de la carga útil que espera obtener (las estructuras de datos se discutirán más adelante). Si no define una estructura de datos, Fusion determinará la estructura de datos automáticamente cuando se envíe la publicación.
1. En Postman, se recomienda enviar a la URL copiada. La publicación debe incluir los datos básicos de formulario. Para este ejemplo, necesita tres campos: Nombre, Fecha de nacimiento y ClientToken.

   ![Imagen de Webhooks 4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. Después de hacer clic en Enviar desde Postman, debe obtener una indicación de que la publicación se ha aceptado.
1. Este es el punto en el que el escenario mostrará que la estructura de datos se ha determinado correctamente.
1. Puede ver que los datos se han recibido abriendo el inspector de ejecución.

   ![Imagen de Webhooks 5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **Configure el enrutamiento para tokens de cliente.**

1. Agregue un enrutador al módulo de activación.
1. En la ruta superior, agregue un módulo de respuesta de Webhook. Esta será nuestra ruta para cuando el token del cliente no coincida.
1. Establezca el estado en 401.
1. Establezca el Cuerpo en {&quot;error&quot;: &quot;No se pudo autenticar la solicitud. Compruebe su clientToken&quot;}.

   ![Imagen de Webhooks 6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. Cree un filtro entre el enrutador y el módulo de respuesta de Webhook. Nómbrelo “El token de cliente no coincide”.
1. Para la condición, utilice el campo clientToken del módulo activador y haga una comparación numérica “No equivale a” con el número 5121933.

   ![Imagen de Webhook 7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. En la ruta inferior, agregue otro módulo de respuesta de Webhook. Esta será nuestra ruta para cuando el token de cliente coincida.
1. Establezca el estado en 200.
1. Al configurar el Cuerpo, utilice las funciones del panel de asignación para comprobar si la persona tiene 18 años o más. Si los tiene, devuelva “¡Tiene edad para beber!”, si no, “No ha tenido suerte…”

   ![Imagen de Webhook 9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. Cree un filtro entre el enrutador y el módulo de respuesta de Webhook en la ruta inferior. Nómbrelo “El token de cliente sí coincide”.
1. Para la condición, utilice el campo clientToken del módulo activador y haga una comparación numérica “Equivale a” con el número 5121933.


   ![Imagen de Webhook 8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. Haga clic en el botón Programación debajo de Ejecutar una vez para activar su escenario, de modo que cada vez que haya una nueva publicación se reciba, recorra cualquiera de los caminos y genere una respuesta. 
