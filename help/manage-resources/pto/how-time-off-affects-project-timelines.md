---
title: Mostrar los días libres afecta a la cronología del proyecto
description: Vea lo que sucede en la cronología del proyecto cuando la configuración de los días libres no está establecida.
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
TQID: https://experienceleague.adobe.com/sN6HqoLl6N-asOtCSlZyKP6W0FSpT0C-7egQTlgAdkY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 525
ht-degree: 100%

---

# Cómo afectan los días libres a las cronologías del proyecto

El hecho de que los días libres de un usuario asignado se tengan en cuenta en la cronología del proyecto depende de la configuración del proyecto denominada [!UICONTROL Días libres del usuario]. Esta configuración determina si los días libres del usuario asignado principal de la tarea se ajusta las fechas planificadas para esa tarea del proyecto.

Veamos lo que sucede con una cronología de proyecto cuando se selecciona una configuración o la otra: [!UICONTROL Considerar los días libres del usuario en las duraciones de las tareas] o [!UICONTROL Ignorar los días libres del usuario en las duraciones de tareas].

![Configuración de los días libres del usuario](assets/toapt_01.png)

## Tenga en cuenta los días libres del usuario en las duraciones de la tarea

Esta opción es la configuración predeterminada de Workfront.

En este ejemplo, el usuario asignado principal de la tarea tiene días de descanso marcados en su calendario personal.

![calendario personal](assets/toapt_02.png)

El administrador de proyectos desea asignar a esta persona a una tarea que tiene fechas planificadas que se superponen con los días libres del usuario.

![tarea de proyecto con fechas](assets/toapt_03.png)

Cuando este usuario está asignado a la tarea, las fechas programadas se ajustan automáticamente. Ahora, la fecha planificada de finalización de la tarea se ha ampliado a varios días para adaptarse a los días libres del usuario. Es importante tener en cuenta que este cambio puede afectar a las fechas planificadas de otras tareas del proyecto y, potencialmente, a la fecha planificada de finalización del proyecto.

![tarea de proyecto con fecha de vencimiento](assets/toapt_04.png)

## [!UICONTROL Ignore los días libres del usuario en las duraciones de la tarea]

Con esta opción, las fechas planificadas de la tarea permanecen como estaban planeadas originalmente, incluso si el usuario asignado principal tiene días libres mientras dura esa tarea.

El miembro del equipo tiene días libres marcados en su calendario.

![Calendario de días libres personales con las fechas marcadas](assets/toapt_05.png)

El administrador del proyecto les asigna una tarea que se superpone con sus días libres. Una vez asignada la tarea el usuario, las fechas planificadas se mantienen según lo planeado originalmente.

![ajustar las fechas de tareas del proyecto](assets/toapt_06.png)

Para asegurar que el trabajo se realice a tiempo, puede resultar útil asignar a otra persona que pueda trabajar en la tarea mientras el usuario asignado original está fuera de la oficina.

## Ajuste la configuración en el nivel de proyecto

Para cambiar la configuración de los días libres del usuario en un proyecto, haga lo siguiente:

* Abra el proyecto haciendo clic en su nombre en Workfront.

* Seleccione [!UICONTROL Editar] en el menú de tres puntos del encabezado de página, a la derecha del nombre del proyecto.

* Desplácese hasta la [!UICONTROL Configuración del proyecto] y busque el campo [!UICONTROL días libres del usuario].

* Seleccione la opción que desee aplicar a este proyecto. [!UICONTROL Considere los días libres del usuario durante las tareas] o [!UICONTROL ignore los días libres del usuario durante tareas].

* Haga clic en el botón [!UICONTROL Guardar] en la esquina superior derecha de la ventana.

![Tenga en cuenta el tiempo libre del usuario en las duraciones de la tarea](assets/toapt_07.png)


**Nota**: Esta configuración no está disponible cuando selecciona [!UICONTROL Detalles del proyecto] en el menú del panel izquierdo de la página del proyecto.

Existe una configuración global para esto en las preferencias del proyecto en el menú [!UICONTROL Configuración]. El administrador del sistema gestiona esta configuración. Es posible que los administradores del grupo puedan ajustar esta configuración para los grupos que administran.

Workfront recomienda que la configuración esté definida de la forma que desea que la mayoría de los proyectos gestione los días libres del personal en su organización.

La configuración también se puede incorporar en plantillas de proyecto a través de los detalles de la plantilla.
