---
title: Trabajar con JSON
description: Aprenda a crear y analizar JSON en un escenario para satisfacer sus necesidades de diseño.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11056
thumbnail: KT11056.png
exl-id: 72d5159e-72e5-4202-90de-753b3d7626de
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Trabajar con JSON

Aprenda a crear y analizar JSON en un escenario para satisfacer sus necesidades de diseño.

## Resumen del ejercicio

El propósito de este ejercicio es mostrar conceptualmente cómo utilizar la información enviada a un escenario en formato JSON, analizándola en campos y elementos que puede asignar a lo largo de su escenario. A continuación, puede obtener información de esas matrices asignadas o agregar la información en JSON para enviarla a otro sistema que espere JSON como entrada de recepción.

![Trabajar con la imagen json 1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## Pasos a seguir

**Cree una estructura de datos y analice el JSON.**

1. Cree un nuevo escenario y asígnele el nombre &quot;Trabajo con datos de anillo JSON&quot;.
1. Para el módulo déclencheur, utilice el módulo Establecer variable.
1. Para el Nombre de variable, escriba &quot;Datos de anillo&quot;.
1. Para el valor Variable, copie y pegue el contenido del documento &quot;_Donut Data - Sample JSON.rtf&quot; encontrado en la carpeta Fusion Exercise Files de su unidad de prueba.

   ![Uso de la imagen 2 de json](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. Cambie el nombre de este módulo a &quot;JSON desde otro conector&quot;.
1. Añada un módulo Analizar JSON.
1. Haga clic en Add para el campo Data structure.
1. Seleccione el Generador y pegue los datos de anillo: datos JSON de muestra que ha copiado en el campo Datos de muestra.

   ![Uso de la imagen 3 de json](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. Haga clic en Guardar y asigne a la estructura de datos el nombre &quot;Datos de anillo&quot;. A continuación, haga clic en Guardar.
1. Asigne los datos de anillo del módulo Establecer variable al campo de cadena JSON.

   ![Trabajar con la imagen json 4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. Guarde el escenario y, a continuación, haga clic en Ejecutar una vez para ver el resultado.

   **La salida del módulo JSON de análisis debe tener este aspecto:**

   ![Uso de la imagen 5 de json](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **Asigne a variables de matriz específicas.**

1. Agregue un enrutador después del módulo Analizar JSON.
1. En la ruta superior, agregue un módulo Establecer variable.
1. Para el Nombre de variable, escriba &quot;Tipos de batería por anillo&quot;.
1. Para el valor Variable, utilice la función map para obtener los tipos de batería de la matriz batters.

   ![Uso de la imagen 6 de json](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. Haga clic en Aceptar y luego en Ejecutar una vez.
1. Abra el inspector de ejecución para ver el paquete de salida de cada una de las tres operaciones, mostrando los tipos de batería de cada una.

   ![Uso de la imagen 7 de json](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **Agregar datos de escenario a JSON.**

1. En la ruta de enrutamiento inferior, agregue un módulo Acumulado a JSON.
1. Para el módulo de origen, seleccione el iterador: el módulo JSON de análisis.
1. Para la Estructura de datos, cree o elija cualquier estructura de datos. Para este ejemplo, utilice datos de anillo.
1. Siga y asigne los campos directamente para este ejemplo, como se muestra a continuación.
1. Cuando llegue a la masa y la superficie, observe que son matrices, por lo que debe hacer clic en Agregar elemento para asignarlas.

   ![Uso de la imagen 8 de json](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. Guarde el escenario y haga clic en Ejecutar una vez.

Observe el inspector de ejecución del módulo Agregado a JSON y observe cómo pudo agregar tres paquetes en una sola cadena JSON. A continuación, puede enviar esta cadena a otros sistemas que esperen JSON.

![Trabajar con la imagen json 9](../12-exercises/assets/working-with-json-walkthrough-9.png)
