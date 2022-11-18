---
title: Introducción a los iteradores
description: Aprenda a utilizar aplicaciones de tipo iteración y a realizar acciones en cada paquete de información.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# Introducción a los iteradores

Aprenda a utilizar aplicaciones de tipo iteración y a realizar acciones en cada paquete de información.

## Información general del ejercicio

Observe un proyecto específico en Workfront y luego observe todas las tareas dentro de ese proyecto. Utilizará el módulo de herramientas de incremento para contar el número de tareas dentro del proyecto. Finalmente, utilizará el módulo Set variable para restar el número de elementos secundarios del número de problemas abiertos y generar un valor numérico para cada uno de los paquetes de tareas.

![Introducción a los iteradores Imagen 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## Pasos a seguir

**Lea un proyecto y tareas relacionadas.**

1. Iniciar un nuevo escenario. Denomínela &quot;Introducción a la iteración&quot;.
1. Seleccione Workfront como módulo de déclencheur, Leer un registro.
1. Para Tipo de registro, seleccione Proyecto.
1. Para las salidas, seleccione ID, Nombre y Descripción.
1. En el campo ID , coloque el ID del proyecto del componente Booth de los Expositores de moda de Northstar desde la instancia de la unidad de prueba de Workfront.
1. Cambie el nombre de este módulo &quot;Buscar proyectos WF&quot;.
1. Añada otro módulo de Workfront para leer las tareas relacionadas con este proyecto. Elija el módulo Leer registros relacionados .
1. Para Tipo de registro, seleccione Proyecto.
1. Para el ID de registro principal, seleccione el ID del módulo Leer un registro .
1. Para Colecciones, seleccione Tareas.
1. Para los productos, seleccione ID, nombre, descripción, número de elementos secundarios, número de problemas abiertos y trabajo.
1. Cambie el nombre de este módulo &quot;Leer tareas del proyecto&quot;.
1. Guarde el escenario y, a continuación, haga clic en Ejecutar una vez para ver los resultados.

   + Haga clic en el inspector de ejecución y verá un paquete como entrada (el proyecto) y 28 paquetes como salida (las tareas).

   **Contar y procesar paquetes iterados.**

1. Añada otro módulo después Leer registros relacionados. Elija un módulo de herramientas de función Increment .

   + Deje el campo Reset a value como Never y haga clic en OK.

1. Cambie el nombre de este módulo &quot;Cuente el número de tareas&quot;.
1. Agregue un módulo Set variable . Establezca el nombre de la variable en &quot;Matemáticas aleatorias&quot;.
1. En el campo Variable value , reste el número de elementos secundarios abiertos del número de tareas opTasks abiertas.

   **Debería tener este aspecto:**

   ![Introducción a los iteradores Imagen 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. Cambie el nombre de este módulo &quot;Random Math&quot;.
1. Guarde el escenario y haga clic en Ejecutar una vez.

Para cada una de las tareas producidas por el módulo del iterador Leer registros relacionados, Workfront Fusion realizó 28 ejecuciones. Estos 28 paquetes se seguirán procesando en todo el escenario a menos que se añada un agregador para cerrar el bucle.
