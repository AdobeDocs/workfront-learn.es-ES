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
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:41:24.173Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 240
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
