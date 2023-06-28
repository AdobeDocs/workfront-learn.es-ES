---
title: Su turno para crear un calendario
description: Aprenda a crear un calendario de clientes que muestre las tareas y los problemas incompletos.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
thumbnail: your-turn-to-create-a-calendar.png
jira: KT-10026
exl-id: 74d57f1a-c6c5-49e0-9529-2e2deb2f273e
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# Su turno para crear un calendario

En esta actividad obtendrá experiencia práctica creando su propio calendario.

## Actividad: crear un calendario

Cree un calendario de clientes llamado &quot;Mi trabajo incompleto&quot;.

Incluya un grupo de calendario llamado &quot;Tareas incompletas&quot; que muestre todas las tareas incompletas que se le han asignado en Proyectos actuales.

Seleccione rojo como color para estos elementos.

Incluya otro grupo de calendario llamado &quot;Problemas incompletos&quot; que muestre todos los problemas incompletos asignados a usted en Proyectos actuales. Seleccione azul como color para estos elementos.

## Respuesta

1. Vaya al área Calendarios del menú Principal.
1. Haga clic en el botón Nuevo calendario y asigne al calendario el nombre &quot;Mi trabajo incompleto&quot;.
1. En la primera agrupación, haga clic en Agregar elementos avanzados.
1. En la ventana Agregar elementos al calendario que aparece, asigne un nombre al grupo &quot;Tareas incompletas&quot;.
1. Seleccione rojo como color.
1. Cambie el campo Fecha a Fechas planificadas.
1. Establezca el campo Mostrar en el calendario como Solo fecha de finalización.
1. Establezca el campo Cambiar a fechas reales cuando esté disponible en No.

   ![Imagen de la pantalla para agregar elementos a un calendario](assets/calendar-activity-1.png)

1. En el cuadro ¿Qué desea agregar al calendario? , seleccione Tareas.
1. Añada tres reglas de filtro:

   * Proyecto > Estado es igual a > Igual a > Actual
   * Asignación Usuarios > ID > Igual a > $$USER.ID
   * Tarea > Completar > Igual > Falso

1. Haga clic en Guardar.

   ![Imagen de la pantalla para agregar elementos a un calendario](assets/calendar-activity-2.png)

1. Cree una segunda agrupación haciendo clic en Agregar al calendario.
1. En esta agrupación, haga clic en Agregar elementos avanzados.
1. En la ventana Agregar elementos al calendario que aparece, asigne un nombre al grupo &quot;Problemas incompletos&quot;.
1. Seleccione azul como color.
1. Cambie el campo Fecha a Fechas planificadas.
1. Establezca el campo Mostrar en el calendario como Solo fecha de finalización.
1. Establezca el campo Cambiar a fechas reales cuando esté disponible en No.
1. En el cuadro ¿Qué desea agregar al calendario? , seleccione Problemas.
1. Añada las tres reglas de filtro siguientes:

   * Proyecto > Estado es igual a > Igual a > Actual
   * Asignación Usuarios > ID > Igual a > $$USER.ID
   * Problema > Completado > Igual > Falso

1. Haga clic en Guardar.

   ![Imagen de la pantalla para agregar elementos a un calendario](assets/calendar-activity-3.png)

Debido a que ha utilizado $$USER.ID en los filtros, puede compartir este calendario con otros usuarios y estos verán sus propias tareas y problemas incompletos.
