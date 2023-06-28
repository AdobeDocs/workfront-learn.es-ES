---
title: Filtros
description: Aprenda a utilizar el filtro entre módulos para permitir solo determinados tipos de paquetes.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Filtros

Aprenda a utilizar el filtro entre módulos para permitir solo determinados tipos de paquetes.

## Resumen del ejercicio

Añada un filtro entre los dos módulos en el escenario de asignación básica Más allá para crear únicamente proyectos que tengan un color de proyecto &quot;Rojo&quot; en el archivo CSV.

![Imagen de filtros 1](../12-exercises/assets/filters-walkthrough-1.png)

## Pasos a seguir

1. Cree un clon del escenario &quot;Más allá de la asignación básica&quot; y asígnele el nombre &quot;Uso del filtro poderoso&quot;.

   **Agregue un filtro antes del módulo Crear proyectos de Workfront para permitir que solo se creen proyectos rojos.**

   ![Imagen de filtros 2](../12-exercises/assets/filters-walkthrough-2.png)

1. Añada un filtro haciendo clic en la línea de puntos que conecta los módulos o haciendo clic en la llave inglesa y seleccionando Set up a filter.
1. Utilice el campo Label para asignar un nombre al filtro &quot;Solo proyectos rojos&quot;.
1. En el campo Condición, asigne el campo Color del proyecto (columna 3 del archivo CSV). Seleccione el operador Igual a (sin distinción de mayúsculas y minúsculas) y, a continuación, escriba &quot;red&quot;.
1. Haga clic en Aceptar.

   ![Imagen de filtros 3](../12-exercises/assets/filters-walkthrough-3.png)

   **Pruebe el filtro y compruebe los resultados.**

1. Haga clic en Guardar para guardar el escenario y, a continuación, en Ejecutar una vez.
1. Haga clic en el inspector de ejecución del filtro para ver cómo el filtro examinó cada paquete y cómo se pasó o no se pudo pasar al módulo Crear proyectos de Workfront.

   ![Imagen de filtros 4](../12-exercises/assets/filters-walkthrough-4.png)

1. Busque los proyectos creados en la instancia de Workfront.
