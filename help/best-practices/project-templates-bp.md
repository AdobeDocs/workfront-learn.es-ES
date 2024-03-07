---
title: 'Práctica recomendada: plantillas de proyecto'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de plantillas de proyecto de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: d39151288d8b749940c5183063392ee471769445
workflow-type: ht
source-wordcount: '1743'
ht-degree: 100%

---

# Práctica recomendada: plantillas de proyecto

## ¿Qué es una “práctica recomendada” de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de “por qué”.

La pregunta “¿Por qué son estas prácticas recomendadas?” se encuentra después de la lista de alto nivel, proporciona mayores detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., cuya implementación se debe considerar al trabajar con Workfront.

</br>
</br>

## Prácticas recomendadas para las plantillas de proyecto

* Utilice plantillas al crear proyectos.

* Establezca una convención de nomenclatura para las plantillas de proyecto.

* Establezca un grupo determinado de usuarios que puedan crear y actualizar plantillas de proyecto.

* Utilice el Uso compartido de proyectos en una plantilla de proyecto para conceder acceso automáticamente a los proyectos creados con esa plantilla.

* Asigne funciones de trabajo o equipos a tareas, no a las personas.

* Evite ser demasiado detallado al crear tareas en una plantilla de proyecto. Limite el número de tareas de una plantilla de proyecto a las necesarias para completar el trabajo.

* Utilice la descripción de la tarea para captar los pequeños pasos de la tarea, en lugar de desglosarla en varias tareas.

* Asegúrese de que las tareas de plantilla incluyan las duraciones de tareas, horas planificadas y predecesores.

* Configure previamente los detalles del proyecto y adjuntar formularios personalizados a la plantilla.

* Revise y actualice regularmente las plantillas de proyecto.

* Compruebe las plantillas para asegurarse de que tienen toda la información necesaria antes de compartirla y de que otras personas empiecen a utilizarla.

* Al ajustar la opción Programar desde en una plantilla, revise y actualice las restricciones de la tarea.

* Compruebe el equipo del proyecto en la plantilla y quite los usuarios que no estén asociados al proyecto.

</br>
</br>

## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Utilice plantillas al crear proyectos.

**He aquí por qué**

Las plantillas de proyecto eliminan las suposiciones de los administradores del proyecto (y otros que crean proyectos) sobre qué tareas debe contener un proyecto, cómo estructurar la cronología, etc. Las plantillas son la forma más eficaz de acelerar la creación de proyectos.

Es importante destacar que las plantillas proporcionan coherencia a los proyectos similares, de modo que las personas, los procesos y los puntos de datos se detallan del mismo modo cada vez. Incluso los proyectos con plazos de entrega rápidos (uno o dos días) y tareas mínimas pueden beneficiarse de la creación con plantillas de proyecto.

Esta coherencia entre los proyectos genera datos más precisos, lo que resulta vital a la hora de tomar decisiones para su equipo, su departamento y toda la organización.

</br>
</br>

**Práctica recomendada**

Establezca una convención de nomenclatura para las plantillas de proyecto.

**He aquí por qué**

La asignación de nombres coherente facilita la búsqueda de las plantillas. También ayuda a los administradores del proyecto y a otras personas que crean proyectos a seleccionar la plantilla correcta cuando hay plantillas con nombres similares en varios equipos o departamentos.

</br>
</br>

**Práctica recomendada**

Establezca un grupo determinado de usuarios que puedan crear y actualizar plantillas de proyecto.

**He aquí por qué**

Tener plantillas de proyecto coherentes y bien construidas es clave para una buena administración del trabajo y para una creación de informes precisos. Limite el número de usuarios que pueden editar plantillas para evitar cambios accidentales o no aprobados.

</br>
</br>

**Práctica recomendada**

Utilice el Uso compartido de proyectos en una plantilla de proyecto para conceder acceso automáticamente a los proyectos creados con esa plantilla.

**He aquí por qué**

El acceso a proyectos específicos se concede a través del propio proyecto. Si el mismo grupo de personas siempre necesita acceder a los proyectos creados con una plantilla específica, agréguelos en la opción Uso compartido de proyectos de la plantilla. No solo puede controlar el acceso a los proyectos en cuanto se creen, sino que también se optimizan los esfuerzos de escalabilidad si es necesario que los permisos cambien en el futuro.

