---
title: Agregación
description: Aprenda a acumular varios paquetes de información en un solo valor.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Agregación

Aprenda a acumular varios paquetes de información en un solo valor.

## Resumen del ejercicio

Utilizando el escenario &quot;Introducción a la iteración&quot; creado en el último ejercicio, agregue las horas planificadas en cada tarea de trabajo del proyecto y envíese un correo electrónico con esa información.

![Imagen de agregación 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## Pasos a seguir

**Añada un filtro y SUME las horas planificadas.**

1. Clone el escenario &quot;Introducción a la iteración&quot; creado en el ejercicio anterior y asígnele el nombre &quot;Introducción a la agregación&quot;.
1. Agregue un filtro entre el módulo Tareas del proyecto de lectura y el módulo Contar el número de tareas. Asigne un nombre al filtro &quot;Solo tareas de trabajo&quot;.
1. Establezca la condición en Número de elementos secundarios [Operador numérico: Igual a] 0.

   ![Imagen de agregación 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. Después del módulo Random Math, añada un módulo de la herramienta Numeric Aggregator.
1. Establezca el módulo de origen en Leer tareas del proyecto.
1. Establezca la función Aggregate en SUM.
1. Establezca el Valor en el campo Trabajo del módulo Leer tareas del proyecto.
1. Cambie el nombre de este módulo &quot;SUMA de todas las horas planificadas para tareas&quot;.

   ![Imagen de agregación 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **Observe la sombra que muestra que la agregación finaliza la iteración.**

   ![Imagen de agregación 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **Envíe un correo electrónico con las horas agregadas.**

1. Agregue un módulo Enviar un correo electrónico desde la aplicación Correo electrónico, después del agregador numérico.
1. Envíese el correo electrónico a usted mismo.
1. La línea de asunto es &quot;Detalles del proyecto&quot;
1. En el campo Contenido, ponga &quot;Hay un proyecto llamado [nombre del proyecto] que tiene un número total de [resultado] horas planificadas&quot;. El &quot;[nombre del proyecto]&quot; se toma del módulo Leer un registro y &quot;[resultado]&quot; se toma del módulo del agregador.

   ![Imagen de agregación 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. Guardar y ejecutar una vez. Busque el correo electrónico en su bandeja de entrada.

Dentro de la iteración, se puede acceder a los paquetes individuales. Pero fuera de la iteración, en el módulo Enviar un correo electrónico, solo se puede acceder a los campos agregados.
