---
title: 'Práctica recomendada: plantillas de proyecto'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de plantillas de proyecto de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10919
exl-id: 17cd2e49-ee16-4b80-a8b2-ccc254fa8014
source-git-commit: 6a155c50d31e789381c1151e9ee9c091e62c909e
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 61%

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

* Compruebe el equipo del proyecto en la plantilla y elimine los usuarios que no estén asociados al proyecto.

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

El acceso a proyectos específicos se concede a través del propio proyecto. Si el mismo grupo de personas siempre necesita acceder a los proyectos creados con una plantilla específica, agréguelos en la opción Uso compartido de proyectos de la plantilla. No solo puede controlar el acceso a los proyectos en cuanto se crean, sino que además optimiza los esfuerzos de escalabilidad si los permisos deben cambiar en el futuro.

Para obtener instrucciones sobre cómo compartir proyectos creados con una plantilla, consulte el capítulo titulado &quot;Cómo compartir proyectos creados con una plantilla&quot; en [Compartir una plantilla de proyecto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/create-and-manage-project-templates/share-a-project-template.html).

**Nota**: El Uso compartido de plantillas otorga acceso a la plantilla misma. Un usuario debe tener al menos permisos de visualización para realizar proyectos con la plantilla.

</br>
</br>

**Práctica recomendada**

Asigne funciones de trabajo o equipos a tareas, no a las personas.

**He aquí por qué**

Cuando un usuario individual cambia de posición o abandona la organización, debe actualizar manualmente las plantillas de proyecto que incluyen a esa persona. Esto lleva tiempo de parte de los administradores del sistema o grupo o de los administradores del proyecto.

Si utiliza roles o equipos en las plantillas, los cambios de plantilla no tendrán un efecto directo en las plantillas de proyecto porque a cualquier persona asignada a ese rol o a ese equipo se le podría asignar el trabajo. Esto ayuda a garantizar que el trabajo no se deslice por las grietas. Las asignaciones de funciones también facilitan la asignación de trabajo a usuarios individuales, ya que Workfront puede mostrarle una lista de las personas a las que se ha asignado esa función de trabajo.

Además, las herramientas de planificación de recursos de Workfront utilizan las funciones del puesto para ayudarle a calcular los recursos necesarios y planificar el trabajo futuro.

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

Si se asignan varias tareas de una fila al mismo rol o individuo, eso indica que esas tareas se podrían combinar. Si se asignan demasiadas tareas a un usuario, es posible que parezca que hay más trabajo por completar, lo que puede afectar a la adopción de Workfront.

</br>
</br>

**Práctica recomendada**

Asegúrese de que las tareas de plantilla incluyan las duraciones de tareas, horas planificadas y predecesores.

**He aquí por qué**

Estas tres cosas (duraciones, horas planificadas y predecesoras) son los componentes básicos de la cronología del proyecto. Estas son claves para saber cuánto tiempo llevará hacer el trabajo y cuándo lo tendrá que hacer. Las herramientas de administración de recursos de Workfront utilizan duraciones y horas planificadas, además de asignaciones de roles, para calcular la capacidad de los recursos, la disponibilidad y mucho más.

Si no está seguro de cómo estimar las duraciones o las horas planificadas por primera vez, trabaje con el equipo del proyecto para definir algunas estimaciones iniciales. Una vez que haya utilizado la plantilla, vuelva a reunirse con el equipo del proyecto para determinar dónde se pueden realizar cambios para que la plantilla sea más precisa. Si los usuarios registran el tiempo en Workfront, puede comparar las horas planificadas de un proyecto con las horas reales para ver dónde son necesarios los ajustes.


</br>
</br>

**Práctica recomendada**

Configure previamente los detalles del proyecto y adjuntar formularios personalizados a la plantilla.

**He aquí por qué**

Asegúrese de rellenar la información estándar de todos los proyectos en la plantilla de proyecto. Esto no solo ayuda a acelerar la creación de proyectos, sino que garantiza que la información necesaria esté presente y que sea coherente en todos los proyectos.

Adjunte formularios personalizados de proyecto que coincidan con formularios personalizados de solicitud para extraer la información enviada al convertir la solicitud en un proyecto mediante la plantilla.

Para obtener instrucciones sobre cómo adjuntar un formulario personalizado a un objeto, como una plantilla de proyecto, consulte [Adjuntar un formulario personalizado a un objeto](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-using-a-custom-form.html).

</br>
</br>

**Práctica recomendada**

Revise y actualice regularmente las plantillas de proyecto.

**He aquí por qué**

A medida que cambian los procesos y los equipos, las plantillas de proyecto deben actualizarse. Establezca una cadencia regular, como trimestral, para comprobar y ver qué plantillas no se utilizan de forma activa. Puede desactivarlos para que sigan en Workfront, pero no aparecerán en las listas de selección de plantillas.

</br>
</br>

**Práctica recomendada**

Compruebe las plantillas para asegurarse de que tienen toda la información necesaria antes de compartirla y de que otras personas empiecen a utilizarla.


**He aquí por qué**

Dado que las plantillas se utilizarán una y otra vez para crear proyectos, debe asegurarse de que todo esté configurado correctamente y por completo. Esto lleva a conseguir una coherencia en todos los proyectos y a la precisión de los datos para la creación de informes.

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
* Compruebe el equipo del proyecto para asegurarse de que no haya personas adicionales asignadas

</br>
</br>

**Práctica recomendada**

Cuando ajuste la opción Modo de horario en una plantilla, revise y actualice las restricciones de la tarea.

**He aquí por qué**

La combinación de distintas restricciones de tareas en un proyecto puede provocar cálculos de fechas planificados inesperados y confusos. Por ejemplo, cuando se selecciona Fecha de inicio para la opción Modo de programación, a todas las tareas creadas en ese proyecto se les asigna la delimitación de tareas Lo antes posible de forma predeterminada. Si posteriormente cambia la opción Modo de horario a Fecha de finalización, las tareas creadas tendrán una delimitación de tareas Lo más tarde posible de forma predeterminada. Tener una combinación no intencional de tareas con cada una de estas restricciones puede dar como resultado fechas planificadas confusas en la cronología del proyecto.

Para comprender mejor las restricciones de tareas y cómo utilizarlas, consulte [Explicación y administración de los tipos de duración y las restricciones de tareas](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html?lang=es).

</br>
</br>

**Práctica recomendada**

Compruebe el equipo del proyecto en la plantilla y elimine los usuarios que no van a trabajar con el proyecto.

**He aquí por qué**

Cuando crea una plantilla a partir de un proyecto existente, a menos que elija la opción Borrar asignaciones durante la creación, Workfront coloca en la sección Personas a las personas a las que se les han asignado tareas o problemas en el proyecto. Y mientras trabaja con la plantilla, puede que desee quitar estas personas a las que se les asignó anteriormente un trabajo o cambiar una asignación que usted mismo hizo en la plantilla.

Todos estos usuarios se incluirán como parte del equipo del proyecto, en las secciones Personas y Programación del proyecto. Como resultado, se propagarán a todos los proyectos creados a partir de esa plantilla. Esto podría causar confusión al usuario porque, como parte del equipo del proyecto, recibe notificaciones sobre la actividad en el proyecto, ve el proyecto en la lista Proyectos en los que estoy y obtiene permisos para el proyecto y sus tareas, problemas y documentos.


