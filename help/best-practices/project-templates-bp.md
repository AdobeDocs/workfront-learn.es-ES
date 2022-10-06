---
title: 'Práctica recomendada: Plantillas de proyecto'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de plantillas de proyecto de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---

# Práctica recomendada: Plantillas de proyecto

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las mejores prácticas son directrices que representan un curso de acción eficaz y eficiente; sean adoptados fácilmente por usted y los usuarios de su empresa; y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, tenga en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco para ayudarle a guiar la configuración y el uso del sistema Workfront.

## Navegar por esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

La pregunta &quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de plantillas de proyecto

* Utilice plantillas al crear proyectos.

* Establezca una convención de nombres para las plantillas de proyecto.

* Establezca un grupo determinado de usuarios que puedan crear y actualizar plantillas de proyecto.

* Utilice Uso compartido de proyectos en una plantilla de proyecto para conceder acceso automáticamente a los proyectos creados con esa plantilla.

* Asigne funciones de trabajo o equipos a tareas, no a personas.

* Evite ser demasiado granular al crear tareas en una plantilla de proyecto. Limite el número de tareas de una plantilla de proyecto a las necesarias para completar el trabajo.

* Utilice la descripción de la tarea para capturar los pequeños pasos de la tarea, en lugar de desglosarla en varias tareas.

* Asegúrese de que las tareas de plantilla incluyen duraciones de tareas, horas planificadas y predecesores.

* Preconfigurar los detalles del proyecto y adjuntar formularios personalizados a la plantilla.

* Revise y actualice regularmente las plantillas de proyecto.

* Compruebe las plantillas para asegurarse de que tienen toda la información necesaria antes de compartirla y de que otras personas empiecen a utilizarla.

* Al ajustar la opción Programar desde en una plantilla, revise y actualice las restricciones de la tarea.

* Compruebe el equipo del proyecto en la plantilla y elimine los usuarios que no estén asociados al proyecto.

</br>
</br>

## ¿Por qué estas prácticas recomendadas?

**Práctica recomendada**

Utilice plantillas al crear proyectos.

**He aquí por qué**

Las plantillas de proyecto eliminan las conjeturas de los jefes de proyecto (y otros que crean proyectos) sobre qué tareas debe contener un proyecto, cómo estructurar la cronología, etc. Las plantillas son la forma más eficaz de acelerar la creación de proyectos.

Es importante destacar que las plantillas proporcionan coherencia en los proyectos de tipos similares, de modo que las personas, los procesos y los puntos de datos se detallan del mismo modo cada vez. Incluso los proyectos con retornos rápidos (uno o dos días) y tareas mínimas pueden beneficiarse de la creación con plantillas de proyecto.

Esta coherencia entre los proyectos genera datos más precisos, lo que resulta vital a la hora de tomar decisiones para su equipo, su departamento y toda la organización.

</br>
</br>

**Práctica recomendada**

Establezca una convención de nombres para las plantillas de proyecto.

**He aquí por qué**

La asignación de nombres coherente facilita la búsqueda de las plantillas. También ayuda a los administradores de proyectos y a otras personas que crean proyectos a seleccionar la plantilla correcta cuando hay plantillas con nombres similares en varios equipos o departamentos.

</br>
</br>

**Práctica recomendada**

Establezca un grupo determinado de usuarios que puedan crear y actualizar plantillas de proyecto.

**He aquí por qué**

Tener plantillas de proyecto coherentes y bien construidas es clave para una buena administración del trabajo y para generar informes precisos. Limite el número de usuarios que pueden editar plantillas para evitar cambios accidentales o no aprobados.

</br>
</br>

**Práctica recomendada**

Utilice Uso compartido de proyectos en una plantilla de proyecto para conceder acceso automáticamente a los proyectos creados con esa plantilla.

**He aquí por qué**

El acceso a proyectos específicos se concede a través del propio proyecto. Si el mismo grupo de personas siempre necesita acceder a los proyectos creados con una plantilla específica, agréguelos en la opción Uso compartido de proyectos de la plantilla. No solo puede controlar el acceso a los proyectos en cuanto se creen, sino que también optimiza los esfuerzos de escalabilidad si es necesario que los permisos cambien en el futuro.

**Nota**: Uso compartido de plantillas otorga acceso a la plantilla misma. Un usuario debe tener al menos permisos de visualización para realizar proyectos con la plantilla.

</br>
</br>

**Práctica recomendada**

Asigne funciones de trabajo o equipos a tareas, no a personas.

**He aquí por qué**

Cuando un usuario individual cambia de posición o abandona la organización, deberá actualizar manualmente las plantillas de proyecto que incluyan a esa persona. Esto lleva tiempo en parte de los administradores del sistema o grupo o de los jefes de proyecto.

Si utiliza funciones de trabajo o equipos en plantillas, los cambios de plantilla no tendrán un efecto directo en las plantillas de proyecto, ya que a cualquier persona a la que se le haya asignado esa función de trabajo o a ese equipo se le podría asignar el trabajo. Esto ayuda a garantizar que el trabajo no se deslice por las grietas. Las asignaciones de funciones de trabajo también facilitan la asignación de trabajo a usuarios individuales, ya que Workfront puede mostrarle una lista de las personas a las que se ha asignado esa función de trabajo.

Además, las herramientas de planificación de recursos de Workfront utilizan las funciones de trabajo para ayudarle a calcular los recursos necesarios y planificar el trabajo futuro.

</br>
</br>

**Práctica recomendada**

Evite ser demasiado granular al crear tareas en una plantilla de proyecto. Limite el número de tareas de una plantilla de proyecto a las necesarias para completar el trabajo.

**He aquí por qué**

