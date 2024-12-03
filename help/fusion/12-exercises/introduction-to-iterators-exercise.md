---
title: Introducción al ejercicio de iteradores
description: Aprenda a utilizar aplicaciones de tipo iteración y a realizar acciones en cada paquete de información.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
recommendations: noDisplay,catalog
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 100%

---

# Introducción al ejercicio de iteradores

Aprenda a utilizar aplicaciones de tipo iteración y a realizar acciones en cada paquete de información.

## Información general del ejercicio

Examine un proyecto específico y todas las tareas dentro de ese proyecto de Workfront. Utilizará el módulo de herramientas de incremento para contar el número de tareas dentro del proyecto. Finalmente, utilizará el módulo de la variable Set para restar el número de tareas secundarias del número de problemas abiertos y generar un valor numérico para cada uno de los paquetes de tareas.

![Imagen 1 de Introducción a los iteradores](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Pasos a seguir

**Lea un proyecto y tareas relacionadas.**

1. Comenzar en un escenario nuevo. Denomínelo “Introducción a la iteración”.
1. Seleccione Workfront como el módulo de activación, Leer un registro.
1. Para Tipo de registro, seleccione Proyecto.
1. Para las Salidas, seleccione ID, Nombre y Descripción.
1. En el campo ID, introduzca el ID del proyecto Northstar Fashion Exhibitors Booth desde la instancia de la unidad de prueba de Workfront.
1. Cambie el nombre de este módulo “Buscar proyectos WF”.
1. Añada otro módulo de Workfront para leer las tareas relacionadas con este proyecto. Elija el módulo Leer registros relacionados.
1. Para Tipo de registro, seleccione Proyecto.
1. Para el ID de registro principal, seleccione el ID del módulo Leer un registro.
1. Para Colecciones, seleccione Tareas.
1. Para las Salidas, seleccione ID, Nombre, Descripción, Número de tareas secundarias, Número de problemas abiertos y Trabajo.
1. Cambie el nombre de este módulo como “Leer tareas del proyecto”.
1. Guarde el escenario y, a continuación, haga clic en Ejecutar una vez para ver los resultados.

   + Haga clic en el inspector de ejecución y verá un paquete como entrada (el proyecto) y 28 paquetes como salida (las tareas).

   **Contar y procesar paquetes iterados.**

1. Añada otro módulo después de Leer registros relacionados. Elija un módulo de herramientas de función Incremento.

   + Deje el campo Restablecer un valor como Nunca y haga clic en OK.

1. Cambie el nombre de este módulo a “Contar el número de tareas”.
1. Agregue un módulo Establecer variable. Establezca el nombre de la variable como “Matemáticas aleatorias”.
1. En el campo Valor de variable, reste el número de tareas secundarias abiertas del número de tareas opTasks abiertas.

   **Debería tener este aspecto:**

   ![Imagen 2 de la Introducción a los iteradores](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Cambie el nombre de este módulo a “Matemáticas aleatorias”.
1. Guarde el escenario y haga clic en Ejecutar una vez.

Para cada una de las tareas producidas por el módulo del iterador Leer registros relacionados, Workfront Fusion realizó 28 ejecuciones. Estos 28 paquetes se seguirán procesando en todo el escenario a menos que se añada un agregador para cerrar el bucle.
