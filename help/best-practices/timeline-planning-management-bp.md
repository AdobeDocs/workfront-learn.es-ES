---
title: 'Práctica recomendada: planificación y administración de la cronología'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de cronologías de proyectos en Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
jira: KT-10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '1110'
ht-degree: 100%

---

# Práctica recomendada: planificación y administración de la cronología

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El punto &quot;¿Por qué estas son prácticas recomendadas?&quot; se encuentra después de la lista de alto nivel, proporciona mayores detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., cuya implementación se debe considerar al trabajar con Workfront.

</br>
</br>

## Prácticas recomendadas de planificación y administración de cronología

* Todos los proyectos completados deben tener un estado que refleje que se han completado.

* Al copiar un proyecto, establezca el estado del nuevo proyecto en Planificación.

* Haga que los usuarios registren el tiempo real empleado en las tareas para que pueda comparar las horas reales con las horas planificadas.

* Utilice duraciones de tareas y predecesores cuando sea posible para crear y actualizar la cronología del proyecto, en lugar de seleccionar fechas de inicio y finalización específicas.

* Pida a los usuarios que actualicen los estados de sus tareas, el porcentaje completado y las horas reales cada día (o en una programación establecida cada semana).

* Establezca el estado del proyecto en Planificación al actualizar el plan del proyecto para evitar que las notificaciones se envíen automáticamente a medida que se realicen cambios.

* Quite del equipo del proyecto a los usuarios que no tengan trabajo asignado en él.

* Coloque las métricas del proyecto en la parte superior del menú del panel izquierdo para los usuarios que utilizan Workfront principalmente para ver los datos.


</br>
</br>


## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Todos los proyectos completados deben tener un estado que refleje que se han completado.


**A continuación se explica por qué**

Asegurarse de que todos los proyectos completados tengan un estado Completado (o equivalente) mantiene la instancia de Workfront limpia y actualizada. Al mantener los estados del proyecto actualizados y cerrarlos, los usuarios pueden saber fácilmente qué trabajo ya se ha realizado para que puedan centrarse en prioridades activas. También garantiza que los datos de los informes sobre proyectos, tareas, recursos, etc. sean precisos.


</br>
</br>

**Práctica recomendada**

Al copiar un proyecto, establezca el estado del nuevo proyecto en Planificación.

**A continuación se explica por qué**

El estado de Planificación (o un equivalente) impide que las notificaciones de Workfront sobre asignaciones, cambios en la cronología, etc. se publiquen antes de que el proyecto esté listo. Al copiar un proyecto, aparece un cuadro de diálogo con opciones de proyecto; cambie el estado aquí, mientras ajusta otras opciones para que los datos no se copien del proyecto original a la versión copiada.

</br>
</br>

**Práctica recomendada**

Haga que los usuarios registren el tiempo real empleado en las tareas para que pueda comparar las horas reales con las horas planificadas.


**A continuación se explica por qué**

Saber cuánto tarda el trabajo de las tareas significa que puede actualizar las plantillas de proyecto para una mejor precisión en la planificación de futuros proyectos. También significa que las estimaciones de recursos, mediante las herramientas de administración de recursos de Workfront, son más precisas.

</br>
</br>

**Práctica recomendada**

Utilice duraciones de tareas y predecesores cuando sea posible para crear y actualizar la cronología del proyecto, en lugar de seleccionar fechas de inicio y finalización específicas.

**A continuación se explica por qué**

El uso de duraciones y predecesores junto con restricciones flexibles de tareas (lo antes posible y lo más tarde posible) permite realizar cambios automáticos de fechas de cronología que se “propagan en cascada” a través del plan del proyecto. Por ejemplo, cuando la duración de una tarea aumenta en un día, eso cambia la fecha planificada de finalización de la tarea, lo que a su vez cambia las fechas de finalización de las tareas siguientes.

Al seleccionar fechas de inicio y de finalización específicas para las tareas, la restricción de tareas cambia a una que “bloquea” la fecha (debe comenzar, debe terminar, fechas fijas), lo que significa que debe realizar algunas actualizaciones de fechas de la cronología manualmente.

</br>
</br>


**Práctica recomendada**

Pida a los usuarios que actualicen los estados de sus tareas, el porcentaje completado y las horas reales cada día (o en una programación establecida cada semana).

**A continuación se explica por qué**

Los informes de Workfront solo son tan precisos como los datos introducidos en Workfront. Cuando la información que indica el progreso del trabajo (como el estado y el porcentaje completado) no se actualiza con regularidad, los informes que muestran el progreso del trabajo no serán precisos. La actualización diaria proporciona la mejor precisión en los datos de la creación de informes en tiempo real.


El estado de la tarea también sirve para informar a los usuarios de cuándo se ha completado el trabajo anterior y sus nuevas tareas pueden comenzar. Cuando el estado de la tarea no cambia para reflejar el progreso real en el elemento de trabajo, Workfront no puede enviar las notificaciones adecuadas.

</br>
</br>

**Práctica recomendada**

Establezca el estado del proyecto en Planificación al actualizar el plan del proyecto para evitar que las notificaciones se envíen automáticamente a medida que se realicen cambios.

**A continuación se explica por qué**

Los cambios en el plan del proyecto pueden generar múltiples notificaciones al modificarse las asignaciones de tareas, las fechas de inicio y finalización previstas y otro tipo de configuración. Esto puede resultar molesto para los usuarios y causar confusión acerca de las asignaciones correctas, los plazos, etc.

El estado Planificación indica a Workfront que no envíe notificaciones acerca del proyecto a los integrantes del equipo (usuarios asignados a tareas/problemas u otras personas con acceso) porque el plan aún se está desarrollando o simplemente aún no está listo para su lanzamiento. Una vez completados los cambios, devuelva el estado del proyecto a Actual y se enviarán las notificaciones. Seguir este proceso minimiza la cantidad de notificaciones que reciben los usuarios.

</br>
</br>

**Práctica recomendada**

Quite del equipo del proyecto a los usuarios que no tengan trabajo asignado en él.


**A continuación se explica por qué**

Cuando asigna a alguien una tarea o problema en un proyecto, el usuario se añade a la lista del equipo en las secciones Programación y Personas. Sin embargo, permanece en ella aunque lo haya eliminado de la asignación. Esto podría causar confusión para el usuario porque, como parte del equipo, recibe notificaciones sobre la actividad y ve el proyecto en la lista Proyectos en los que estoy.


Además, los integrantes del equipo del proyecto obtienen permisos para él y sus tareas, problemas y documentos. Esto puede hacer que los usuarios tengan acceso a elementos de Workfront que no necesitan o que no deberían tener.

</br>
</br>

**Práctica recomendada**

Coloque las métricas del proyecto en la parte superior del menú del panel izquierdo para los usuarios que utilizan Workfront principalmente para ver los datos.

**A continuación se explica por qué**

A la mayoría de los líderes, ejecutivos y otros usuarios que no administran proyectos o realizan asignaciones de tareas agradecerían ver este nivel de métricas cuando abren un proyecto por primera vez. Utilice una plantilla de diseño para mover Métricas de proyecto a la parte superior del menú del panel izquierdo de una página para que los usuarios puedan acceder a ella de forma más visible y sencilla.