Para obtener instrucciones sobre cómo compartir proyectos creados con una plantilla, consulte el capítulo titulado &quot;Cómo compartir proyectos creados con una plantilla&quot; en [Compartir una plantilla de proyecto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/share-a-project-template.html?lang=es).

**Nota**: El Uso compartido de plantillas otorga acceso a la plantilla misma. Un usuario debe tener al menos permisos de visualización para realizar proyectos con la plantilla.

</br>
</br>

**Práctica recomendada**

Asigne funciones de trabajo o equipos a tareas, no a las personas.

**He aquí por qué**

Cuando un usuario individual cambia de puesto de trabajo o abandona la organización, deberá actualizar manualmente las plantillas de proyecto que incluyan a esa persona. Esto lleva tiempo de parte de los administradores del sistema o grupo o de los administradores del proyecto.

Si utiliza funciones de trabajo o equipos en plantillas, los cambios de personal no tendrán un efecto directo en las plantillas de proyecto, ya que a cualquier persona a la que se le haya asignado esa función o ese equipo se le podría asignar el trabajo. Esto ayuda a garantizar que el trabajo no se escape de las manos. Las asignaciones de funciones también facilitan la asignación de trabajo a usuarios individuales, ya que Workfront puede mostrarle una lista de las personas a las que se ha asignado esa función de trabajo.

Además, las herramientas de planificación de recursos de Workfront utilizan las funciones de trabajo para ayudarle a calcular los recursos necesarios y planificar el trabajo futuro.

</br>
</br>

**Práctica recomendada**

Evite ser demasiado detallado al crear tareas en una plantilla de proyecto. Limite el número de tareas de una plantilla de proyecto a las necesarias para completar el trabajo.

**He aquí por qué**

Las plantillas de proyecto demasiado complicadas ocasionan una mala experiencia para los usuarios como los administradores del proyecto, administradores de recursos, integrantes del equipo, etc. Demasiadas tareas hacen que la cronología del proyecto sea difícil de administrar, con plazos de tareas superpuestos y varias tareas asignadas a las mismas funciones o personas.


</br>
</br>

**Práctica recomendada**

Utilice la descripción de la tarea para captar los pequeños pasos de la tarea, en lugar de desglosarla en varias tareas.

**He aquí por qué**

Si se asignan varias tareas de una fila a la misma función o a la misma persona, eso indica que esas tareas se podrían combinar. Tener demasiadas tareas asignadas a un usuario puede hacerle sentir que hay más trabajo por completar, lo que puede afectar a la adopción de Workfront.

</br>
</br>

**Práctica recomendada**

Asegúrese de que las tareas de plantilla incluyan las duraciones de tareas, horas planificadas y predecesores.

**He aquí por qué**

Estos tres elementos, duraciones, horas planificadas y predecesores, son los componentes básicos de la cronología del proyecto. Estas son claves para saber cuánto tiempo llevará hacer el trabajo y cuándo lo tendrá que hacer. Las herramientas de administración de recursos de Workfront emplean duraciones y horas planificadas, además de asignaciones de funciones para calcular la capacidad de los recursos, la disponibilidad y mucho más.

Si no está seguro de cómo calcular las duraciones o las horas planificadas por primera vez, trabaje con el equipo del proyecto para definir algunas estimaciones iniciales. Una vez que haya utilizado la plantilla, vuelva a reunirse con el equipo del proyecto para determinar dónde se podrían realizar cambios para que la plantilla sea más precisa. Si los usuarios registran el tiempo en Workfront, puede comparar las horas planificadas de un proyecto con las horas reales para ver dónde es necesario realizar ajustes.


</br>
</br>

**Práctica recomendada**

Configure previamente los detalles del proyecto y adjuntar formularios personalizados a la plantilla.

**He aquí por qué**

Asegúrese de rellenar la información estándar de todos los proyectos en la plantilla de proyecto. Esto no solo ayudará a acelerar la creación de proyectos, sino que también garantizará que la información necesaria esté presente y que sea coherente entre los proyectos.

Adjunte formularios personalizados de proyecto que coincidan con formularios personalizados de solicitud para extraer la información enviada al convertir la solicitud en un proyecto mediante la plantilla.

