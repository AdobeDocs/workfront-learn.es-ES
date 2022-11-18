---
title: Patrones de enrutamiento
description: Refuerce su concepto de enrutamiento y rutas de reserva sin tener que lidiar realmente con ninguna otra API.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Patrones de enrutamiento

Refuerce su concepto de enrutamiento y rutas de reserva sin tener que lidiar realmente con ninguna otra API.

## Información general del ejercicio

Utilice el módulo Set Variable para enviar un número a través de varias rutas para ver cómo se comportan los filtros y las visitas en el orden previsto al enrutar.

![Patrones de enrutamiento Imagen 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Pasos a seguir

1. Cree un nuevo escenario y llámele &quot;Patrones de enrutamiento y abandonos&quot;.
1. Para el déclencheur, añada el módulo de herramientas Establecer variable . Coloque &quot;My Number&quot; para el nombre de la variable, deje la duración de la variable como One cycle y establezca el campo Variable como &quot;75&quot;.

   ![Patrones de enrutamiento Imagen 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Añada otro módulo y elija el módulo Router. Para ambas rutas, seleccione la herramienta Increment function y haga clic en OK sin realizar ningún cambio para cada una.

   + Para la primera ruta, cree un filtro, asígnele el nombre &quot;Menos de 100&quot; y establezca la condición en [Mi número] Menos de 100.

   + Para la segunda ruta, cree un filtro, asígnele el nombre &quot;Menos de 1000&quot; y establezca la condición en [Mi número] Menos de 1000. Asegúrese de utilizar el operador Numérico para ambos.

   ![Patrones de enrutamiento Imagen 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Patrones de enrutamiento Imagen 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Haga clic en Ejecutar una vez y observe cómo el paquete pasa por la ruta &quot;Menos de 100&quot;.
1. A continuación, cambie el campo Set Variable module a 950 y vuelva a ejecutar. Míralo correr por la segunda ruta.
1. Haga clic en el enrutador y añada una ruta más. Añada el módulo de herramientas de la función Increment . Para el filtro, haga clic en la casilla de verificación &quot;La ruta de reserva&quot;. Observe cómo la flecha que señala a esa ruta cambia a un acento circunflejo, indicando que es la ruta de reserva.

   ![Patrones de enrutamiento Imagen 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Cambie el número de la variable Set a 9500 y Ejecutar una vez. Como el número no es menor a 100 o menor que 1000, el paquete viaja por la ruta de reserva.

Si agrega una ruta más con un módulo de herramienta de función Increment pero no establece ningún filtro, ¿qué ocurrirá cuando vuelva a hacer clic en Ejecutar? ¿Alguna vez un paquete irá por la ruta de reserva con la cuarta ruta añadida?

+ No, porque sin ningún filtro establecido, cada paquete siempre irá por esta ruta en lugar de la ruta de reserva.
