---
title: 'Práctica recomendada: preferencias de proyecto, tarea y problema'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de las preferencias de proyecto, tarea y problema de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Práctica recomendada: preferencias de proyecto, tarea y problema

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las mejores prácticas son directrices que representan un curso de acción eficaz y eficiente; sean adoptados fácilmente por usted y los usuarios de su empresa; y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, tenga en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco para ayudarle a guiar la configuración y el uso del sistema Workfront.

## Navegar por esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

La pregunta &quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas para las preferencias de proyecto, tarea y problema

* Establezca el tipo de duración de tarea predeterminado en Simple.

* Establezca la preferencia para el estado de un nuevo proyecto en Planificación o Idea, no en Actual.

* Active Crear líneas de base automáticamente en las preferencias globales del proyecto.

* Compruebe todas las opciones de la sección Casos de negocio de las preferencias del proyecto del sistema.

* En las preferencias de problemas, marque la opción para Actualizar automáticamente el estado del problema resuelto cuando cambie el estado del objeto resuelto.

</br>
</br>


## ¿Por qué estas prácticas recomendadas?

**Práctica recomendada**

Establezca el tipo de duración de tarea predeterminado en Simple.

**He aquí por qué**

Los tipos de duración definen la relación entre la duración de la tarea, las horas programadas y el número de personas asignadas a la tarea.

Con Simple como valor predeterminado del sistema global, todas las tareas creadas manualmente tienen este tipo de duración. Las horas planificadas se dividen de manera uniforme entre los asignadores de tareas a lo largo de la duración. El tipo de duración simple puede simplificar la planificación del proyecto, ya que le permite realizar cambios en los asignadores de tareas y en las horas planificadas sin afectar a la duración de la tarea, la fecha de inicio planificada o la fecha de finalización planificada.

</br>
</br>

**Práctica recomendada**

Establezca la preferencia para el estado de un nuevo proyecto en Planificación o Idea, no en Actual.

**He aquí por qué**

El estado Actual indica que un proyecto está activo y que el trabajo se está realizando. Es raro que un proyecto tenga que estar en este estado tras su creación. Incluso si utiliza una plantilla de proyecto, existe cierta &quot;planificación&quot; relacionada con la realización de asignaciones de tareas, el ajuste de la fecha de finalización prevista del proyecto, etc. El estado de Planning también suprime las notificaciones a los asignadores de tareas y a los integrantes del equipo del proyecto. Recibir notificaciones antes de que el proyecto esté activo puede ser confuso para los involucrados.

</br>
</br>

**Práctica recomendada**

Active Crear líneas de base automáticamente en las preferencias globales del proyecto.

**He aquí por qué**

Cada vez que cambia el estado de un proyecto a Actual, Workfront registra automáticamente una línea de base del proyecto. Esta &quot;instantánea&quot; del proyecto proporciona información histórica sobre cómo cambió el plan del proyecto con el paso del tiempo. Por ejemplo, puede comparar el plan del proyecto original con el plan actual cuando muestre cómo el cambio de prioridades o alcance afectó a los plazos del proyecto.

</br>
</br>

**Práctica recomendada**

Compruebe todas las opciones de la sección Casos de negocio de las preferencias del proyecto del sistema.

**He aquí por qué**

Active las cinco opciones para permitir que los administradores de proyectos, planificadores y otros incluyan cualquiera de esas secciones en el caso empresarial de un proyecto. Si las opciones no están activadas, no aparecen en la ventana de casos empresariales. Los usuarios pueden dejar cualquiera de los campos en blanco si no es necesario para ese proyecto en particular, pero no pueden habilitar un campo en el nivel de proyecto. Estas opciones solo se pueden habilitar globalmente en Configuración.

</br>
</br>

**Práctica recomendada**

En las preferencias de problemas, marque la opción para Actualizar automáticamente el estado del problema resuelto cuando cambie el estado del objeto resuelto.

**He aquí por qué**

Cuando un problema se convierte en un proyecto, esta configuración de preferencias &quot;vincula&quot; los estados de los dos elementos. Actualizar el estado del proyecto (el objeto de resolución) actualizará automáticamente el estado del problema. Esto significa que el solicitante puede ver el progreso realizado en su solicitud, aunque no tenga permisos para ver el proyecto completo en Workfront.