Las plantillas de proyecto demasiado complicadas resultan en una mala experiencia para los usuarios: administradores de proyectos, administradores de recursos, integrantes del equipo, etc. Demasiadas tareas hacen que la cronología del proyecto sea difícil de administrar, con plazos de tareas superpuestos y varias tareas asignadas a las mismas funciones o personas.


</br>
</br>

**Práctica recomendada**

Utilice la descripción de la tarea para capturar los pequeños pasos de la tarea, en lugar de desglosarla en varias tareas.

**He aquí por qué**

Si se asignan varias tareas de una fila a la misma función de trabajo o a la misma persona, eso indica que esas tareas se podrían combinar. Tener demasiadas tareas asignadas a un usuario puede hacerles sentir que hay más trabajo por completar, lo que puede afectar a la adopción de Workfront.

</br>
</br>

**Práctica recomendada**

Asegúrese de que las tareas de plantilla incluyen duraciones de tareas, horas planificadas y predecesores.

**He aquí por qué**

Estas tres cosas (duraciones, horas planificadas y predecesores) son los componentes básicos de la cronología del proyecto. Estas son claves para saber cuánto tiempo tardará el trabajo y cuándo lo tendrá que hacer. Las duraciones y las horas planificadas de las herramientas de administración de recursos de Workfront, además de las asignaciones de funciones de trabajo, permiten calcular la capacidad de los recursos, la disponibilidad y mucho más.

Si no está seguro de cómo estimar las duraciones o las horas programadas por primera vez, trabaje con el equipo del proyecto para definir algunas estimaciones iniciales. Una vez que haya utilizado la plantilla, vuelva a reunirse con el equipo del proyecto para determinar dónde se pueden realizar cambios para que la plantilla sea más precisa. Si los usuarios están iniciando sesión en Workfront, puede comparar las horas planificadas de un proyecto con las horas reales para ver dónde se necesitan los ajustes.


</br>
</br>

**Práctica recomendada**

Preconfigurar los detalles del proyecto y adjuntar formularios personalizados a la plantilla.

**He aquí por qué**

Asegúrese de que la información estándar de todos los proyectos se rellene en la plantilla de proyecto. Esto no solo ayuda a acelerar la creación de proyectos, sino que también garantiza que la información necesaria esté allí y que sea coherente en todos los proyectos.

Adjunte formularios personalizados de proyecto que coincidan con formularios personalizados de solicitud para extraer la información enviada al convertir la solicitud en un proyecto mediante la plantilla.

</br>
</br>

**Práctica recomendada**

Revise y actualice regularmente las plantillas de proyecto.

**He aquí por qué**

A medida que cambian los procesos y los equipos, las plantillas de proyecto deben actualizarse. Establezca una cadencia normal, como trimestral, para comprobar y ver qué plantillas no se utilizan activamente. Puede desactivarlos, de modo que aún estén en Workfront pero no aparezcan en listas de selección de plantillas.

</br>
</br>

**Práctica recomendada**

Compruebe las plantillas para asegurarse de que tienen toda la información necesaria antes de compartirla y de que otras personas empiecen a utilizarla.


**He aquí por qué**

Dado que las plantillas se utilizarán una y otra vez para crear proyectos, debe asegurarse de que todo esté configurado correctamente y completamente. Esto lleva a la coherencia en todos los proyectos y a la precisión de los datos para los informes.

Además de la configuración de tareas, como la duración y las horas planificadas, algunas cosas que se deben revisar antes de compartir plantillas son:

* Programar desde la configuración
* Restricciones de tareas
* Propietario, patrocinador, grupo y empresa del proyecto
* Portfolio y programa
* Ruta y pasos de Milestone
* Procesos de aprobación
* Asegúrese de que los usuarios asignados a tareas en proyectos tengan acceso de Contribute al proyecto
* Conjuntos de recursos
* Notificaciones de recordatorio
* Horario
* Configuración de moneda (si procede)
* Adjuntar documentos estándar
* Adjuntar los formularios aduaneros necesarios
* Compruebe el equipo del proyecto para asegurarse de que no haya personas adicionales asignadas

</br>
</br>

**Práctica recomendada**

Al ajustar la opción Programar desde en una plantilla, revise y actualice las restricciones de la tarea.

**He aquí por qué**

La combinación de distintas restricciones de tareas en un proyecto puede provocar cálculos de fechas planificados inesperados y confusos. Por ejemplo, cuando se selecciona Fecha de inicio en la opción Programar desde , cualquier tarea creada en ese proyecto se asigna de forma predeterminada a la restricción de tareas Tan pronto como sea posible . Si más adelante cambia la opción Programar de a Fecha de Finalización, cualquier tarea creada tendrá de forma predeterminada una restricción de tarea Tan tarde como sea posible. Tener una combinación no intencional de tareas con cada una de estas restricciones puede dar como resultado confusos fechas planificadas en la cronología del proyecto.


</br>
</br>

**Práctica recomendada**

Compruebe el equipo del proyecto en la plantilla y elimine los usuarios que no estén trabajando con el proyecto.

**He aquí por qué**

Cuando crea una plantilla a partir de un proyecto existente, atrae a las personas a las que se asignaron tareas o problemas en el proyecto. Y mientras trabaja con la plantilla, puede eliminar personas a las que se les haya asignado trabajo anteriormente o cambiar una asignación que haya hecho usted mismo en la plantilla.

Todos estos usuarios se incluirán como parte del equipo del proyecto, en las secciones Personas y Programación del proyecto. Como resultado, se propagarán a todos los proyectos creados a partir de esa plantilla. Esto podría causar confusión para el usuario porque, como parte del equipo del proyecto, recibe notificaciones sobre la actividad del proyecto, ve el proyecto en la lista Proyectos en los que estoy y obtiene permisos para el proyecto y sus tareas, problemas y documentos.
