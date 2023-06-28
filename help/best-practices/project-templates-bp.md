---
title: 'Práctica recomendada: plantillas de proyecto'
description: Explore las recomendaciones sobre prácticas recomendadas de los expertos de Adobe Workfront acerca de la configuración, administración y uso de plantillas de proyecto de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---

# Práctica recomendada: plantillas de proyecto

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de plantilla de proyecto

* Utilice plantillas al crear proyectos.

* Establezca una convención de nombres para las plantillas de proyecto.

* Establezca un grupo selecto de usuarios que puedan crear y actualizar plantillas de proyecto.

* Utilizar Uso compartido de proyectos en una plantilla de proyecto para conceder automáticamente acceso a los proyectos creados con esa plantilla.

* Asigne funciones o equipos de trabajo a tareas, no a individuos.

* Evite ser demasiado granular al crear tareas en una plantilla de proyecto. Limite el número de tareas de una plantilla de proyecto a las necesarias para completar el trabajo.

* Utilice la descripción de la tarea para capturar los pasos pequeños de la tarea, en lugar de desglosarla en varias tareas.

* Asegúrese de que las tareas de plantilla incluyan duraciones de tareas, horas planificadas y predecesoras.

* Preconfigure los detalles del proyecto y adjunte formularios personalizados en la plantilla.

* Revisar y actualizar periódicamente las plantillas de proyecto.

* Compruebe las plantillas para asegurarse de que tienen toda la información necesaria antes de compartirlas y de que otros usuarios empiecen a utilizarlas.

* Cuando ajuste la opción Programar desde en una plantilla, revise y actualice las restricciones de la tarea.

* Compruebe el equipo del proyecto en la plantilla y elimine los usuarios que no estén asociados al proyecto.

</br>
</br>

## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Utilice plantillas al crear proyectos.

**He aquí la razón**

Las plantillas de proyecto eliminan las conjeturas de los jefes de proyecto (y de otros que crean proyectos) sobre qué tareas debe contener un proyecto, cómo estructurar la cronología, etc. Las plantillas son la forma más eficaz de acelerar la creación de proyectos.

Es importante destacar que las plantillas proporcionan coherencia en todos los proyectos de tipos similares, de modo que las personas, los procesos y los puntos de datos se detallan de la misma manera cada vez. Incluso los proyectos con plazos de ejecución rápidos (uno o dos días) y tareas mínimas pueden beneficiarse de su creación con plantillas de proyecto.

Esta coherencia en todos los proyectos resulta en datos más precisos, que son vitales al tomar decisiones para su equipo, en su departamento y en toda la organización.

</br>
</br>

**Práctica recomendada**

Establezca una convención de nombres para las plantillas de proyecto.

**He aquí la razón**

Una nomenclatura coherente facilita la búsqueda de las plantillas. También ayuda a los jefes de proyecto y a otros usuarios que crean proyectos a seleccionar la plantilla adecuada cuando existen plantillas con nombres similares en varios equipos o departamentos.

</br>
</br>

**Práctica recomendada**

Establezca un grupo selecto de usuarios que puedan crear y actualizar plantillas de proyecto.

**He aquí la razón**

Tener plantillas de proyecto bien construidas y consistentes es clave para una buena administración del trabajo y un sistema de informes preciso. Limite el número de usuarios que pueden editar las plantillas para evitar cambios accidentales o no aprobados.

</br>
</br>

**Práctica recomendada**

Utilizar Uso compartido de proyectos en una plantilla de proyecto para conceder automáticamente acceso a los proyectos creados con esa plantilla.

**He aquí la razón**

El acceso a proyectos específicos se concede a través del propio proyecto. Si el mismo grupo de personas siempre necesita tener acceso a los proyectos creados con una plantilla específica, agréguelos en la opción Uso compartido de proyectos de la plantilla. No solo puede controlar el acceso a los proyectos en cuanto se crean, sino que también optimiza los esfuerzos de escalabilidad si los permisos deben cambiar en el futuro.

**Nota**: el uso compartido de plantillas concede acceso a la propia plantilla. Un usuario debe tener al menos permisos de visualización para realizar proyectos con la plantilla.

</br>
</br>

**Práctica recomendada**

Asigne funciones o equipos de trabajo a tareas, no a individuos.

**He aquí la razón**

Cuando un usuario individual cambie de posición o abandone la organización, deberá actualizar manualmente las plantillas de proyecto que incluyan a esa persona. Esto lleva tiempo en parte de los administradores del sistema o del grupo o en los jefes de proyecto.

Si utiliza roles o equipos en las plantillas, los cambios de plantilla no tendrán un efecto directo en las plantillas de proyecto porque a cualquier persona asignada a ese rol o a ese equipo se le podría asignar el trabajo. Esto ayuda a garantizar que el trabajo no se deslice por las grietas. Las asignaciones de funciones también facilitan la asignación de trabajo a usuarios individuales, ya que Workfront puede mostrarle una lista de personas asignadas a ese rol.

Además, las herramientas de planificación de recursos de Workfront utilizan las funciones del puesto para ayudarle a calcular los recursos necesarios y planificar el trabajo futuro.

</br>
</br>

**Práctica recomendada**

Evite ser demasiado granular al crear tareas en una plantilla de proyecto. Limite el número de tareas de una plantilla de proyecto a las necesarias para completar el trabajo.

**He aquí la razón**

Las plantillas de proyecto demasiado complicadas producen una mala experiencia para los usuarios: jefes de proyecto, jefes de recursos, integrantes del equipo y mucho más. Demasiadas tareas dificultan la administración de la cronología del proyecto, con fechas límite de tareas superpuestas y varias tareas asignadas a los mismos roles o individuos.


