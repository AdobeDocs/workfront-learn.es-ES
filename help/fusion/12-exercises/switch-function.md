---
title: Función de interruptor
description: Aprenda a utilizar la funcionalidad de conmutador mediante la función de conmutador.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Función de interruptor

Aprenda a utilizar la funcionalidad de conmutador mediante la función de conmutador.

## Resumen del ejercicio

Para realizar cambios sencillos en los datos, utilice la función Switch para transformar un valor en otro dentro de un campo de módulo. En este ejercicio, cambie la clave de dos letras por el nombre real del estado del progreso del proyecto para enviarlo por correo electrónico.

![Cambiar función Imagen 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## Pasos a seguir

1. Clone el escenario denominado &quot;Uso compartido de variables entre rutas de enrutamiento&quot;.
1. Asigne un nombre al nuevo escenario &quot;Uso compartido de variables entre rutas de enrutamiento: conmutador&quot;.
1. Haga clic en el módulo déclencheur y añada Estado de progreso a la sección Salidas.
1. En el módulo Enviar un correo electrónico, añada Estado de progreso al campo Contenido.

   + Si solo asigna el valor proveniente del módulo de búsqueda, existe un código de dos letras para el estado de progreso.
   + Para &quot;cambiar&quot; el código para el nombre completo de cada estado de progreso posible, utilice la función &quot;cambiar&quot; de la pestaña General functions.

1. La función switch utiliza el valor o expresión Progress Status como clave y, a continuación, devuelve el valor de salida en función de esa clave.

   + Un valor clave se define en la primera posición después del estado de progreso (&quot;LT&quot;) con el resultado correspondiente definido en la segunda posición (&quot;Late&quot;).
   + El siguiente valor de clave se define en la tercera posición, con el resultado correspondiente definido en la cuarta posición, etc., para tantas claves como desee.

     ![Cambiar función Imagen 2](../12-exercises/assets/switch-function-walkthrough-2.png)
