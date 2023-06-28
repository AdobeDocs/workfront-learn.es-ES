---
title: Convertir problemas a otros elementos de trabajo
description: Aprenda a convertir problemas en otros elementos de trabajo
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: convert-issues-to-other-work-items.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10069
exl-id: 1fd4d862-e44b-4c50-9663-70e727f6e9b7
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 0%

---

# Convertir problemas en otros elementos de trabajo

## Conversión de un problema en una tarea

Un problema puede ser lo suficientemente importante como para que el tiempo y el esfuerzo para resolverlo deban tenerse en cuenta en el calendario del proyecto y asignarse los recursos apropiados. En este caso, el problema se puede convertir en una tarea.

![Una imagen de la [!UICONTROL Convertir a tarea] opción de un problema en [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. Vaya a [!UICONTROL Problemas] del proyecto o tarea en el que se ha iniciado sesión el problema. O busque el problema en un informe al que tenga acceso.
1. Haga clic en el nombre del problema para abrirlo.
1. En el menú de 3 puntos situado a la derecha del nombre del problema, seleccione **[!UICONTROL Convertir a tarea]**.
1. Rellene el [!UICONTROL Convertir a tarea] formulario. Comience asignando un nombre y una descripción a la nueva tarea.
1. Si la nueva tarea debe formar parte de un proyecto diferente, escriba el nombre del proyecto.
1. En el [!UICONTROL Opciones] , marque las casillas para mantener el problema original, permitir el acceso a la nueva tarea y mantener la fecha de finalización. Siga el flujo de trabajo de su organización al realizar estas selecciones. Adjunte un formulario personalizado si desea transferir datos de formulario personalizados del problema a la tarea. (Todos los campos que existen tanto en el formulario de problema como en el formulario de tarea se transferirán automáticamente al formulario de tarea).
1. Rellene el formulario personalizado, si hay alguno adjunto.
1. Clic **[!UICONTROL Convertir a tarea]** para terminar.

![Una imagen de la [!UICONTROL Convertir a tarea] forma de problema en [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

Según el perfil de la organización [!DNL Workfront] Configuración del sistema, puede que no pueda cambiar la configuración de la sección Opciones cuando convierta la tarea. Estas opciones afectan tanto al problema original como a la nueva tarea.

* **&quot;Mantener el problema original y enlazar su solución a esta tarea&quot;** conserva el problema original y la información relacionada (horas, documentos, etc.). Con esta opción seleccionada, cuando se complete la tarea, el problema se marcará como resuelto. Si no se selecciona esta opción, el problema original se eliminará al finalizar la tarea. Esto puede afectar al modo en que su organización realiza el seguimiento y realiza informes sobre los problemas.
* El **&quot;Permitir que (nombre de usuario) tenga acceso a esta tarea&quot;** Esta opción permite que la persona que creó el problema tenga acceso a esta nueva tarea.
* El **&quot;Conservar la fecha planificada de finalización del problema&quot;** La opción le permite mantener la fecha planificada de finalización ya establecida en el problema. Esto establece la restricción de tarea en [!UICONTROL No terminar después de]. Si la casilla no está marcada, las fechas de la tarea se establecerán como si se creara una nueva tarea dentro del proyecto.

La nueva tarea se coloca al final de la lista de tareas del proyecto. Mueva la tarea a la ubicación deseada, asigne un usuario o equipo al trabajo, añada las horas y la duración planificadas, etc.

>[!NOTE]
>
>No puede agregar problemas a la cronología del proyecto, ya que representan &quot;trabajo no planificado&quot;. La cronología del proyecto es para &quot;trabajo planificado&quot;, es decir, tareas.

## Conversión de un problema en un proyecto

Hay ocasiones en que un problema no se puede resolver resolviendo el problema en sí o convirtiéndolo en una tarea porque el proceso de resolución del problema debe coordinarse más intrincadamente. En este caso, puede convertir el problema en un proyecto.

1. Vaya a la sección Problemas del proyecto o tarea en la que se ha iniciado sesión el problema. O busque el problema en un informe al que tenga acceso.
1. Haga clic en el nombre del problema para abrirlo.
1. Haga clic en el menú de 3 puntos a la derecha del nombre del problema para mostrar el menú Más.
1. A continuación, seleccione si desea crear un nuevo proyecto que esté totalmente en blanco o utilice una plantilla de proyecto, que rellenará previamente la información de la tarea y la escala de tiempo.
1. Rellene la información de la ventana Convertir en proyecto, empezando por el nombre del proyecto.
1. Rellene otros detalles del proyecto según sea necesario para su equipo u organización.
1. En la sección Opciones, marque las casillas para mantener el problema original y permitir el acceso al nuevo proyecto. Siga el flujo de trabajo de su organización al realizar estas selecciones.
1. Rellene el formulario personalizado, si hay alguno adjunto. Adjunte un formulario personalizado si desea transferir datos de formulario personalizados del problema al proyecto. (Todos los campos que existen tanto en el formulario de problema como en el formulario de proyecto se transferirán automáticamente al formulario de proyecto).
1. Clic **Convertir a proyecto** para terminar.

Los campos de detalles del proyecto que aparecen en la ventana Convertir en proyecto dependen del método utilizado para crear el proyecto. Verá más información en el menú de la izquierda si utilizó la opción Convertir a proyecto desde plantilla.

>[!NOTE]
>
>Algunas secciones, como la sección Opciones, aunque visibles, pueden ser inaccesibles según la configuración del sistema de Workfront de su organización.

![Imagen de una pantalla de proyecto que muestra las opciones de conversión](assets/conversion-options.png)

* Haga clic en &quot;**Mantener el problema original y enlazar su solución a este proyecto** Opción &quot;. Esta opción conserva el problema original y la información relacionada (horas, documentos, etc.). Cuando se completa el nuevo proyecto, el problema se marca como resuelto. Si no se selecciona esta opción, el problema original se eliminará al finalizar el proyecto. Esto puede afectar al modo en que su organización realiza el seguimiento y realiza informes sobre los problemas.
* El &quot;**Permitir que (nombre de usuario) tenga acceso a este proyecto** La opción &quot; permite que la persona que creó el problema tenga acceso al proyecto que se está creando.

## Mantener información durante el proceso de conversión

<!-- Need link to wf one doc article below 

To learn about what information transfers when you convert an issue to a task or project, we recommend you read through the conversion considerations in the article, Convert issues. This lists what information is kept when converting issues and what isn’t. Workfront recommends you become familiar with these considerations so you don’t lose important information when converting issues to tasks or projects.

-->

La transferencia de los datos del formulario personalizado requiere lo siguiente:

* Varias copias del mismo formulario personalizado: una para el problema y otra para la tarea o el proyecto. Los campos de estos formularios personalizados deben coincidir de forma exacta, de modo que la información se pueda transferir de un formulario personalizado al otro.

* O un solo formulario personalizado en el que se seleccionan el problema, la tarea o los objetos del proyecto. Con este método, solo es necesario crear y mantener los campos personalizados en un único formulario personalizado. Se trata de una mejora reciente y es mucho más fácil que tener varias copias del mismo formulario, pero cualquiera de los dos métodos funcionará.



<!-- Need link to wf one doc article below

Learn more in the article, Transfer custom form data to a larger work item.

-->

<!-- Pro tips graphic -->

Si incluye un formulario personalizado en una plantilla de proyecto, se asignará automáticamente cuando la plantilla se seleccione en el proceso de conversión.

<!-- Learn more graphic and documentation article links 

* Convert issues
* Transfer custom form data to a larger work item
* Overview of resolving and resolvable objects
* Understanding resolving and resolvable objects
* Unlink issues from their resolvable objects

-->

## Convertir un problema en una tarea o proyecto desde cualquier lista de problemas

Para aumentar la eficacia del trabajo y facilitar la conversión de problemas en un entorno acelerado, puede convertir un problema en una tarea o un proyecto desde cualquier lista de problemas de un proyecto, informe o panel. Seleccione un problema y haga clic en el menú de 3 puntos que aparece.

![Imagen de una pantalla de proyecto que muestra las opciones de conversión de problemas](assets/convert-from-a-list.png)

