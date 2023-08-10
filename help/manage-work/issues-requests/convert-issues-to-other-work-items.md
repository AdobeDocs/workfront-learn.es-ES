---
title: Conversión de un problema o una solicitud en una tarea
description: Aprenda a convertir problemas a otros elementos de trabajo.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: convert-issues-to-other-work-items.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10069
exl-id: 1fd4d862-e44b-4c50-9663-70e727f6e9b7
source-git-commit: ce044bb73f980bd7424d3a477a05cef2a8527230
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 72%

---

# Conversión de un problema o una solicitud en una tarea

Un problema puede ser lo suficientemente significativo como para que el tiempo y el esfuerzo para resolverlo se tengan en cuenta en la cronología del proyecto y se asignen los recursos adecuados. En este caso, el problema se puede convertir en una tarea.

![Una imagen de la opción [!UICONTROL Convertir en tarea] de un problema en [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. Vaya a la sección [!UICONTROL Problemas] del proyecto o la tarea en la que el problema ha iniciado sesión. O busque el problema en un informe al que tenga acceso.
1. Haga clic en el nombre del problema para abrirlo.
1. En el menú de tres puntos a la derecha del nombre del problema, seleccione **[!UICONTROL Convertir en tarea]**.
1. Complete el formulario [!UICONTROL Convertir en tarea]. Comience dando un nombre y una descripción a la nueva tarea.
1. Si la nueva tarea debe formar parte de un proyecto diferente, introduzca el nombre del proyecto.
1. En la sección [!UICONTROL Opciones], marque las casillas para mantener el problema original, permitir el acceso a la nueva tarea y mantener la fecha de finalización. Siga el flujo de trabajo de su organización al realizar estas selecciones.
1. Adjunte un formulario personalizado si desea transferir datos de formulario personalizados del problema a la tarea. (Todos los campos que existen tanto en el formulario de problemas como en el de tareas se transferirán automáticamente al formulario de tareas).
1. Haga clic en **[!UICONTROL Convertir en tarea]** para terminar.

![Una imagen del formulario [!UICONTROL Convertir en tarea] de un problema en [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

Según la organización de [!DNL Workfront] Configuración del sistema, puede que no pueda cambiar la configuración de la sección Opciones cuando convierta la tarea. Estas opciones afectan tanto al problema original como a la nueva tarea.

* **&quot;Mantener el problema original y enlazar su solución a esta tarea&quot;** conserva el problema original y la información relacionada (horas, documentos, etc.). Con esta opción seleccionada, cuando se complete la tarea, el problema se marcará como resuelto. Si esta opción es **no** Si se selecciona, el problema original se eliminará al crear la tarea. Esto puede afectar a la forma en que su organización realiza el seguimiento de los problemas y genera informes sobre ellos.
* El **&quot;Permitir que (nombre de usuario) tenga acceso a esta tarea&quot;** Esta opción permite que la persona que creó el problema tenga acceso a esta nueva tarea.
* El **&quot;Conservar la fecha planificada de finalización del problema&quot;** La opción le permite mantener la fecha planificada de finalización ya establecida en el problema. Esto establece la restricción de tarea en [!UICONTROL Finalizar a más tardar]. Si la casilla está desactivada, las fechas de la tarea se establecen como si se creara una nueva tarea dentro del proyecto.

La nueva tarea se coloca en la parte inferior de la lista de tareas del proyecto. Mueva la tarea a la ubicación deseada, asigne un usuario o equipo al trabajo, añada horas y duración planificadas, etc.

>[!NOTE]
>
>No se pueden agregar problemas a la cronología del proyecto, ya que representan “trabajo no planificado”. La cronología del proyecto es para el “trabajo planificado”, es decir, para las tareas.


