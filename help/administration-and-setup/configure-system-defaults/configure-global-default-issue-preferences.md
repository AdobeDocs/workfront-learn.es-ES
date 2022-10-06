---
title: Configurar las preferencias de problemas predeterminadas globales
description: Obtenga información sobre cómo establecer las preferencias de problemas para problemas convertidos, fechas reales y acceso a problemas.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 3ded3fe9d8b97b1c11cb382f8088930842399c98
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Configuración de las preferencias de problemas predeterminadas globales

Varias configuraciones de todo el sistema establecen valores predeterminados para el comportamiento de los problemas en determinadas circunstancias en [!DNL Workfront].

Una práctica recomendada es dejar los valores predeterminados globales tal cual y permitir a los directores de proyectos realizar los ajustes que necesiten en el nivel de proyecto o en las plantillas de proyecto.

Las preferencias del problema global se pueden ajustar, pero se recomienda que usted y sus [!DNL Workfront] consulte qué configuración se necesita para los flujos de trabajo, los procesos y las necesidades de creación de informes de su organización. El consultor también puede ayudarle a comprender qué ocurrirá si se cambian determinadas opciones de configuración.

Las preferencias de problemas permiten a los administradores del sistema controlar las opciones cuando los problemas se convierten en tareas o proyectos, cómo se calculan las fechas reales y quién obtiene acceso al proyecto cuando se asignan problemas. Echemos un vistazo a dónde se encuentra esa configuración [!DNL Workfront].

## Preferencias de emisión convertidas

Estos ajustes controlan lo que ocurre con un problema cuando se convierte en una tarea o un proyecto en [!DNL Workfront].

![[!UICONTROL Tareas y problemas] ventana preferencias con [!UICONTROL Problemas] sección resaltada](assets/admin-fund-issue-prefs-converting.png)

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expanda el **[!UICONTROL Preferencias de proyecto]** en el panel de menú de la izquierda.
1. Select **[!UICONTROL Tareas y problemas]**.
1. Desplácese hasta el **[!UICONTROL Problemas]** para obtener más información.
1. Haga clic en las opciones que desee.
1. Guarde cuando haya terminado.

Veamos las opciones de esta sección para que pueda elegir las opciones adecuadas para su organización.

* **[!UICONTROL Actualizar automáticamente el estado del problema resuelto cuando cambia el estado del objeto resuelto]**

   Esta configuración permite correlacionar la resolución del problema original con la resolución del nuevo objeto (tarea o proyecto).

   Con esta configuración habilitada (marcada), puede crear estados de problemas personalizados que tengan la misma clave de estado que una tarea o estado del proyecto. Cuando la tarea o el proyecto (el objeto resoluble) se establece en el estado personalizado, el cambio también se muestra en el estado del problema.

   Cuando está desactivado, el estado del objeto de resolución se establece automáticamente en el estado predeterminado, no en el personalizado.

   Para que esta configuración tenga algún efecto, la variable[!UICONTROL Mantenga el problema original y vincule su resolución a la tarea]&quot; debe estar seleccionada.

* **[!UICONTROL Mantenga el problema original y vincule la resolución a la tarea/proyecto]**

   Cuando se convierte el problema, esto indica [!DNL Workfront] para conservar los problemas originales. El estado del problema cambia a medida que se cambia el estado de la tarea o del proyecto. Una vez que la tarea o el proyecto se ha marcado como completado, el problema se marca como resuelto.

   Si no se selecciona esta opción, se elimina el problema original y solo permanece la tarea o proyecto convertido.

   Esta configuración afecta a los informes sobre los problemas que originalmente se iniciaron en un proyecto o que se producen a través de un [!DNL Workfront] cola de solicitudes.

* **[!UICONTROL Permitir que el contacto principal tenga acceso a la tarea/proyecto]**

   Esto da acceso a la persona que creó el problema original a la tarea o al proyecto creado durante la conversión. Pueden revisar el trabajo, hacer actualizaciones y mantenerse informados de su progreso.

