---
title: Función Switch
description: Aprenda a utilizar la funcionalidad del conmutador mediante la función Switch .
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Función Switch

Aprenda a utilizar la funcionalidad del conmutador mediante la función Switch .

## Información general del ejercicio

Para cambios de datos sencillos, utilice la función Switch para transformar un valor en otro dentro de un campo de módulo. En este ejercicio, cambie la clave de dos letras por el nombre real para que el estado del progreso del proyecto se envíe en un correo electrónico.

![Cambiar imagen de función 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Pasos a seguir

1. Clona el escenario llamado &quot;Uso compartido de variables entre rutas de enrutamiento&quot;.
1. Asigne un nombre al nuevo escenario &quot;Variables compartidas entre rutas de enrutamiento - Conmutador&quot;.
1. Haga clic en el módulo déclencheur y añada Estado de progreso a la sección Salidas .
1. En el módulo Enviar un correo electrónico , agregue Estado de progreso al campo Contenido .

   + Si simplemente asigna el valor proveniente del módulo de búsqueda, hay un código de dos letras para el estado de progreso.
   + Para &quot;cambiar&quot; el código del nombre completo de cada estado de progreso posible, utilice la función &quot;switch&quot; de la pestaña General functions .

1. La función switch utiliza el valor o la expresión Progress Status como clave y, a continuación, devuelve el valor de salida basado en esa clave.

   + Un valor clave se define en la primera posición después del estado de progreso (&quot;LT&quot;) con la salida correspondiente definida en la segunda posición (&quot;Late&quot;).
   + El siguiente valor clave se define en la tercera posición, con el resultado correspondiente definido en la cuarta posición, etc., para tantas claves como se desee.

      ![Cambiar imagen de función 2](../12-exercises/assets/switch-function-walkthrough-2.png)
