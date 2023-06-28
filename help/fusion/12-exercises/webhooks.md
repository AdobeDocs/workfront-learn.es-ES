---
title: Webhooks
description: Aprenda a crear, almacenar en déclencheur y administrar escenarios iniciados por ganchos web.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Webhooks

Aprenda a crear, almacenar en déclencheur y administrar escenarios iniciados por ganchos web.

## Resumen del ejercicio

El propósito de este escenario es crear una aplicación para venderla a las tiendas de conveniencia de modo que puedan determinar fácilmente si un cliente tiene la edad suficiente para comprar alcohol o no. El cajero solo tiene que publicar el nombre y la fecha de nacimiento del cliente en la dirección URL que se le haya facilitado. Esa publicación almacenará en déclencheur el escenario que calculará la respuesta y la devolverá al solicitante.

1. El escenario consta de tres webhooks.
1. El módulo déclencheur es un webhook personalizado que escucha una publicación.
1. Cuando reciba una publicación, la enviará a uno de los siguientes módulos.
1. El siguiente módulo devuelve una respuesta al solicitante.

   ![Imagen 1 de webhooks](../12-exercises/assets/webhooks-walkthrough-1.png)

## Pasos a seguir

**Configure el webhook de déclencheur.**

1. Cree un nuevo escenario y asígnele el nombre &quot;Uso de webhooks&quot;.
1. Para el déclencheur, añada el módulo webhook personalizado desde la aplicación Webhooks.
1. Haga clic en Añadir para crear un nuevo webhook.
1. Escriba el nombre de webhook &quot;Aplicación de la edad de beber&quot;.
1. Deje las restricciones de IP en blanco, lo que significa que cualquier persona puede enviarle datos.
1. Haga clic en Guardar.


   ![Imagen 2 de webhooks](../12-exercises/assets/webhooks-walkthrough-2.png)

1. En el panel de asignación de webhooks se ha creado una URL para este webhook específico. Haga clic en &quot;Copiar dirección en el portapapeles&quot; para copiar esa dirección URL.
1. Haga clic en Aceptar.
1. Haga clic en Ejecutar una vez.
1. Utilice la URL de Postman para enviar un nombre y un cumpleaños a su webhook personalizado. Para obtener instrucciones sobre la configuración de Postman, consulte la [Tutorial de Webhooks](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=en) tutorial.

   **El panel del módulo Webhooks debería tener este aspecto:**

   ![Imagen de webhooks 3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **El webhook se encuentra ahora en un estado en el que está escuchando datos para determinar la estructura de datos.**

1. Puede definir la estructura de datos de la carga útil que espera obtener (las estructuras de datos se tratarán más adelante). Si no define una estructura de datos, Fusion determinará la estructura de datos automáticamente cuando se envíe la publicación.
1. En el lado de Postman que desee enviar a la dirección URL copiada. La publicación debe incluir datos de formulario básicos. Para este ejemplo necesita tres campos: Name, Birthdate y clientToken.

   ![Imagen 4 de webhooks](../12-exercises/assets/webhooks-walkthrough-4.png)

1. Después de hacer clic en Enviar desde Postman, debe recibir una indicación de que la publicación se ha aceptado.
1. Este es el punto en el que su escenario mostrará que la estructura de datos se ha determinado correctamente.
1. Puede ver que los datos se han recibido abriendo el inspector de ejecución.

   ![Imagen 5 de webhooks](../12-exercises/assets/webhooks-walkthrough-5.png)

   **Configure el enrutamiento para tokens de cliente.**

1. Agregue un enrutador al módulo de déclencheur.
1. En la ruta superior, añada un módulo de respuesta Webhook. Esta será nuestra ruta para cuando el token del cliente no coincida.
1. Establezca el estado en 401.
1. Establezca el Cuerpo en {&quot;error&quot;: &quot;No se pudo autenticar la solicitud. Compruebe su clientToken&quot;}.

   ![Webhooks Image 6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. Cree un filtro entre el enrutador y el módulo de respuesta Webhook. Asígnele el nombre &quot;El token de cliente no coincide&quot;.
1. Para la condición, utilice el campo clientToken del módulo de déclencheur y realice una comparación numérica de &quot;No igual a&quot; con el número 5121933.

   ![Imagen de webhooks 7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. En la ruta inferior, añada otro módulo de respuesta Webhook. Esta será nuestra ruta para cuando el token del cliente no coincida.
1. Establezca el estado en 200.
1. Al configurar el Cuerpo, utilice las funciones del panel de asignación para comprobar si la persona tiene 21 años o más. Si lo son, devuelven &quot;¡Ya tienes edad para beber!&quot;, de lo contrario devuelven &quot;No tienes suerte...&quot;

   ![Imagen de webhooks 9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. Cree un filtro entre el enrutador y el módulo de respuesta Webhook en la ruta inferior. Asígnele el nombre &quot;El token de cliente no coincide&quot;.
1. Para la condición, utilice el campo clientToken del módulo de déclencheur y realice una comparación numérica de &quot;Igual a&quot; con el número 5121933.


   ![Imagen 8 de webhooks](../12-exercises/assets/webhooks-walkthrough-8.png)

1. Haga clic en el botón Programación en Ejecutar una vez para activar el escenario y que, cada vez que haya una nueva publicación, se reciba, siga cualquiera de las rutas y genere una respuesta.
