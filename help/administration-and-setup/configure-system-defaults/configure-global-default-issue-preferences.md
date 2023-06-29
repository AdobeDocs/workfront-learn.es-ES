---
title: Configurar las preferencias de problemas predeterminadas globales
description: Obtenga información sobre cómo establecer las preferencias de problemas para problemas convertidos, fechas reales y acceso a problemas.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '885'
ht-degree: 100%

---

# Configurar las preferencias de problemas predeterminadas globales

Varias configuraciones de todo el sistema establecen valores predeterminados para el comportamiento de los problemas en determinadas circunstancias en [!DNL Workfront].

Una práctica recomendada es dejar los valores predeterminados globales tal cual y permitir a los administradores del proyecto realizar los ajustes que necesiten en el nivel o en las plantillas de proyecto.

Las preferencias del problema global se pueden ajustar, pero se recomienda que usted y su asesor de [!DNL Workfront] hablen sobre qué configuración se necesita para los flujos de trabajo, los procesos y las necesidades de creación de informes de su organización. El asesor también puede ayudarle a comprender qué ocurrirá si se cambian determinadas opciones de configuración.

Las preferencias de problemas permiten a los administradores del sistema controlar las opciones cuando los problemas se convierten en tareas o proyectos, cómo se calculan las fechas reales y quién obtiene acceso al proyecto cuando se designan problemas. Echemos un vistazo a dónde se encuentra esa configuración en [!DNL Workfront].

## Preferencias convertidas de problemas

Esta configuración controla lo que ocurre con un problema cuando se convierte en una tarea o un proyecto en [!DNL Workfront].

Ventana de preferencias ![[!UICONTROL Tareas y problemas] con la sección de [!UICONTROL Problemas] resaltada](assets/admin-fund-issue-prefs-converting.png)

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expanda la sección **[!UICONTROL Preferencias de proyecto]** en el panel de menú de la izquierda.
1. Seleccione **[!UICONTROL Tareas y problemas]**.
1. Desplácese hasta la sección **[!UICONTROL Problemas]**.
1. Haga clic en las opciones que desee.
1. Guarde cuando haya terminado.

Veamos las opciones de esta sección para que pueda elegir las opciones adecuadas para su organización.

* **[!UICONTROL Actualizar automáticamente el estado del problema solucionable cuando cambie el estado del objeto de resolución]**

  Esta configuración permite correlacionar la resolución del problema original con la resolución del nuevo objeto (tarea o proyecto).

  Con esta configuración habilitada (seleccionada), puede crear estados de problemas personalizados que tengan la misma clave de estado que una tarea o estado del proyecto. Cuando la tarea o el proyecto (el objeto solucionable) se establece en el estado personalizado, el cambio también se muestra en el estado del problema.

  Cuando está desactivado, el estado del objeto solucionable se establece automáticamente en el estado predeterminado, no en el personalizado.

  Para que esta configuración tenga algún efecto, la opción “[!UICONTROL Mantener el problema original y vincular su resolución a la tarea]” debe estar seleccionada.

* **[!UICONTROL Mantener el problema original y vincular su resolución a la tarea/proyecto]**

  Cuando se convierte el problema, esto le indica a [!DNL Workfront] que conserve los problemas originales. El estado del problema cambia a medida que se cambia el estado de la tarea o del proyecto. Una vez que la tarea o el proyecto se ha marcado como completado, el problema se marca como resuelto.

  Si no se selecciona esta opción, se elimina el problema original y solo permanece la tarea o proyecto convertido.

  Esta configuración afecta a la creación de informes sobre los problemas que originalmente se iniciaron en un proyecto o que se producen a través de la cola de solicitudes de [!DNL Workfront].

* **[!UICONTROL Permita que el contacto primario acceda a la tarea/proyecto]**

  Esto da acceso a la persona que creó el problema original a la tarea o al proyecto durante la conversión. Pueden revisar el trabajo, hacer actualizaciones y mantenerse informados de su progreso.

