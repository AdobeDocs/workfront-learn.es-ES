---
title: 'Práctica recomendada: planificación y administración de la cronología'
description: Explore las recomendaciones sobre prácticas recomendadas de los expertos de Adobe Workfront acerca de la configuración, administración y uso de las escalas de tiempo de los proyectos en Workfront.
feature: Get Started with Workfront
role: Admin, Leader, User
level: Beginner
jira: KT-10929
exl-id: 8c18746d-e23a-44d0-b1e3-ebf5ba8d022f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Práctica recomendada: planificación y administración de la cronología

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de planificación y administración del calendario

* Todos los proyectos completados deben tener un estado que indique que se han completado.

* Al copiar un proyecto, establezca el estado del nuevo proyecto en Planificación.

* Haga que los usuarios registren el tiempo real empleado en las tareas para que pueda comparar las horas reales con las planificadas.

* Utilice duraciones de tareas y predecesoras cuando sea posible para generar y actualizar una escala de tiempo de un proyecto, en lugar de seleccionar fechas específicas de inicio y finalización.

* Pida a los usuarios que actualicen sus estados de tareas, porcentaje completado y horas reales cada día (o en una programación establecida cada semana).

* Configure el estado del proyecto a Planificación cuando actualice el plan del proyecto para evitar que las notificaciones se envíen automáticamente a medida que se realicen cambios.

* Elimine usuarios del equipo del proyecto que no tengan asignado un trabajo en el proyecto.

* Coloque las métricas del proyecto en la parte superior del menú del panel izquierdo para los usuarios que utilizan Workfront principalmente para ver datos.


</br>
</br>


## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Todos los proyectos completados deben tener un estado que indique que se han completado.


**He aquí la razón**

Garantizar que todos los proyectos completados tengan un estado completo (o equivalente) mantiene la instancia de Workfront limpia y actualizada. Si mantienen los estados de los proyectos actualizados y los cierran, los usuarios pueden saber fácilmente qué trabajo ya se ha realizado para poder centrarse en las prioridades activas. También garantiza que los datos de los informes sobre proyectos, tareas, recursos, etc., sean precisos.


</br>
</br>

**Práctica recomendada**

Al copiar un proyecto, establezca el estado del nuevo proyecto en Planificación.

**He aquí la razón**

El estado de Planning (o un equivalente) evita que las notificaciones de Workfront sobre asignaciones, cambios de escala de tiempo, etc., salgan antes de que el proyecto esté listo. Al copiar un proyecto, aparecerá un cuadro de diálogo con opciones de proyecto; cambie el estado aquí, mientras ajusta otras opciones para que los datos no se copien del proyecto original a la versión copiada.

</br>
</br>

**Práctica recomendada**

Haga que los usuarios registren el tiempo real empleado en las tareas para que pueda comparar las horas reales con las planificadas.


**He aquí la razón**

Saber cuánto tiempo tarda el trabajo de las tareas significa que puede actualizar las plantillas de proyecto para mejorar la precisión en la planificación de proyectos futuros. También significa que las estimaciones de recursos, que utilizan las herramientas de administración de recursos de Workfront, son más precisas.

</br>
</br>

**Práctica recomendada**

Utilice duraciones de tareas y predecesoras cuando sea posible para generar y actualizar una escala de tiempo de un proyecto, en lugar de seleccionar fechas específicas de inicio y finalización.

**He aquí la razón**

El uso de duraciones y predecesoras junto con delimitaciones flexibles de tareas (Lo antes posible y Lo más tarde posible) permite realizar cambios automáticos de fechas de escala de tiempo que se aplican en cascada en el plan del proyecto. Por ejemplo, cuando la duración de una tarea aumenta en un día, esto cambia la fecha planificada de finalización de la tarea, lo que a su vez cambia las fechas de finalización de las siguientes tareas.

Al seleccionar fechas de inicio y finalización específicas para las tareas, la delimitación de tareas cambia a una que &quot;bloquea&quot; la fecha (Debe comenzar el, Debe finalizar el, Fechas fijas), lo que significa que debe realizar manualmente algunas actualizaciones de fechas de escala de tiempo.

</br>
</br>


**Práctica recomendada**

Pida a los usuarios que actualicen sus estados de tareas, porcentaje completado y horas reales cada día (o en una programación establecida cada semana).

**He aquí la razón**

Los informes de Workfront solo son tan precisos como los datos introducidos en Workfront. Cuando la información que indica el progreso del trabajo (como el estado y el porcentaje completado) no se actualiza con regularidad, los informes que muestran el progreso del trabajo no serán precisos. La actualización diaria proporciona la buena máxima precisión en los datos de informes en tiempo real.


El estado de la tarea también se utiliza para informar a los usuarios de cuándo se ha completado el trabajo anterior y de cuándo pueden comenzar las nuevas tareas. Cuando el estado de la tarea no cambia para reflejar el progreso real en el elemento de trabajo, Workfront no puede enviar las notificaciones adecuadas.

</br>
</br>

**Práctica recomendada**

Configure el estado del proyecto a Planificación cuando actualice el plan del proyecto para evitar que las notificaciones se envíen automáticamente a medida que se realicen cambios.

**He aquí la razón**

Los cambios en el plan del proyecto pueden generar varias notificaciones a medida que se modifican las asignaciones de tareas, las fechas planificadas de inicio y finalización y otras opciones de configuración. Esto puede resultar molesto para los usuarios y causar confusión sobre las asignaciones adecuadas, los plazos, etc.

El estado de Planificación indica a Workfront que no envíe notificaciones sobre el proyecto a los miembros del equipo del proyecto (usuarios asignados a tareas/problemas u otros con acceso al proyecto) porque el plan del proyecto aún se está desarrollando o el proyecto aún no está listo para ejecutarse. Una vez completados los cambios, vuelva a cambiar el estado del proyecto a Actual y se enviarán las notificaciones. Seguir este proceso ayuda a minimizar la cantidad de notificaciones que reciben los usuarios.

</br>
</br>

**Práctica recomendada**

Elimine usuarios del equipo del proyecto que no tengan asignado un trabajo en el proyecto.


**He aquí la razón**

Cuando asigna a alguien una tarea o un problema en un proyecto, esto agrega al usuario a la lista del equipo del proyecto en las secciones Programación y Personas del proyecto. Sin embargo, permanecen en la lista de equipos del proyecto aunque los haya eliminado de la asignación. Esto podría causar confusión al usuario, ya que, como parte del equipo del proyecto, recibe notificaciones sobre la actividad en el proyecto y ve el proyecto en la lista Proyectos en los que participo.


Además, los miembros del equipo del proyecto obtienen permisos para el proyecto y sus tareas, problemas y documentos. Esto puede dar como resultado que los usuarios tengan acceso a elementos en Workfront que no necesitan o no deberían tener.

</br>
</br>

**Práctica recomendada**

Coloque las métricas del proyecto en la parte superior del menú del panel izquierdo para los usuarios que utilizan Workfront principalmente para ver datos.

**He aquí la razón**

La mayoría de los líderes, ejecutivos y otros usuarios que no administran proyectos ni cumplen asignaciones de tareas agradecerían ver este nivel de métricas del proyecto la primera vez que abren un proyecto. Utilice una plantilla de diseño para mover las métricas del proyecto al principio del menú del panel izquierdo de una página de proyecto a fin de que sean más visibles y fáciles de acceder para los usuarios.
