---
title: Exploración de las cronologías de proyectos en Workfront
description: Aprenda a asignar tareas, utilizar diagramas de Gantt y las funciones de ruta crítica, supervisar proyectos mediante vistas, programar tareas de forma eficaz y aplicar restricciones para una planificación del proyecto óptima.
activity: use
feature: Work Management
thumbnail: 335213.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: '2024-11-01T00:00:00.000Z'
recommendations: noDisplay,catalog
jira: KT-8953
exl-id: ba993197-9f84-4fc0-86cc-cf849c889f56
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T14:48:54.364Z'
source-git-commit: f0f541bf3fd6db69e6d813cf81456a5df6848d49
workflow-type: tm+mt
source-wordcount: 643
ht-degree: 9%

---

# Exploración de las cronologías de proyectos en Workfront

Lo que aprenderá:

* Obtenga información general sobre la planificación y administración de proyectos con Workfront. Aprenda cómo las tareas principales agrupan varias subtareas, que se asignan a roles de trabajo y, posteriormente, a usuarios con las habilidades necesarias. Las tareas predecesoras indican relaciones secuenciales entre tareas, mientras que las tareas sin predecesoras se pueden realizar en paralelo. El gráfico Gantt ofrece una cronología visual y la función Ruta crítica resalta las tareas que podrían retrasar el proyecto si se retrasan.
* Diferentes vistas en Workfront, como la vista estándar para la planificación y la vista de estado para la monitorización del progreso, que incluye indicadores de progreso, comentarios, documentos, problemas, aprobaciones, rutas críticas e hitos. Se puede realizar un seguimiento de la actividad reciente para ver actualizaciones y notas.
* La programación se puede realizar desde una fecha de inicio o de finalización, y Workfront calcula las fechas correspondientes en función de las duraciones de las tareas y sus predecesoras. El vídeo recomienda programar desde una fecha de inicio las fechas de finalización esenciales para permitir cierto margen de demora. También se tratan las delimitaciones de tareas, como &quot;lo antes posible&quot; y &quot;lo más tarde posible&quot;, lo que muestra cómo afectan a la programación de tareas. Se pueden crear vistas personalizadas para mostrar las delimitaciones de las tareas.

>[!VIDEO](https://video.tv.adobe.com/v/3435838/?captions=spa&quality=12&learn=on&enablevpops=1)

>[!IMPORTANT]
>
>Para obtener una explicación más completa de los tipos de duración y las restricciones de tareas, consulte [Explicación y administración de los tipos de duración y las restricciones de tareas](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md).

## Principales conclusiones

* **Administración y asignación de tareas:** Las tareas principales agrupan varias subtareas, que se asignan a roles de trabajo y, posteriormente, a usuarios con las habilidades necesarias. Las predecesoras indican relaciones secuenciales, mientras que las tareas sin predecesoras se pueden realizar en paralelo. palo de golf
* **Diagrama de Gantt y ruta crítica:** El gráfico de Gantt proporciona una escala de tiempo visual del proyecto y la característica Ruta crítica resalta las tareas que podrían retrasar el proyecto si se retrasan. palo de golf
* **Vistas y supervisión:** Las distintas vistas de Workfront, como la vista estándar para la planificación y la vista de estado para la supervisión, incluyen indicadores de progreso, comentarios, documentos, problemas, aprobaciones, rutas críticas y hitos. También se puede realizar un seguimiento de la actividad reciente. palo de golf
* **Opciones de programación:** los proyectos se pueden programar desde una fecha de inicio o de finalización, y Workfront calcula las fechas correspondientes en función de las duraciones de las tareas y sus predecesoras. Se recomienda programar desde una fecha de inicio en las fechas de finalización críticas para permitir cierto margen de demora. palo de golf
* **Restricciones de tarea:** Las restricciones de tarea como &quot;lo antes posible&quot; y &quot;lo más tarde posible&quot; afectan la programación de tareas. Cambiar el modo de programación después de la creación del proyecto puede afectar a las restricciones de tareas y las fechas planificadas. Se pueden crear vistas personalizadas para mostrar las restricciones de tareas. palo de golf


## Para cambiar o no cambiar fechas en las escalas de tiempo del &#x200B;proyecto...

| PROS (Cambio de fechas) | CONTRAS (cambio de fechas) | PROS (Sin cambiar las fechas) | CONTRAS (no cambia las fechas) |
|---------------------------|---------------------------|---------------------------|---------------------------|
| <ul><li>Reduce el estrés y proporciona expectativas actualizadas para los usuarios - &quot;_Los creativos no sabrían qué es real_&quot;</li><li>Asignación precisa de recursos, especialmente en el Distribuidor de cargas de trabajo</li><li>Use los informes de entradas de diario (o la duración del proyecto) para llamar a los cambios de fecha</li><li>Uso de la condición para mostrar si el proyecto está fuera de ámbito</li><li>Puede agregar un formulario personalizado (o usar problemas) para rastrear cambios: por qué se insertó, quién lo insertó, cuánto tiempo</li></ul> | <ul></li><li>Datos engañosos, ya que los informes no reflejan el estado verdadero</li><li>Percepción falsa del progreso - ilusión de que todo está en camino&#x200B;</li><li>Fomente una cultura de siempre retroceder en los plazos en lugar de abordar las causas profundas&#x200B;</li><li>Pérdida de confianza de las partes interesadas / percepción del equipo para cumplir los plazos </li></ul> | <ul></li><li>Representación precisa de la cronología del proyecto: los datos se pueden utilizar para realizar análisis y contar una historia clara de lo que ha sucedido</li><li>Opción para cambiar la duración o agregar el retardo al predecesor en su lugar</li><li>Identifique fácilmente las mejoras del proceso para la futura planificación de proyectos/gestión de riesgos&#x200B;</li><li>Opción para aprovechar las líneas de base para capturar el plan de proyecto original y utilizarlo como comparación</li><li>Si no tienes a la gente para hacerlo, y hacerlo por todo, no lo hagas&#x200B;</li></ul> | <ul></li><li>Confusión y/o frustración del usuario: abundancia de tareas &quot;tardías&quot; a pesar del hecho de que acaba de ser notificado</li><li>Los recursos se asignaron efectivamente para asignarlos al plan original, pero ahora están sobrecargados de trabajo demorado</li><li>La cronología del proyecto no se puede usar para comunicar claramente las actualizaciones a las partes interesadas</li></ul> |


## Tutoriales recomendados sobre este tema

* [Seguimiento del progreso mediante porcentaje completado y estado de progreso](/help/manage-work/project-timelines/track-work-progress-from-the-project-timeline.md)
* [Comprender los tipos de fechas y el estado de progreso](/help/manage-work/project-timelines/understand-task-dates-and-progress-status.md)
* [Tipos de duración maestros y restricciones de tareas](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md)

