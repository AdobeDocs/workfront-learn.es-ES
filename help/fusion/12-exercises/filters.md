---
title: Ejercicio con filtros
description: Descubra cómo utilizar el filtro entre módulos para permitir solo determinados tipos de paquetes.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:22.961Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 100%

---

# Ejercicio con filtros

Descubra cómo utilizar el filtro entre módulos para permitir solo determinados tipos de paquetes.

## Información general del ejercicio

Agregue un filtro entre los dos módulos en el escenario Más allá de la asignación básica para crear solo proyectos que tengan el color de proyecto “Rojo” en el archivo CSV.

![Imagen 1 de los filtros](../12-exercises/assets/filters-walkthrough-1.png)

## Pasos a seguir

1. Cree un clon del escenario “Más allá de la asignación básica” y asígnele el nombre “Usando el poderoso filtro”.

   **Agregue un filtro antes del módulo Crear proyectos de Workfront para que solo se puedan crear proyectos de color rojo.**

   ![Imagen 2 de los filtros](../12-exercises/assets/filters-walkthrough-2.png)

1. Añada un filtro haciendo clic en la línea de puntos que conecta los módulos o haciendo clic en la llave inglesa y seleccionando Configurar un filtro.
1. Utilice el campo Etiquetar para asignar al filtro el nombre “Solo proyectos de color rojo”.
1. En el campo Condición, asigne el campo Color del proyecto (columna 3 del archivo CSV). Seleccione el operador Igual a (sin distinción de mayúsculas y minúsculas) y, a continuación, escriba “rojo”.
1. Haga clic en Aceptar.

   ![Imagen 3 de los filtros](../12-exercises/assets/filters-walkthrough-3.png)

   **Pruebe el filtro y compruebe los resultados.**

1. Haga clic en Guardar para guardar el escenario y, a continuación, en Ejecutar una vez.
1. Haga clic en el inspector de ejecución del filtro para ver cómo el filtro ha examinado cada paquete y si ha pasado o no al módulo Crear proyectos de Workfront.

   ![Imagen 4 de los filtros](../12-exercises/assets/filters-walkthrough-4.png)

1. Busque los proyectos creados en la instancia de Workfront.
