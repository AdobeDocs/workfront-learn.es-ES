---
title: Patrones de enrutamiento
description: Refuerce su concepto de enrutamiento y rutas de reserva sin necesidad de lidiar con ninguna otra API.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Patrones de enrutamiento

Refuerce su concepto de enrutamiento y rutas de reserva sin necesidad de lidiar con ninguna otra API.

## Resumen del ejercicio

Utilice el módulo Establecer variable para enviar un número a través de varias rutas para ver cómo se comportan los filtros y las retrospectivas al enrutar.

![Patrones de enrutamiento Imagen 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Pasos a seguir

1. Cree un nuevo escenario y denomínelo &quot;Patrones de enrutamiento y reserva&quot;.
1. Para el déclencheur, añada el módulo de la herramienta Establecer variable. Ponga &quot;Mi número&quot; para el nombre de la variable, deje la duración de la variable como un ciclo y establezca el campo Variable en &quot;75&quot;.

   ![Patrones de enrutamiento Imagen 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Añada otro módulo y elija el módulo Router. Para ambas rutas, seleccione la herramienta de función Incremento y haga clic en Aceptar sin realizar ningún cambio para cada una.

   + Para la primera ruta, cree un filtro, asígnele el nombre &quot;Menos de 100&quot; y establezca la condición en [Mi número] Menos de 100

   + Para la segunda ruta, cree un filtro, asígnele el nombre &quot;Menos de 1000&quot; y establezca la condición en [Mi número] Menos de 1000. Asegúrese de utilizar el operador Numérico para ambos.

   ![Patrones de enrutamiento Imagen 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Patrones de enrutamiento Imagen 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Haga clic en Ejecutar una vez y observe cómo el paquete pasa por la ruta &quot;Menos de 100&quot;.
1. A continuación, cambie el campo del módulo Establecer variable a 950 y Ejecute una vez más. Véanlo correr por el segundo camino.
1. Haga clic en el enrutador y agregue una ruta más. Añada el módulo de la herramienta Increment function. Para el filtro, haga clic en la casilla de verificación &quot;La ruta de reserva&quot;. Observe cómo la flecha que señala a esa ruta cambia a un acento circunflejo, lo que indica que es la ruta de reserva.

   ![Patrones de enrutamiento Imagen 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Cambie el número de la variable Set a 9500 y Run once. Como el número no es menor que 100 ni menor que 1000, el paquete se desplaza por la ruta de reserva.

Si agrega una ruta más con un módulo de herramienta Incremento de función, pero no establece ningún filtro, ¿qué ocurrirá cuando haga clic en Ejecutar una vez más? ¿Seguirá un paquete en la ruta alternativa con la cuarta ruta añadida?

+ No, porque sin ningún filtro establecido, cada paquete siempre seguirá esta ruta en lugar de la ruta de reserva.
