---
title: 'Práctica recomendada: planificación y administración de cronogramas'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de cronologías de proyectos en Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
kt: 10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Práctica recomendada: planificación y administración de cronogramas

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las mejores prácticas son directrices que representan un curso de acción eficaz y eficiente; sean adoptados fácilmente por usted y los usuarios de su empresa; y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, tenga en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco para ayudarle a guiar la configuración y el uso del sistema Workfront.

## Navegar por esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

La pregunta &quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de planificación y administración de cronogramas

* Todos los proyectos completados deben tener un estado que refleje que se han completado.

* Al copiar un proyecto, establezca el estado del nuevo proyecto en Planificación.

* Haga que los usuarios registren el tiempo real empleado en las tareas para que pueda comparar las horas reales con las horas planificadas.

* Utilice duraciones de tareas y predecesores cuando sea posible para crear y actualizar una cronología de proyecto, en lugar de seleccionar fechas de inicio y finalización específicas.

* Pida a los usuarios que actualicen sus estados de tarea, el porcentaje completado y las horas reales cada día (o en una programación establecida cada semana).

* Establezca el estado del proyecto en Planning al actualizar el plan del proyecto para evitar que las notificaciones se envíen automáticamente a medida que se realicen cambios.

* Elimine usuarios del equipo del proyecto a los que no se haya asignado trabajo en el proyecto.

* Coloque las métricas del proyecto en la parte superior del menú del panel izquierdo para los usuarios que utilicen Workfront principalmente para ver datos.


</br>
</br>


## ¿Por qué estas prácticas recomendadas?

**Práctica recomendada**

Todos los proyectos completados deben tener un estado que refleje que se han completado.


**He aquí por qué**

Asegurarse de que todos los proyectos completados tengan un estado Complete (o equivalente) mantiene la instancia de Workfront limpia y actualizada. Al mantener los estados del proyecto actualizados y cerrarlos, los usuarios pueden saber fácilmente qué trabajo ya se ha realizado para que puedan centrarse en prioridades activas. También garantiza que los datos de los informes sobre proyectos, tareas, recursos, etc. sean precisos.


</br>
</br>

**Práctica recomendada**

Al copiar un proyecto, establezca el estado del nuevo proyecto en Planificación.

**He aquí por qué**

El estado de Planning (o un equivalente) impide que las notificaciones de Workfront sobre asignaciones, cambios en la cronología, etc. se publiquen antes de que el proyecto esté listo. Al copiar un proyecto, aparece un cuadro de diálogo con opciones de proyecto; cambie el estado aquí, mientras ajusta otras opciones para que los datos no se copien del proyecto original a la versión copiada.

</br>
</br>

**Práctica recomendada**

Haga que los usuarios registren el tiempo real empleado en las tareas para que pueda comparar las horas reales con las horas planificadas.


**He aquí por qué**

Saber cuánto tarda el trabajo de las tareas significa que puede actualizar las plantillas de proyecto para una mejor precisión en la planificación de futuros proyectos. También significa que las estimaciones de recursos, mediante las herramientas de administración de recursos de Workfront, son más precisas.

</br>
</br>

**Práctica recomendada**

Utilice duraciones de tareas y predecesores cuando sea posible para crear y actualizar una cronología de proyecto, en lugar de seleccionar fechas de inicio y finalización específicas.

**He aquí por qué**

El uso de duraciones y predecesores junto con restricciones flexibles de tareas (lo antes posible y lo más tarde posible) permite realizar cambios automáticos de fechas de cronología que se &quot;propagan&quot; en cascada a través del plan del proyecto. Por ejemplo, cuando la duración de una tarea aumenta en un día, eso cambia la fecha de finalización prevista de la tarea, lo que a su vez cambia las fechas de finalización de las tareas siguientes.

Al seleccionar fechas de inicio y finalización específicas para las tareas, la restricción de tareas cambia a una que &quot;bloquea&quot; la fecha (debe comenzar el, debe terminar el, fechas fijas), lo que significa que debe realizar algunas actualizaciones de fechas de la cronología manualmente.

</br>
</br>


**Práctica recomendada**

Pida a los usuarios que actualicen sus estados de tarea, el porcentaje completado y las horas reales cada día (o en una programación establecida cada semana).

**He aquí por qué**

Los informes de Workfront solo son tan precisos como los datos introducidos en Workfront. Cuando la información que indica el progreso del trabajo (como el estado y el porcentaje completado) no se actualiza con regularidad, los informes que muestran el progreso del trabajo no serán precisos. La actualización diaria proporciona una buena precisión en los datos de los informes en tiempo real.


El estado de la tarea también se utiliza para informar a los usuarios de cuándo se ha completado el trabajo anterior y sus nuevas tareas pueden comenzar. Cuando el estado de la tarea no cambia para reflejar el progreso real en el elemento de trabajo, Workfront no puede enviar las notificaciones adecuadas.

</br>
</br>

**Práctica recomendada**

Establezca el estado del proyecto en Planning al actualizar el plan del proyecto para evitar que las notificaciones se envíen automáticamente a medida que se realicen cambios.

**He aquí por qué**

Los cambios en el plan del proyecto pueden generar varias notificaciones a medida que se cambian las asignaciones de tareas, las fechas de inicio y finalización planificadas y otros ajustes. Esto puede ser perjudicial para los usuarios y causar confusión sobre asignaciones adecuadas, plazos, etc.

El estado de Planning indica a Workfront que no envíe notificaciones sobre el proyecto a los miembros del equipo del proyecto (usuarios asignados a tareas o problemas u otras personas con acceso al proyecto) porque el plan del proyecto aún se está desarrollando o simplemente no está listo para su lanzamiento aún. Una vez completados los cambios, vuelva a cambiar el estado del proyecto a Actual y se envíen las notificaciones. Seguir este proceso ayuda a minimizar la cantidad de notificaciones que los usuarios reciben.

</br>
</br>

**Práctica recomendada**

Elimine usuarios del equipo del proyecto a los que no se haya asignado trabajo en el proyecto.


**He aquí por qué**

Cuando se asigna a alguien una tarea o problema en un proyecto, se agrega el usuario a la lista del equipo del proyecto en las secciones Programación y personas del proyecto. Sin embargo, permanecen en la lista de equipos del proyecto aunque los haya eliminado de la asignación. Esto podría causar confusión para el usuario porque, como parte del equipo del proyecto, recibe notificaciones sobre la actividad del proyecto y ve el proyecto en la lista Proyectos en los que estoy.


Además, los miembros del equipo del proyecto obtienen permisos para el proyecto y sus tareas, problemas y documentos. Esto puede hacer que los usuarios tengan acceso a elementos de Workfront que no necesitan o que no deberían tener.

</br>
</br>

**Práctica recomendada**

Coloque las métricas del proyecto en la parte superior del menú del panel izquierdo para los usuarios que utilicen Workfront principalmente para ver datos.

**He aquí por qué**

A la mayoría de los líderes, ejecutivos y otros usuarios que no administran proyectos o realizan asignaciones de tareas les agradaría ver este nivel de métricas de proyecto cuando abren un proyecto por primera vez. Utilice una plantilla de diseño para mover Métricas de proyecto a la parte superior del menú del panel izquierdo de una página de proyecto para que los usuarios puedan acceder a ella de forma más visible y sencilla.
