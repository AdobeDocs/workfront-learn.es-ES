---
title: Uso de JSON
description: Aprenda a crear y analizar JSON en un escenario para satisfacer sus necesidades de diseño.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Uso de JSON

Aprenda a crear y analizar JSON en un escenario para satisfacer sus necesidades de diseño.

## Información general del ejercicio

El propósito de este ejercicio es mostrar conceptualmente cómo utilizar la información enviada a un escenario en formato JSON, analizándola en campos y elementos que puede asignar a lo largo de su escenario. A continuación, puede obtener información de esas matrices asignadas o agregar la información en JSON para enviarla a otro sistema que espere que JSON sea una entrada de recepción.

![Uso de json Image 1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## Pasos a seguir

**Cree una estructura de datos y analizando JSON.**

1. Cree un nuevo escenario y asígnele el nombre &quot;Uso de datos circulares JSON&quot;.
1. Para el módulo de déclencheur, utilice el módulo Set variable .
1. Para el nombre de la variable, escriba &quot;Datos de anillo&quot;.
1. Para el valor Variable , copie y pegue el contenido del documento &quot;_Donut Data - Sample JSON.rtf&quot; que se encuentra en la carpeta Fusion Exercise Files de la unidad de prueba.

   ![Uso de json Image 2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. Cambie el nombre de este módulo &quot;JSON desde otro conector&quot;.
1. Agregue un módulo JSON de análisis.
1. Haga clic en Add para el campo Data structure .
1. Seleccione el Generador y pegue los datos de anillo - Muestra de datos JSON que ha copiado en el campo Datos de ejemplo .

   ![Uso de json Image 3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. Haga clic en Guardar y asigne a la estructura de datos el nombre &quot;Datos de anillo&quot;. A continuación, haga clic en Guardar.
1. Asigne los datos de anillo del módulo Set variable al campo JSON string .

   ![Uso de json Image 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. Guarde el escenario y haga clic en Ejecutar una vez para ver el resultado.

   **La salida del módulo Parse JSON debe tener este aspecto:**

   ![Uso de json Image 5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **Asigne a variables de matriz específicas.**

1. Añada un router después del módulo Parse JSON.
1. En la ruta superior, agregue un módulo Set variable .
1. Para el nombre de la variable, escriba &quot;Tipos de barras por anillo&quot;.
1. Para el valor Variable, utilice la función map para obtener los tipos de barras de la matriz de batters.

   ![Uso de json Image 6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. Haga clic en Aceptar y, a continuación, en Ejecutar una vez.
1. Abra el inspector de ejecución para ver el paquete de salida de cada una de las tres operaciones, mostrando los tipos de batería de cada una.

   ![Uso de json Image 7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **Agregar datos de escenario a JSON.**

1. En la ruta de enrutamiento inferior, agregue un agregado al módulo JSON.
1. Para el módulo de origen, elija el iterador: el módulo Parse JSON.
1. Para la estructura de datos, cree o elija cualquier estructura de datos. Para este ejemplo, utilice datos de anillo.
1. Continúe y asigne los campos directamente para este ejemplo, como se muestra a continuación.
1. Cuando llegue a la batería y la parte superior, fíjese en que son matrices, por lo que debe hacer clic en Agregar elemento para asignarlas.

   ![Uso de json Image 8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. Guarde el escenario y haga clic en Ejecutar una vez.

Observe el inspector de ejecución del módulo Aggregate to JSON y observe cómo ha podido agregar tres paquetes en una sola cadena JSON. A continuación, puede enviar esta cadena a otros sistemas que esperen JSON.

![Uso de json Image 9](../12-exercises/assets/working-with-json-walkthrough-9.png)
