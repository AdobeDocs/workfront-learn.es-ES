---
title: Configurar las preferencias globales predeterminadas del problema
description: Obtenga información sobre cómo establecer preferencias de problemas para problemas convertidos, fechas reales y acceso a problemas.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# Configurar las preferencias globales predeterminadas del problema

Varias configuraciones de todo el sistema establecen valores predeterminados sobre cómo se comportan los problemas en determinadas circunstancias en [!DNL Workfront].

Una práctica recomendada es dejar los valores predeterminados globales tal cual y permitir que los jefes de proyecto realicen los ajustes que necesiten en el nivel de proyecto o en las plantillas de proyecto.

Las preferencias del problema global se pueden ajustar, pero se recomienda que usted y su [!DNL Workfront] Los consultores de analizan qué configuraciones son necesarias para los flujos de trabajo, los procesos y las necesidades de creación de informes de su organización. Su asesor también puede ayudarle a comprender qué sucederá si se cambian determinadas configuraciones.

Las preferencias de problema permiten a los administradores del sistema controlar las opciones cuando los problemas se convierten en tareas o proyectos, cómo se calculan las fechas reales y quién obtiene acceso al proyecto cuando se asignan los problemas. Vamos a echar un vistazo a dónde se encuentran esas configuraciones [!DNL Workfront].

## Preferencias de problema convertido

Esta configuración controla lo que sucede con un problema cuando se convierte en una tarea o un proyecto en [!DNL Workfront].

![[!UICONTROL Tareas y problemas] ventana de preferencias con [!UICONTROL Problemas] sección resaltada](assets/admin-fund-issue-prefs-converting.png)

1. Clic **[!UICONTROL Configurar]** en el **[!UICONTROL Menú principal]**.
1. Expanda el **[!UICONTROL Preferencias de proyecto]** en el panel de menú izquierdo.
1. Seleccionar **[!UICONTROL Tareas y problemas]**.
1. Desplácese hasta **[!UICONTROL Problemas]** sección.
1. Haga clic en las opciones deseadas.
1. Guardar cuando haya terminado.

Veamos las opciones de esta sección, para que pueda elegir las opciones adecuadas para su organización.

* **[!UICONTROL Actualizar automáticamente el estado del problema solucionable cuando cambie el estado del objeto de resolución]**

  Esta configuración le permite correlacionar la resolución del problema original con la resolución del nuevo objeto (tarea o proyecto).

  Con esta configuración habilitada (marcada), puede crear estados de problemas personalizados que tengan la misma clave de estado que el estado de una tarea o un proyecto. Cuando la tarea o el proyecto (el objeto solucionable) se establece en el estado personalizado, el cambio también se muestra en el estado del problema.

  Cuando está desactivado, el estado del objeto de resolución se establece automáticamente en el estado predeterminado, en lugar de en los personalizados.

  Para que esta configuración tenga algún efecto, utilice la opción &quot;[!UICONTROL Mantener el problema original y enlazar su solución a la tarea]Se debe seleccionar la opción &quot;.

* **[!UICONTROL Mantener el problema original y la hora es la resolución de la tarea o el proyecto]**

  Cuando se convierte el problema, esto indica [!DNL Workfront] para conservar los problemas originales. El estado del problema cambia a medida que se cambia el estado de la tarea o el proyecto. Una vez que la tarea o el proyecto se han marcado como completos, el problema se marca como resuelto.

  Si esta opción no está activada, el problema original se elimina y solo permanece la tarea o el proyecto convertido.

  Esta configuración afecta a la creación de informes sobre los problemas que se registraron originalmente en un proyecto o que se producen a través de una [!DNL Workfront] cola de solicitudes.

* **[!UICONTROL Permitir que el contacto primario acceda a la tarea o al proyecto]**

  Esto proporciona a la persona que creó el problema original acceso a la tarea o al proyecto creados durante la conversión. Pueden revisar el trabajo, realizar actualizaciones y mantenerse informados de su progreso.

