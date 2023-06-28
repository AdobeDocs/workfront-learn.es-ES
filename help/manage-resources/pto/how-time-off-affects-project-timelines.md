---
title: Mostrar los días libres afecta a las escalas de tiempo del proyecto
description: Vea qué sucede con la cronología de un proyecto cuando el tiempo de espera está activado y desactivado.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 4%

---

# Cómo afectan los días libres a las escalas de tiempo del proyecto

Si el tiempo libre de un usuario asignado influye en la cronología del proyecto depende de una configuración de proyecto llamada [!UICONTROL Tiempo libre del usuario]. Esta configuración determina si el tiempo libre para el usuario asignado principal de la tarea ajusta las fechas planificadas para esa tarea en el proyecto.

Veamos lo que sucede con la cronología de un proyecto cuando se selecciona cada una de las configuraciones (C)[!UICONTROL Considere el tiempo libre del usuario en las duraciones de tareas] o [!UICONTROL Omitir tiempo libre del usuario en duraciones de tareas].

![Configuración de tiempo libre del usuario](assets/toapt_01.png)

## Tenga en cuenta el tiempo libre del usuario en las duraciones de la tarea

Esta opción es la configuración predeterminada de Workfront.

En este ejemplo, el usuario asignado principal de la tarea tiene los días libres marcados en su calendario personal.

![calendario personal](assets/toapt_02.png)

El administrador del proyecto desea asignar esta persona a una tarea con fechas planificadas que se superpongan con el tiempo de espera del usuario.

![tarea de proyecto con fechas](assets/toapt_03.png)

Cuando se asigna este usuario a la tarea, las fechas planificadas se ajustan automáticamente. Ahora, la fecha planificada de finalización de la tarea se ha ampliado en varios días para dar cabida al tiempo libre del usuario. Es importante tener en cuenta que este cambio puede afectar a las fechas planificadas de otras tareas del proyecto y, potencialmente, a la fecha planificada de finalización del proyecto.

![tarea de proyecto con fecha de vencimiento](assets/toapt_04.png)

## [!UICONTROL Ignore el tiempo libre del usuario en las duraciones de la tarea]

Con esta opción, las fechas planificadas de la tarea permanecen tal y como estaban planificadas originalmente, incluso si el usuario principal asignado tiene tiempo libre durante la duración de la tarea.

El miembro del equipo tiene días libres marcados en su calendario.

![calendario de pto con fechas marcadas](assets/toapt_05.png)

El jefe de proyecto les asigna una tarea que se superpone con el tiempo libre. Una vez asignado el usuario, las fechas planificadas para la tarea permanecen tal y como estaban planificadas originalmente.

![ajustar fechas de tareas de proyecto](assets/toapt_06.png)

Para asegurarse de que el trabajo se realiza a tiempo, puede resultar útil asignar a otra persona que pueda trabajar en la tarea mientras el usuario asignado original esté fuera de la oficina.

## Ajuste de la configuración en el nivel de proyecto

Para cambiar la configuración de Tiempo libre del usuario en un proyecto:

* Abra el proyecto haciendo clic en su nombre en Workfront.

* Seleccionar [!UICONTROL Editar] en el menú de 3 puntos del encabezado de página, a la derecha del nombre del proyecto.

* Desplácese hasta [!UICONTROL Configuración de proyecto] y busque la sección [!UICONTROL Tiempo libre del usuario] field.

* Seleccione la opción que desee aplicar a este proyecto: [!UICONTROL Considere el tiempo libre del usuario en las duraciones de tareas] o I[!UICONTROL ignorar tiempo libre del usuario en las duraciones de las tareas].

* Haga clic en [!UICONTROL Guardar] en la esquina superior derecha de la ventana.

![Tenga en cuenta el tiempo libre del usuario en las duraciones de la tarea](assets/toapt_07.png)


**Nota**: Esta configuración no está disponible cuando selecciona [!UICONTROL Detalles del proyecto] en el menú del panel izquierdo de la página del proyecto.

Existe una configuración global para esto en las preferencias de proyecto en la [!UICONTROL Configurar] menú. El administrador del sistema administra esta configuración. Los administradores de grupo pueden ajustar esta configuración para los grupos que administran.

Workfront recomienda que la configuración se establezca de la manera que desea que la mayoría de los proyectos administren los días libres en su organización.

La configuración también se puede incorporar en las plantillas de proyecto a través de los detalles de la plantilla.
