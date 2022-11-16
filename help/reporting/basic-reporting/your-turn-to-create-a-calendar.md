---
title: Su turno para crear un calendario
description: Obtenga información sobre cómo crear un calendario de clientes que muestre las tareas y los problemas incompletos.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
thumbnail: your-turn-to-create-a-calendar.png
kt: 10026
exl-id: 74d57f1a-c6c5-49e0-9529-2e2deb2f273e
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# Su turno para crear un calendario

En esta actividad obtendrá experiencia creando su propio calendario.

## Actividad: Crear un calendario

Cree un calendario de clientes llamado &quot;Mi trabajo incompleto&quot;.

Incluya un grupo de calendario llamado &quot;Tareas incompletas&quot; que muestre todas las tareas incompletas asignadas a usted en Proyectos actuales.

Seleccione rojo como color para estos elementos.

Incluya otro grupo de calendario llamado &quot;Problemas incompletos&quot; que muestre todos los problemas incompletos asignados en proyectos actuales. Seleccione azul como color para estos elementos.

## Respuesta

1. Vaya al área Calendarios desde el menú Principal.
1. Haga clic en el botón Nuevo calendario y asigne un nombre al calendario &quot;Mi trabajo incompleto&quot;.
1. En la primera agrupación, haga clic en Agregar elementos avanzados.
1. En la ventana Agregar elementos al calendario que aparece, asigne al grupo el nombre &quot;Tareas incompletas&quot;.
1. Seleccione rojo como color.
1. Cambie el campo Fecha a Fechas planificadas.
1. Establezca el campo En el calendario, mostrar en Solo fecha de finalización.
1. Establezca el campo Switch to real dates when available en No.

   ![Imagen de la pantalla para agregar elementos a un calendario](assets/calendar-activity-1.png)

1. En ¿Qué desea agregar al calendario? , seleccione Tareas.
1. Añadir tres reglas de filtro:

   * Proyecto > Estado Es Igual A > Igual > Actual
   * Usuarios de asignación > ID > Igual > $$USER.ID
   * Tarea > Completar > Igual > Falso

1. Haga clic en Guardar.

   ![Imagen de la pantalla para agregar elementos a un calendario](assets/calendar-activity-2.png)

1. Cree una segunda agrupación haciendo clic en Agregar al calendario.
1. En esta agrupación, haga clic en Agregar elementos avanzados.
1. En la ventana Agregar elementos al calendario que aparece, asigne al grupo el nombre &quot;Problemas incompletos&quot;.
1. Seleccione azul como color.
1. Cambie el campo Fecha a Fechas planificadas.
1. Establezca el campo En el calendario, mostrar en Solo fecha de finalización.
1. Establezca el campo Switch to real dates when available en No.
1. En ¿Qué desea agregar al calendario? , seleccione Problemas.
1. Agregue las tres reglas de filtro siguientes:

   * Proyecto > Estado Es Igual A > Igual > Actual
   * Usuarios de asignación > ID > Igual > $$USER.ID
   * Problema > Se completó > Igual > Falso

1. Haga clic en Guardar.

   ![Imagen de la pantalla para agregar elementos a un calendario](assets/calendar-activity-3.png)

Como ha utilizado $$USER.ID en los filtros, puede compartir este calendario con otros y verán sus propias tareas y problemas incompletos.
