---
title: Ejercicio de patrones de enrutamiento
description: Refuerce su concepto de enrutamiento y rutas de reserva sin tener que lidiar con ninguna otra API.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
recommendations: noDisplay,noCatalog
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 98%

---

# Ejercicio de patrones de enrutamiento

Refuerce su concepto de enrutamiento y rutas de reserva sin tener que lidiar con ninguna otra API.

## Información general del ejercicio

Utilice el módulo de la variable Set para enviar un número a través de varias rutas para ver cómo se comportan los filtros y las reservas al enrutar.

![Imagen 1 de Patrones de enrutamiento](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## Pasos a seguir

1. Cree un nuevo escenario y llámele “Patrones de enrutamiento y reservas”.
1. Para el activador, añada el módulo de herramientas de la variable Set. Introduzca “Mi número” para el nombre de la variable, deje la duración de la variable como Un ciclo y establezca el campo Variable como “75”.

   ![Imagen 2 de Patrones de enrutamiento](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. Añada otro módulo y elija el módulo Enrutador. Para ambas rutas, seleccione la herramienta de función Incrementar y haga clic en Aceptar sin realizar ningún cambio para cada una.

   + Para la primera ruta, cree un filtro, asígnele el nombre “Menos de 100” y establezca la condición en [Mi número] Menos de 100.

   + Para la segunda ruta, cree un filtro, asígnele el nombre “Menos de 1000” y establezca la condición en [Mi número] Menos de 1000. Asegúrese de utilizar el operador Numérico para ambos.

   ![Imagen 3 de Patrones de enrutamiento](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![Imagen 4 de Patrones de enrutamiento](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. Haga clic en Ejecutar una vez y observe cómo el paquete pasa por la ruta “Menos de 100”.
1. A continuación, cambie el campo del módulo de la variable Set a 950 y vuelva a ejecutar. Obsérvelo correr por la segunda ruta.
1. Haga clic en el enrutador y añada una ruta más. Añada el módulo de herramientas de la función Incrementar. Para el filtro, haga clic en la casilla de verificación “La ruta de reserva”. Observe cómo la flecha que señala a esa ruta cambia a un signo de intercalación, indicando que es la ruta de reserva.

   ![Imagen 5 de Patrones de enrutamiento](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. Cambie el número de la variable Set a 9500 y Ejecute una vez. Como el número no es menor que 100 ni menor que 1000, el paquete viaja por la ruta de reserva.

Si agrega una ruta más con un módulo de herramienta de función de Incremento, pero no establece ningún filtro, ¿qué ocurrirá cuando vuelva a hacer clic en Ejecutar? ¿Alguna vez un paquete irá por la ruta de reserva con la cuarta ruta añadida?

+ No, porque sin ningún filtro establecido, cada paquete siempre irá por esta ruta en lugar de la ruta de reserva.
