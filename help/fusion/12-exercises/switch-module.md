---
title: Ejercicio del módulo de cambio
description: Obtenga información sobre cómo utilizar el módulo de cambio cuando necesite realizar transformaciones de datos más complejas o dinámicas.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
recommendations: noDisplay,catalog
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:40:26.747Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 327
ht-degree: 100%

---

# Ejercicio del módulo de cambio

Obtenga información sobre cómo utilizar el módulo de cambio cuando necesite realizar transformaciones de datos más complejas o dinámicas.

## Información general del ejercicio

Busque proyectos de correo directo en la unidad de prueba y cambie el nombre de cada proyecto en función de un valor seleccionado en un campo personalizado adjunto al proyecto.

![Imagen 1 del módulo de cambio](../12-exercises/assets/switch-module-walkthrough-1.png)

## Pasos a seguir

1. Cree un nuevo escenario y asígnele el nombre “Uso del módulo de cambio”.
1. Para el módulo de activación, utilice el módulo Búsqueda de Workfront.
1. Configure la conexión de Workfront y establezca el tipo de registro en Project.
1. En los criterios de búsqueda, especifique que solo desea ver los proyectos que tienen un valor en el campo personalizado Canal.
1. Para las salidas, seleccione ID, Nombre, Número de referencia y el campo personalizado Canal.

   ![Imagen 2 del módulo de cambio](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Agregue el módulo de conmutación desde Herramientas.
1. Para el campo Entrada, asigne el campo personalizado Canal del módulo de búsqueda.

   ![Imagen 2 del módulo de cambio](../12-exercises/assets/switch-module-walkthrough-3.png)

1. A continuación, añada casos para cada valor posible proveniente del campo personalizado Canal. El valor posible se introduce en el campo Patrón. Desea que el campo de salida incluya un código de 3 letras específico, seguido del número de referencia del proyecto y, a continuación, el nombre del proyecto.

   **El panel de asignación debe tener este aspecto:**

   ![Imagen 4 del módulo de cambio](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Puede agregar tantos casos adicionales como desee. Observe el campo Otro en la parte inferior. Se utilizará si el valor de entrada no coincide con ninguno de los casos.

   **Actualice el nombre del proyecto en Workfront.**

   ![Imagen 5 del módulo de cambio](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Agregue un módulo de actualización de registro de Workfront.
1. En el campo ID, asigne al ID desde el módulo de activación.
1. Establezca el Tipo de registro en Proyecto.
1. Seleccione el campo Nombre en la sección Seleccionar campos a asignar y asígnelo a la salida del módulo de cambio.
1. Guarde el escenario y ejecute una vez. Vea los nombres de proyecto actualizados en la unidad de prueba.
