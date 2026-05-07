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
autotag-review: '2026-05-06T16:42:51.955Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 390
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
