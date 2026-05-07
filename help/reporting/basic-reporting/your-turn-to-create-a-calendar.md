---
title: 'Actividad: crear un informe de calendario'
description: Instrucciones paso a paso sobre cómo crear un calendario de clientes que muestre las tareas y problemas incompletos.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
last-substantial-update: '2025-06-23T00:00:00.000Z'
thumbnail: your-turn-to-create-a-calendar.png
jira: KT-10026
exl-id: 74d57f1a-c6c5-49e0-9529-2e2deb2f273e
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
subfeature_v2:
  - id: c6584858-4838-4ce3-ab7f-7292f37179f4
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T14:16:18.343Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 81%

---

# Actividad: crear un informe de calendario

Confeccione un calendario de clientes llamado “Mi trabajo incompleto”.

Incluya un grupo de calendario llamado “Tareas incompletas” que muestre todas las tareas incompletas asignadas que tiene asignadas en Proyectos actuales.

Seleccione el color rojo para estos elementos.

Incluya otro grupo de calendario llamado “Problemas incompletos” que muestre todos los problemas incompletos que tiene asignados en Proyectos actuales. Seleccione el color azul para estos elementos.

## Respuesta

1. Vaya al área Calendarios en el menú principal.
1. Haga clic en el botón Nuevo calendario y llame al calendario “Mi trabajo incompleto”.
1. Haga clic en el botón Agregar al calendario y, a continuación, en Agregar elementos avanzados.
1. En la ventana emergente Agregar elementos al calendario, nombre el grupo “Tareas incompletas”.
1. Seleccione rojo como color.
1. Cambie el campo Fecha a Fechas planificadas.
1. Establezca En el calendario, el campo Mostrar en Solo fecha de finalización.
1. Establezca el campo Cambiar a fechas reales cuando estén disponibles en No.
1. En la sección ¿Qué desea agregar al calendario?, , seleccione Tareas. A continuación, haga clic en el botón Agregar tareas.
1. Agregue tres reglas de filtro:

   * Proyecto > Estado Es Igual A > Igual > Actual
   * Usuarios de la asignación > ID > Igual > $$USER.ID
   * Tarea > Completada > Igual > Falso

1. Haga clic en Guardar.

   ![Imagen de la pantalla para agregar elementos a un calendario](assets/calendar-activity-1.png)

1. Cree una segunda agrupación haciendo clic en Agregar al calendario y, a continuación, en Agregar elementos avanzados.
1. En la ventana emergente Agregar elementos al calendario, llame al grupo “Problemas incompletos”.
1. Seleccione azul como color.
1. Cambie el campo Fecha a Fechas planificadas.
1. Establezca En el calendario, el campo Mostrar en Solo fecha de finalización.
1. Establezca el campo Cambiar a fechas reales cuando estén disponibles en No.
1. En la sección ¿Qué desea agregar al calendario?, , seleccione Problemas. A continuación, haga clic en el botón Agregar problemas.
1. Agregue las tres reglas de filtro siguientes:

   * Proyecto > Estado Es Igual A > Igual > Actual
   * Usuarios de la asignación > ID > Igual > $$USER.ID
   * Problema > Completado > Igual > Falso

1. Haga clic en Guardar.

   ![Imagen de la pantalla para agregar elementos a un calendario](assets/calendar-activity-2.png)

Como ha utilizado $$USER.ID en los filtros, puede compartir este calendario con otros y verán sus propias tareas y problemas incompletos.