* **[!UICONTROL Permitir cambiar esta configuración durante la conversión]**

  Cuando se selecciona, esta opción establece la configuración predeterminada para &quot;[!UICONTROL Mantener problema original]&quot; y &quot;[!UICONTROL Permitir contacto principal]&quot; puede ser cambiado por el usuario que convierte el problema. Si desea que los valores predeterminados permanezcan sin cambios, anule la selección de esta opción.

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## Preferencias de fechas reales

Se utilizan varios tipos de fechas en [!DNL Workfront]. Las fechas reales son una &quot;marca de tiempo&quot; que [!DNL Workfront] genera cuando se producen ciertos cambios de estado.

El [!UICONTROL Fecha real de inicio] La marca de tiempo se crea cuando el estado del problema cambia de Nuevo a otro estado. El [!UICONTROL Fecha real de finalización] la marca de tiempo se produce cuando el estado del problema cambia a un estado que indica que está cerrado.

Es importante tener en cuenta que esta preferencia controla la configuración de fecha real tanto para las tareas como para los problemas.

![[!UICONTROL Tareas y problemas] ventana de preferencias con [!UICONTROL Fechas reales] sección resaltada](assets/admin-fund-issue-prefs-actual-dates.png)

1. Clic **[!UICONTROL Configurar]** en el **[!UICONTROL Menú principal]**.
1. Expanda el **[!UICONTROL Preferencias de proyecto]** en el panel de menú izquierdo.
1. Seleccionar **[!UICONTROL Tareas y problemas]**.
1. Desplácese hasta **[!UICONTROL Fechas reales]** sección.
1. Seleccione la opción que desee para la **[!UICONTROL Fecha real de inicio]** — [!UICONTROL Ahora] (la fecha y hora actuales) o [!UICONTROL La fecha planificada de inicio] (el [!UICONTROL Fecha real de inicio] coincide con la fecha de inicio establecida en los detalles del problema).
1. Ahora, seleccione la opción para. **[!UICONTROL Fecha real de finalización]** — [!UICONTROL Ahora] (la fecha y hora actuales) o [!UICONTROL Fecha planificada de finalización] (el [!UICONTROL Fecha real de inicio] coincide con la fecha establecida en los detalles del problema).
1. Guardar cuando haya terminado.


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## Acceso al problema

El [!UICONTROL Acceso] la configuración de problemas controla el acceso que se concede a un usuario cuando se le asigna un problema en Workfront. Esta configuración controla el acceso al propio problema, además del acceso al proyecto con el que está asociado.

Antes de cambiar esta configuración, hable con su administrador de flujos de trabajo o procesos [!DNL Workfront] y su equipo de gobierno interno.

![[!UICONTROL Tareas y problemas] ventana de preferencias con [!UICONTROL Cada vez que se asigne a una persona a un PROBLEMA] sección resaltada](assets/admin-fund-issue-prefs-access-1.png)

1. Clic **[!UICONTROL Configurar]** en el **[!UICONTROL Menú principal]**.
1. Expanda el **[!UICONTROL Preferencias de proyecto]** en el panel de menú izquierdo.
1. Seleccionar **[!UICONTROL Tareas y problemas]**.
1. Desplácese hasta **[!UICONTROL Acceso]** y busque la sección &quot;[!UICONTROL Cada vez que se asigne a una persona a un PROBLEMA]Opción &quot;.
1. Configurar el acceso compartido para el propio problema — [!UICONTROL Ver], [!UICONTROL Contribute], o [!UICONTROL Administrar]. [!DNL Workfront] recomienda dejar las opciones avanzadas tal cual.
1. Marque la casilla si el usuario asignado del problema también debe tener acceso al proyecto
1. A continuación, seleccione el acceso compartido para el proyecto — [!UICONTROL Ver], [!UICONTROL Contribute], o [!UICONTROL Administrar]. Al configurar la variable [!UICONTROL Opciones avanzadas], tenga en cuenta los flujos de trabajo de su organización y las necesidades de acceso.
1. Guardar cuando haya terminado.

![[!UICONTROL Acceso] ventana que muestra [!UICONTROL Contribute] opciones](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