Para obtener instrucciones sobre cómo adjuntar un formulario personalizado a un objeto, como una plantilla de proyecto, consulte [Asignación de un formulario personalizado a un objeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-using-a-custom-form.html?lang=es).

</br>
</br>

**Práctica recomendada**

Revise y actualice regularmente las plantillas de proyecto.

**He aquí por qué**

A medida que cambian los procesos y los equipos, las plantillas de proyecto deben actualizarse. Establezca una cadencia normal, como trimestral, para comprobar y ver qué plantillas no se utilizan activamente. Puede desactivarlas, de modo que aún estén en Workfront, pero no aparezcan en listas de selección de plantillas.

Para obtener instrucciones sobre cómo desactivar una plantilla de proyecto, consulte [Desactivar una plantilla de proyecto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/deactivate-a-project-template.html?lang=es).

</br>
</br>

**Práctica recomendada**

Compruebe las plantillas para asegurarse de que tienen toda la información necesaria antes de compartirla y de que otras personas empiecen a utilizarla.


**He aquí por qué**

Dado que las plantillas se utilizarán una y otra vez para crear proyectos, deberá asegurarse de que todo esté configurado correctamente y completamente. Esto lleva a conseguir una coherencia en todos los proyectos y a la precisión de los datos para la creación de informes.

Además de la configuración de tareas, como la duración y las horas planificadas, es necesario revisar algunas cosas antes de compartir plantillas, como por ejemplo:

* La configuración Programación desde
* Las restricciones de tareas
* El propietario, patrocinador, grupo y empresa del proyecto
* Portafolios de productos y programas
* Pasos y ruta de hitos
* Procesos de aprobación
* Asegúrese de que los usuarios asignados a las tareas de los proyectos tengan acceso a Contribuir al proyecto
* Conjuntos de recursos
* Notificaciones de recordatorio
* Programación
* Configuración de moneda (si procede)
* Adjuntar documentos estándar
* Adjuntar los formularios aduaneros necesarios
* Comprobar el equipo del proyecto para asegurarse de que no haya personas adicionales asignadas

</br>
</br>

**Práctica recomendada**

Al ajustar la opción Modo de programación desde en una plantilla, revise y actualice las restricciones de la tarea.

**He aquí por qué**

La combinación de distintas restricciones de tareas en un proyecto puede provocar cálculos de fechas planificados inesperados y confusos. Por ejemplo, cuando se selecciona Fecha de inicio en la opción Modo de programación, cualquier tarea creada en ese proyecto se asignará de forma predeterminada a la restricción de tareas Tan pronto como sea posible. Si más adelante cambia la opción Modo de programación a Fecha de finalización, cualquier tarea creada tendrá de forma predeterminada una restricción de tarea Tan tarde como sea posible. Tener una combinación no intencional de tareas con cada una de estas restricciones puede dar como resultado fechas planificadas confusas en la cronología del proyecto.

Para comprender mejor las restricciones de tareas y cómo utilizarlas, consulte [Explicación y administración de los tipos de duración y las restricciones de tareas](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html?lang=es).

</br>
</br>

**Práctica recomendada**

Compruebe el equipo del proyecto en la plantilla y quite a los usuarios que no estén trabajando con el proyecto.

**He aquí por qué**

Cuando crea una plantilla a partir de un proyecto existente, a menos que elija la opción Borrar asignaciones durante la creación, Workfront coloca en la sección Personas a las personas a las que se les han asignado tareas o problemas en el proyecto. Y mientras trabaja con la plantilla, puede que quiera quitar a las personas a las que se les haya asignado trabajo anteriormente o cambiar una asignación que haya hecho usted mismo en la plantilla.

Todos estos usuarios se incluirán como parte del equipo del proyecto, en las secciones Personas y Programación del proyecto. Como resultado, se propagarán a todos los proyectos creados a partir de esa plantilla. Esto podría causar confusión para el usuario porque, como parte del equipo del proyecto, recibirá notificaciones sobre la actividad del proyecto, verá el proyecto en la lista de Proyectos en los que estoy y obtendrá permisos para el proyecto y sus tareas, problemas y documentos.

Para obtener instrucciones sobre cómo editar el equipo del proyecto en una plantilla de proyecto, consulte [Editar el equipo del proyecto en una plantilla de proyecto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/edit-the-project-team-in-a-project-template.html?lang=es).
