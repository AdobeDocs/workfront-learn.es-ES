---
title: Mostrar el tiempo de espera afecta a las líneas de tiempo del proyecto
description: Vea lo que sucede en una línea de tiempo del proyecto cuando el tiempo de configuración está activado y desactivado.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
kt: 10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 4%

---

# Cómo afecta el tiempo de espera a los plazos del proyecto

Si el tiempo de espera de un usuario asignado en la cronología del proyecto depende de la configuración de un proyecto denominada [!UICONTROL Tiempo de espera del usuario desactivado]. Esta configuración determina si el tiempo de espera para el usuario asignado principal de la tarea ajusta las fechas planificadas para esa tarea en el proyecto.

Veamos lo que sucede con una línea de tiempo de proyecto cuando se selecciona cada uno de los ajustes: C[!UICONTROL Considere el tiempo de espera del usuario en las duraciones de las tareas] o [!UICONTROL Ignorar el tiempo de espera del usuario en duraciones de tareas].

![Configuración del tiempo de espera del usuario](assets/toapt_01.png)

## Tenga en cuenta el tiempo libre del usuario en las duraciones de la tarea

Esta opción es la configuración predeterminada de Workfront.

En este ejemplo, el usuario asignado principal de la tarea tiene días de descanso marcados en su calendario personal.

![calendario personal](assets/toapt_02.png)

El administrador de proyectos desea asignar a esta persona a una tarea que tenga fechas planificadas que se superpongan con el tiempo de espera del usuario.

![tarea de proyecto con fechas](assets/toapt_03.png)

Cuando este usuario está asignado a la tarea, las fechas programadas se ajustan automáticamente. Ahora, la fecha de finalización prevista de la tarea se ha ampliado en varios días para adaptarse al tiempo libre del usuario. Es importante tener en cuenta que este cambio puede afectar a las fechas planificadas de otras tareas del proyecto y, potencialmente, a la fecha de finalización prevista del proyecto.

![tarea de proyecto con fecha de vencimiento](assets/toapt_04.png)

## [!UICONTROL Ignore el tiempo libre del usuario en las duraciones de la tarea]

Con esta opción, las fechas planificadas de la tarea permanecen como estaba planeado originalmente, incluso si el usuario asignado principal tiene tiempo libre durante la duración de la tarea.

El miembro del equipo tiene días libres marcados en su calendario.

![Enviar calendario con fechas marcadas](assets/toapt_05.png)

El administrador de proyectos les asigna una tarea que se superpone con el tiempo de espera. Una vez asignado el usuario, las fechas planificadas de la tarea se mantienen según lo planeado originalmente.

![ajustar fechas de tareas del proyecto](assets/toapt_06.png)

Para asegurarse de que el trabajo se realiza a tiempo, puede resultar útil asignar a otra persona que pueda trabajar en la tarea mientras el usuario asignado original está fuera de la oficina.

## Ajuste la configuración en el nivel de proyecto

Para cambiar la configuración de Tiempo de espera de usuario en un proyecto:

* Abra el proyecto haciendo clic en su nombre en Workfront.

* Select [!UICONTROL Editar] en el menú de 3 puntos del encabezado de página, a la derecha del nombre del proyecto.

* Desplácese hasta el [!UICONTROL Configuración del proyecto] y busque [!UICONTROL Tiempo de espera del usuario desactivado] campo .

* Seleccione la opción que desee aplicar a este proyecto — [!UICONTROL Considere el tiempo de espera del usuario en las duraciones de las tareas] o I[!UICONTROL ignorar el tiempo de espera del usuario en duraciones de tareas].

* Haga clic en el [!UICONTROL Guardar] en la esquina superior derecha de la ventana.

![Tenga en cuenta el tiempo libre del usuario en las duraciones de la tarea](assets/toapt_07.png)


**Nota**: Esta configuración no está disponible cuando selecciona [!UICONTROL Detalles del proyecto] en el menú del panel izquierdo de la página del proyecto.

Existe una configuración global para esto en las preferencias del proyecto en la [!UICONTROL Configuración] para abrir el Navegador. El administrador del sistema administra esta configuración. Es posible que los administradores del grupo puedan ajustar esta configuración para los grupos que administran.

Workfront recomienda que la configuración esté definida de la forma que desea que la mayoría de los proyectos gestione el tiempo de espera en su organización.

La configuración también se puede incorporar en plantillas de proyecto a través de los detalles de la plantilla.
