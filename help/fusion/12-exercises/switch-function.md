---
title: Ejercicio de función de cambio
description: Aprenda a utilizar la funcionalidad del conmutador mediante la función de conmutación.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 100%

---

# Ejercicio de función de cambio

Aprenda a utilizar la funcionalidad del conmutador mediante la función de conmutación.

## Información general del ejercicio

Para cambios de datos sencillos, utilice la función de conmutación para transformar un valor en otro dentro de un campo de módulo. En este ejercicio, cambie la clave de dos letras por el nombre real del estado de progreso del proyecto para enviarlo por correo electrónico.

![Imagen 1 de la Función de cambio](../12-exercises/assets/switch-function-walkthrough-1.png)

## Pasos a seguir

1. Clonar el escenario llamado “Uso compartido de variables entre rutas de enrutamiento”.
1. Asigne al nuevo escenario el nombre “Uso compartido de variables entre rutas de enrutamiento: conmutación”.
1. Haga clic en el módulo activador y añada Estado de progreso a la sección Salidas.
1. En el módulo Enviar un correo electrónico, añada Estado de progreso al campo Contenido.

   + Si simplemente asigna el valor proveniente del módulo Búsqueda, hay un código de dos letras para el estado de progreso.
   + Para “conmutar” el código del nombre completo de cada estado de progreso posible, utilice la función de “conmutación” de la pestaña Funciones generales.

1. La función de conmutación utiliza el valor o la expresión Estado de progreso como clave y, a continuación, devuelve el valor de salida basado en esa clave.

   + Un valor clave se define en la primera posición después del Estado de progreso (“LT”) con la salida correspondiente definida en la segunda posición (“Late”).
   + El siguiente valor clave se define en la tercera posición, con la salida correspondiente en la cuarta posición, etc., para tantas claves como se desee.

     ![Imagen 2 de la Función de cambio](../12-exercises/assets/switch-function-walkthrough-2.png)