* **[!UICONTROL Permita cambiar esta configuración durante la conversión]**

  Cuando se selecciona esta opción permite que el usuario que convierta el problema pueda cambiar las configuraciones predeterminadas “[!UICONTROL Conservar el problema original]” y “[!UICONTROL Permitir contacto principal]”. Si desea que los valores predeterminados permanezcan sin cambios, anule la selección de esta opción.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Preferencias de fechas reales

En [!DNL Workfront] se usan varios tipos de fechas. Las fechas reales son una “marca de tiempo” que [!DNL Workfront] genera cuando se producen determinados cambios de estado.

Se crea la marca de tiempo [!UICONTROL Fecha de inicio real] cuando el estado del problema cambia de Nuevo a otro estado. Se genera la marca de tiempo [!UICONTROL Fecha de finalización real] cuando el estado del problema cambia a un estado que indica que se ha cerrado.

Es importante tener en cuenta que esta preferencia controla la configuración de fecha real tanto para las tareas como para los problemas.

Ventana de preferencia de ![[!UICONTROL Tareas y problemas] con la sección de [!UICONTROL Fechas reales] resaltada](assets/admin-fund-issue-prefs-actual-dates.png)

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expanda la sección **[!UICONTROL Preferencias de proyecto]** en el panel de menú de la izquierda.
1. Seleccione **[!UICONTROL Tareas y problemas]**.
1. Desplácese hasta la sección **[!UICONTROL Fechas reales]**.
1. Seleccione la opción que desee para **[!UICONTROL Fecha de inicio real]** — [!UICONTROL Ahora] (la fecha y hora actuales) o [!UICONTROL La fecha de inicio planeada] (la [!UICONTROL Fecha de inicio real] coincide con la fecha de inicio establecida en los detalles del problema).
1. Ahora seleccione la opción para **[!UICONTROL Fecha de finalización real]**: [!UICONTROL Ahora] (la fecha y hora actuales) o [!UICONTROL La fecha planificada de finalización] (la [!UICONTROL Fecha de inicio real] coincide con la fecha establecida en los detalles del problema).
1. Guarde cuando haya terminado.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Acceso a problemas

El valor [!UICONTROL Acceso] para problemas controla el acceso que se otorga a un usuario cuando se le asigna un problema en Workfront. Estos ajustes controlan el acceso al problema en sí, además del acceso al proyecto al que está asociado el problema.

Antes de cambiar esta configuración, comente las necesidades de flujos de trabajo o procesos con sus consultores de [!DNL Workfront] y su equipo de administración interna.

Ventana de preferencias de ![[!UICONTROL Tareas y problemas] con la sección [!UICONTROL Cuando alguien está asignado a un PROBLEMA] resaltada](assets/admin-fund-issue-prefs-access-1.png)

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expanda la sección **[!UICONTROL Preferencias de proyecto]** en el panel de menú de la izquierda.
1. Seleccione **[!UICONTROL Tareas y problemas]**.
1. Desplácese hasta la sección **[!UICONTROL Acceso]** y busque “[!UICONTROL Cuando alguien está asignado a un PROBLEMA]”.
1. Establezca el acceso para compartir para el problema en sí: [!UICONTROL Ver], [!UICONTROL Contribuir] o [!UICONTROL Administrar]. [!DNL Workfront] recomienda dejar las opciones avanzadas como están.
1. Marque la casilla si el destinatario del problema también debe tener acceso al proyecto
1. A continuación, seleccione el acceso para compartir para el proyecto: [!UICONTROL Ver], [!UICONTROL Contribuir] o [!UICONTROL Administrar]. A medida que configura las [!UICONTROL Opciones avanzadas], tenga en cuenta los flujos de trabajo de su organización y las necesidades de acceso.
1. Guarde cuando haya terminado.

Ventana de ![[!UICONTROL Acceso] que muestra las opciones [!UICONTROL Contribuir] ](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
