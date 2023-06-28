---
title: 'Práctica recomendada: preferencias de proyecto, tarea y problema'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de las preferencias de proyectos, tareas y problemas de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Práctica recomendada: preferencias de proyecto, tarea y problema

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de preferencias de proyectos, tareas y problemas

* Establezca el tipo de duración de tarea predeterminado en Simple.

* Establezca la preferencia para el estado de un nuevo proyecto en Planificación o Idea, no en Actual.

* Habilitar Crear líneas de base automáticamente en las preferencias de proyecto globales.

* Marque todas las opciones en la sección Casos comerciales de las preferencias de proyecto del sistema.

* En las preferencias de problemas, marque la opción Actualizar automáticamente el estado del problema solucionable cuando cambie el estado del objeto de resolución.

</br>
</br>


## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Establezca el tipo de duración de tarea predeterminado en Simple.

**He aquí la razón**

Los tipos de duración definen la relación entre la duración de la tarea, las horas planificadas y el número de personas asignadas a la tarea.

Con Simple como valor predeterminado del sistema global, todas las tareas creadas manualmente tienen este tipo de duración. Las horas planificadas se dividen equitativamente entre las personas asignadas a la tarea a lo largo de la duración. El tipo de duración sencilla puede simplificar la planificación del proyecto, ya que le permite realizar cambios en las personas asignadas a la tarea y en las horas planificadas sin afectar a la duración, la fecha de inicio o la fecha de finalización planificadas de la tarea.

</br>
</br>

**Práctica recomendada**

Establezca la preferencia para el estado de un nuevo proyecto en Planificación o Idea, no en Actual.

**He aquí la razón**

El estado Actual indica que un proyecto está activo y que se está trabajando activamente. Es raro que un proyecto necesite estar en este estado tras la creación. Incluso si utiliza una plantilla de proyecto, hay cierta &quot;planificación&quot; en realizar asignaciones de tareas, ajustar la fecha planificada de finalización del proyecto, etc. El estado de Planificación también suprime las notificaciones a los usuarios asignados de la tarea y a los miembros del equipo del proyecto. La recepción de notificaciones antes de que el proyecto esté activo puede resultar confusa para los implicados.

</br>
</br>

**Práctica recomendada**

Habilitar Crear líneas de base automáticamente en las preferencias de proyecto globales.

**He aquí la razón**

Cada vez que cambia el estado de un proyecto a Actual, Workfront registra automáticamente una línea de base del proyecto. Esta &quot;instantánea&quot; del proyecto proporciona información histórica sobre cómo el plan del proyecto cambió con el tiempo. Por ejemplo, puede comparar el plan del proyecto original con el plan actual cuando muestre al equipo de liderazgo cómo los cambios de prioridades o de alcance afectaron a los plazos del proyecto.

</br>
</br>

**Práctica recomendada**

Marque todas las opciones en la sección Casos comerciales de las preferencias de proyecto del sistema.

**He aquí la razón**

Habilite las cinco opciones para permitir que los jefes de proyecto, los planificadores y otros incluyan cualquiera de esas secciones en el caso comercial de un proyecto. Si las opciones no están habilitadas, no aparecen en la ventana de caso comercial. Los usuarios pueden dejar cualquiera de los campos en blanco si no es necesario para ese proyecto en particular, pero no pueden habilitar un campo en el nivel de proyecto. Estas opciones solo se pueden habilitar globalmente en Configuración.

</br>
</br>

**Práctica recomendada**

En las preferencias de problemas, marque la opción Actualizar automáticamente el estado del problema solucionable cuando cambie el estado del objeto de resolución.

**He aquí la razón**

Cuando un problema se convierte en un proyecto, esta configuración de preferencia &quot;vincula&quot; los estados de los dos elementos. Al actualizar el estado del proyecto (el objeto de resolución), se actualizará automáticamente el estado del problema. Esto significa que el solicitante puede ver el progreso que se realiza en su solicitud, incluso si no tiene permisos para ver todo el proyecto en Workfront.