* **[!UICONTROL Permitir cambiar esta configuración durante la conversión]**

   Cuando se selecciona, esta opción significa la configuración predeterminada para &quot;[!UICONTROL Conservar el problema original]&quot; y &quot;[!UICONTROL Permitir contacto principal]&quot; puede cambiarlo el usuario que convierta el problema. Si desea que los valores predeterminados permanezcan sin cambios, anule la selección de esta opción.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Preferencias de fechas reales

Hay varios tipos de fechas que se utilizan en [!DNL Workfront]. Las fechas reales son una &quot;marca de tiempo&quot; que [!DNL Workfront] se genera cuando se producen determinados cambios de estado.

La variable [!UICONTROL Fecha de inicio real] la marca de tiempo se crea cuando el estado del problema cambia de Nuevo a otro estado. La variable [!UICONTROL Fecha de finalización real] la marca de tiempo se produce cuando el estado del problema cambia a un estado que indica que se ha cerrado.

Es importante tener en cuenta que esta preferencia controla la configuración de fecha real tanto para las tareas como para los problemas.

![[!UICONTROL Tareas y problemas] ventana preferencias con [!UICONTROL Fechas reales] sección resaltada](assets/admin-fund-issue-prefs-actual-dates.png)

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expanda el **[!UICONTROL Preferencias de proyecto]** en el panel de menú de la izquierda.
1. Select **[!UICONTROL Tareas y problemas]**.
1. Desplácese hasta el **[!UICONTROL Fechas reales]** para obtener más información.
1. Seleccione la opción que desee para la variable **[!UICONTROL Fecha de inicio real]** — [!UICONTROL Ahora] (la fecha y hora actuales) o [!UICONTROL La fecha de inicio planeada] (el [!UICONTROL Fecha de inicio real] coincide con la fecha de inicio establecida en los detalles del problema).
1. Ahora seleccione la opción para la variable **[!UICONTROL Fecha de finalización real]** — [!UICONTROL Ahora] (la fecha y hora actuales) o [!UICONTROL La fecha de finalización prevista] (el [!UICONTROL Fecha de inicio real] coincide con la fecha establecida en los detalles del problema).
1. Guarde cuando haya terminado.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Acceso a problemas

La variable [!UICONTROL Acceso] la configuración de problemas controla el acceso que se concede a un usuario cuando se le asigna un problema en Workfront. Estos ajustes controlan el acceso al problema en sí, además del acceso al proyecto al que está asociado el problema.

Antes de cambiar esta configuración, comente con su [!DNL Workfront] consultores y su equipo de administración interna.

![[!UICONTROL Tareas y problemas] ventana preferencias con [!UICONTROL Cuando alguien está asignado a un problema] sección resaltada](assets/admin-fund-issue-prefs-access-1.png)

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expanda el **[!UICONTROL Preferencias de proyecto]** en el panel de menú de la izquierda.
1. Select **[!UICONTROL Tareas y problemas]**.
1. Desplácese hasta el **[!UICONTROL Acceso]** y busque &quot;[!UICONTROL Cuando alguien está asignado a un problema]&quot;.
1. Establezca el acceso para compartir para el problema en sí — [!UICONTROL Ver], [!UICONTROL Contribute]o [!UICONTROL Administrar]. [!DNL Workfront] recomienda dejar las opciones avanzadas tal cual.
1. Marque la casilla si el destinatario del problema también debe tener acceso al proyecto.
1. A continuación, seleccione el acceso para compartir para el proyecto — [!UICONTROL Ver], [!UICONTROL Contribute]o [!UICONTROL Administrar]. A medida que configura la variable [!UICONTROL Opciones avanzadas], tenga en cuenta los flujos de trabajo de su organización y las necesidades de acceso.
1. Guarde cuando haya terminado.

![[!UICONTROL Acceso] ventana mostrada [!UICONTROL Contribute] opciones](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
