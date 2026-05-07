---
title: 'Práctica recomendada: preferencias de proyecto, tarea y problema'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de las preferencias de proyecto, tarea y problema de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10918
exl-id: 321af897-3791-4b06-a9dd-241b5246b2a0
TQID: https://experienceleague.adobe.com/2Nc0Sj-3xZ-H8ir2OvXLhRJFEEKZu0DM8jIbFvizqlM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 704
ht-degree: 89%

---

# Práctica recomendada: preferencias de proyecto, tarea y problema

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El área &quot;¿Por qué son estas prácticas recomendadas?&quot;, que se encuentra después de la lista de alto nivel, proporciona más detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas para las preferencias de proyecto, tarea y problema

* Establezca el tipo de duración de tarea predeterminado en Simple.

* Establezca la preferencia para el estado de un nuevo proyecto en Planificación o Idea, no en Actual.

* Habilite Crear líneas de base automáticamente en las preferencias globales del proyecto.

* Compruebe todas las opciones de la sección Casos de negocio de las preferencias del proyecto del sistema.

* En las preferencias de problemas, marque la opción para Actualizar automáticamente el estado del problema resuelto cuando cambie el estado del objeto resuelto.

</br>
</br>


## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Establezca el tipo de duración de tarea predeterminado en Simple.

**A continuación se explica por qué**

Los tipos de duración definen la relación entre la duración de la tarea, las horas planificadas y el número de personas asignadas a la tarea.

Con Simple como valor predeterminado del sistema global, todas las tareas creadas manualmente tienen este tipo de duración. Las horas planificadas se dividen de manera uniforme entre los destinatarios de las tareas a lo largo de la duración. El tipo de duración simple puede simplificar la planificación del proyecto, ya que le permite realizar cambios en los destinatarios de las tareas y las horas planificadas, sin afectar a la duración de la tarea, la fecha de inicio o fecha planificada de finalización.

</br>
</br>

**Práctica recomendada**

Establezca la preferencia para el estado de un nuevo proyecto en Planificación o Idea, no en Actual.

**A continuación se explica por qué**

El estado Actual indica que el proyecto está activo y que el trabajo se está realizando. Es raro que un proyecto tenga que estar en este estado tras su creación. Incluso si utiliza una plantilla de proyecto, hay cierta &quot;planificación&quot; en realizar asignaciones de tareas, ajustar la fecha planificada de finalización del proyecto, etc. El estado de Planificación también suprime las notificaciones a los usuarios asignados de la tarea y a los miembros del equipo del proyecto. Recibir notificaciones antes de que el proyecto esté activo puede ser confuso para los involucrados.

</br>
</br>

**Práctica recomendada**

Habilite Crear líneas de base automáticamente en las preferencias globales del proyecto.

**A continuación se explica por qué**

Cada vez que cambia el estado de un proyecto a Actual, Workfront registra automáticamente una línea de base del proyecto. Esta “instantánea” del proyecto proporciona información histórica sobre cómo cambió el plan del proyecto con el paso del tiempo. Por ejemplo, puede comparar el plan del proyecto original con el plan actual cuando muestre a la dirección cómo el cambio de prioridades o alcance afectó a los plazos del proyecto.

</br>
</br>

**Práctica recomendada**

Compruebe todas las opciones de la sección Casos de negocio de las preferencias del proyecto del sistema.

**A continuación se explica por qué**

Active las cinco opciones para permitir que los administradores del proyecto, planificadores y otros incluyan cualquiera de esas secciones en el caso empresarial de un proyecto. Si las opciones no están habilitadas, no aparecen en la ventana de casos empresariales. Los usuarios pueden dejar cualquiera de los campos en blanco si no es necesario para ese proyecto en particular, pero no pueden habilitar un campo en el nivel de proyecto. Estas opciones solo se pueden habilitar globalmente en Configuración.

</br>
</br>

**Práctica recomendada**

En las preferencias de problemas, marque la opción para Actualizar automáticamente el estado del problema resuelto cuando cambie el estado del objeto resuelto.

**A continuación se explica por qué**

Cuando un problema se convierte en un proyecto, esta configuración de preferencias “vincula” los estados de los dos elementos. Al actualizar el estado del proyecto (el objeto de resolución) se actualiza automáticamente el estado del problema. Esto significa que el solicitante puede ver el progreso realizado en su solicitud, aunque no tenga permisos para ver el proyecto completo en Workfront.