</br>
</br>

**Práctica recomendada**

Utilice la descripción de la tarea para capturar los pasos pequeños de la tarea, en lugar de desglosarla en varias tareas.

**He aquí la razón**

Si se asignan varias tareas de una fila al mismo rol o individuo, eso indica que esas tareas se podrían combinar. Tener demasiadas tareas asignadas a un usuario puede hacer que sienta que hay más trabajo por completar, lo que puede afectar a la adopción de Workfront.

</br>
</br>

**Práctica recomendada**

Asegúrese de que las tareas de plantilla incluyan duraciones de tareas, horas planificadas y predecesoras.

**He aquí la razón**

Estas tres cosas (duraciones, horas planificadas y predecesoras) son los componentes básicos de la cronología del proyecto. Estos son la clave para saber cuánto tiempo llevará el trabajo y cuándo debe realizarse. Duración de las herramientas de administración de recursos y horas planificadas de Workfront, además de asignaciones de funciones, para calcular la capacidad de los recursos, la disponibilidad y mucho más.

Si no está seguro de cómo estimar las duraciones o las horas planificadas por primera vez, trabaje con el equipo del proyecto para definir algunas estimaciones iniciales. Una vez que haya utilizado la plantilla, vuelva a reunirse con el equipo del proyecto para determinar dónde se podrían realizar cambios para que la plantilla sea más precisa. Si los usuarios registran el tiempo en Workfront, puede comparar las horas planificadas de un proyecto con las horas reales para ver dónde son necesarios los ajustes.


</br>
</br>

**Práctica recomendada**

Preconfigure los detalles del proyecto y adjunte formularios personalizados en la plantilla.

**He aquí la razón**

Asegúrese de que la información que es estándar en todos los proyectos se rellene en la plantilla de proyecto. Esto no solo ayuda a acelerar la creación de proyectos, sino que garantiza que la información necesaria esté presente y que sea coherente en todos los proyectos.

Adjunte formularios personalizados de proyecto que coincidan con formularios personalizados de solicitud para extraer la información enviada al convertir la solicitud en un proyecto mediante la plantilla.

</br>
</br>

**Práctica recomendada**

Revisar y actualizar periódicamente las plantillas de proyecto.

**He aquí la razón**

A medida que cambien los procesos y los equipos, se deberán actualizar las plantillas de proyecto. Establezca una cadencia regular, como trimestral, para comprobar y ver qué plantillas no se utilizan de forma activa. Puede desactivarlas, por lo que aún se encuentran en Workfront, pero no aparecerán en las listas de selección de plantillas.

</br>
</br>

**Práctica recomendada**

Compruebe las plantillas para asegurarse de que tienen toda la información necesaria antes de compartirlas y de que otros usuarios empiecen a utilizarlas.


**He aquí la razón**

Dado que las plantillas se utilizarán una y otra vez para crear proyectos, querrá asegurarse de que todo esté configurado correcta y completamente. Esto conduce a la coherencia en todos los proyectos y a datos precisos para la creación de informes.

Además de la configuración de tareas, como la duración y las horas planificadas, algunos aspectos que se deben revisar antes de compartir las plantillas incluyen:

* Programar a partir de
* Restricciones de tarea
* Propietario, patrocinador, grupo y compañía del proyecto
* Portfolio y programa
* Ruta y pasos de hito
* Procesos de aprobación
* Asegúrese de que los usuarios asignados a tareas en proyectos tengan acceso de tipo Contribuir al proyecto
* Conjuntos de recursos
* Notificaciones de recordatorio
* Programación
* Configuración de moneda (si corresponde)
* Adjuntar documentos estándar
* Adjuntar los formularios de aduana necesarios
* Compruebe el equipo del proyecto para asegurarse de que no haya personas adicionales asignadas

</br>
</br>

**Práctica recomendada**

Cuando ajuste la opción Programar desde en una plantilla, revise y actualice las restricciones de la tarea.

**He aquí la razón**

La combinación de distintas delimitaciones de tareas en un proyecto puede causar cálculos de fechas planificadas inesperados y confusos. Por ejemplo, cuando se selecciona Fecha de inicio para la opción Programar desde, a cualquier tarea creada en ese proyecto se le asigna la delimitación de tareas Lo antes posible de forma predeterminada. Si posteriormente cambia la opción Programar desde a Fecha de finalización, las tareas creadas tendrán una delimitación de tareas Lo más tarde posible de forma predeterminada. Tener una combinación involuntaria de tareas con cada una de estas delimitaciones puede resultar en una confusión de las fechas planificadas en la escala de tiempo del proyecto.


</br>
</br>

**Práctica recomendada**

Compruebe el equipo del proyecto en la plantilla y elimine los usuarios que no trabajarán con el proyecto.

**He aquí la razón**

Al crear una plantilla a partir de un proyecto existente, se traslada a las personas a las que se les asignaron tareas o problemas en el proyecto. Y mientras trabaja con la plantilla, puede quitar personas a las que se les había asignado trabajo anteriormente o cambiar una asignación que haya realizado usted mismo en la plantilla.

Todos estos usuarios se enumerarán como parte del equipo del proyecto, en las secciones Personas y Programación del proyecto. Como resultado, se propagarán a todos los proyectos creados a partir de esa plantilla. Esto podría causar confusión al usuario, ya que como parte del equipo del proyecto, recibe notificaciones sobre la actividad en el proyecto, lo ve en la lista Proyectos en los que estoy y obtiene permisos sobre el proyecto y sus tareas, problemas y documentos.
