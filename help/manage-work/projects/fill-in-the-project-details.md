---
title: Rellene los detalles del proyecto
description: Descubra qué 12 campos de detalles del proyecto [!DNL  Workfront] recomienda rellenar al crear un proyecto.
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 1%

---

# Rellene los detalles del proyecto

No se preocupe... no tiene que rellenar todos los campos y casillas de verificación de los detalles del proyecto con cada proyecto que cree en [!DNL  Workfront]. Utilice plantillas para rellenar previamente la información y, a continuación, preste atención a los 12 campos de detalles del proyecto más importantes que se enumeran a continuación.

1. **Nombre**

   Un nombre de proyecto descriptivo ayuda a todos a identificar el propósito del proyecto. Asegúrese de seguir la convención de nomenclatura de proyectos de su organización, que puede requerir que se incluya determinada información en el nombre del proyecto (como un número de referencia, un nombre de departamento o un indicador de categoría).


1. **Descripción**

   Cuando varias personas trabajan en un proyecto, usted, como administrador del proyecto, debe asegurarse de que todos estén al día con el propósito y las expectativas del proyecto.

   Haga esto con una descripción del proyecto que proporcione información básica, responda preguntas y permita al equipo del proyecto avanzar con su trabajo. Por ejemplo, &quot;Una campaña destinada a aumentar en un 50% los ingresos que generan trabajo&quot; o &quot;Nueva actualización del sistema para mejorar la eficiencia en todo el departamento&quot;.

   Algunos clientes de Workfront incluyen una muestra del aspecto que debería tener una descripción de proyecto en sus plantillas de proyecto.

1. **Estado**

   El estado se utiliza en Workfront para indicar dónde está un proyecto o en qué fase del flujo de trabajo. El estado se utiliza en muchos informes de Workfront para realizar un seguimiento del progreso del trabajo.

   Workfront recomienda que el estado se establezca en Planificación mientras se desarrolla y finaliza el plan del proyecto. Lo clave con el estado de Planning es que las notificaciones de Workfront no salen a los usuarios asignados de tareas sobre el proyecto mientras está en este estado.

   A continuación, una vez que el proyecto esté listo para ejecutarse, cambie el estado a Actual. Esto permite a Workfront enviar notificaciones a las personas sobre las nuevas tareas a las que están asignadas, pero no envía notificaciones a los usuarios sobre las tareas que se les asignaron mientras el proyecto estaba en estado de Planificación.

   >[!TIP]
   >
   >  Al realizar cambios en el proyecto, como cambiar las fechas de vencimiento, puede revertir el estado a Planning o desactivar la función de guardado automático para evitar que las notificaciones se emitan hasta que se completen los cambios.

   El administrador del sistema puede establecer el estado de Planning como el Workfront global predeterminado para nuevos proyectos.

1. **Modo de horario**

   Los proyectos de Workfront se pueden programar desde una fecha de inicio o de finalización. Esa selección importante determina cómo se calculan las fechas planificadas de cada tarea.

   La opción Fecha de comienzo toma la fecha de comienzo del proyecto (especificada por usted) y la duración y predecesoras de cada tarea para calcular cuándo terminará el proyecto. Workfront recomienda utilizar esta opción, ya que es la más común y facilita la planificación de las fechas de los proyectos.

   Sin embargo, puede utilizar una fecha de finalización. Workfront busca la fecha de finalización (que ha introducido usted) y el trabajo por hacer (en función de las duraciones y predecesoras) y, a continuación, trabaja hacia atrás para calcular la fecha de inicio del proyecto. Workfront recomienda esperar a utilizar la fecha de finalización después de establecer un determinado nivel de competencia en Workfront.

   Sea cual sea la opción que elija, no olvide seleccionar una fecha del calendario emergente.

   La opción Modo de programación se puede establecer en la plantilla.

1. **Grupo**

   Un grupo es una unidad organizativa de Workfront que a menudo se alinea con un departamento. Este campo se puede establecer en la plantilla del proyecto. Si no es así, el campo se establece automáticamente en el grupo de inicio de la persona que crea el proyecto. Puede cambiar el grupo según sea necesario.

   Generalmente, la mayoría de las personas que trabajan en el proyecto provienen de este grupo. Pero esto no restringe a las personas de otros grupos a las que se les asigna trabajo en el proyecto.

   El grupo del proyecto también determina qué preferencias de proyecto, tarea y problema utilizará el proyecto. Estas preferencias, como un estado personalizado para un grupo específico, las establece el administrador del sistema o un administrador del grupo.

   La configuración de grupo es una forma cómoda, a través de los informes, de mostrar todos los proyectos en los que trabaja un departamento.

1. **Propietario del proyecto**

   El propietario del proyecto es el término que utiliza Workfront para designar al administrador de proyectos. Esta es la persona responsable de la planificación y/o gestión del proyecto.

   Para que el propietario del proyecto tenga permisos de administración completos para el proyecto, debe tener una licencia de planificación.

   Normalmente, este campo se deja en blanco en la plantilla y se rellena automáticamente con el nombre de la persona que crea el proyecto. Si se introduce un nombre en la plantilla, ese es el propietario predeterminado del proyecto.

1. **Patrocinador de proyecto**

   El patrocinador del proyecto no es obligatorio, pero cuando se utiliza, suele ser la persona que ha solicitado el proyecto. A menudo se trata de una parte interesada interna, como un administrador o un ejecutivo, con responsabilidad general por el proyecto.

   El patrocinador recibe automáticamente permisos de visualización en el proyecto y debe ser un usuario con licencia de Workfront.

   El patrocinador del proyecto se puede establecer en la plantilla.

1. **Gerente de recursos**

   Los usuarios de Workfront enumerados en este campo pueden utilizar las herramientas de planificación y administración de recursos de Workfront para los proyectos específicos en los que aparecen. Se pueden enumerar hasta 30 nombres en el campo Administrador de recursos, y cada uno debe tener una licencia de planificación.

   El campo Administrador de recursos se puede establecer en la plantilla.

1. **Formularios personalizados**

   Workfront proporciona campos nativos para elementos como el nombre del proyecto y la fecha de inicio. Pero hay información adicional que necesita como jefe de proyecto o que el equipo del proyecto necesitará. Sus datos únicos son igualmente importantes y se pueden almacenar fácilmente en estos formularios. Detalles como fechas de publicación, tamaños de recursos de impresión, canales de envío, etc.

   Los formularios personalizados pueden capturar esta información y se pueden incluir en listas e informes en Workfront, lo que facilita la visualización y edición de la información.

   Los formularios personalizados se pueden adjuntar a las plantillas con antelación.

1. **Programación**

   El trabajo se lleva a cabo las 24 horas del día, ya que muchas empresas tienen empleados en todo el mundo.

   Workfront le permite aplicar una programación común a los proyectos. Las crea el administrador del sistema. Los horarios reflejan los días y horas laborables de sus equipos, además de los días en los que los empleados no trabajarán (como los festivos).

   Como planificador, asegúrese de que está aplicando la programación correcta al proyecto correcto. La configuración de la programación afecta a los cálculos de la cronología y tiene en cuenta los días libres y las zonas horarias.

   La programación asignada al proyecto debe ser la que se aplique a la mayoría de los usuarios asignados de la tarea. Si no se especifica ninguna programación para el proyecto, se utilizará la marcada como predeterminada.

   La programación se puede establecer en la plantilla.

1. **Conjuntos de recursos**

   Los conjuntos de recursos son colecciones de usuarios de Workfront que se necesitan al mismo tiempo para la finalización de proyectos en su organización. Se puede asignar un conjunto de recursos a varios proyectos, lo que significa que hay proyectos que compiten por recursos.

   Tener conjuntos de recursos asignados a un proyecto es un requisito previo para utilizar el Planificador de recursos y otras herramientas de administración de recursos en Workfront.

   Se puede establecer un conjunto de recursos predeterminado en la plantilla.

1. **Acceso al proyecto para visualizadores y colaboradores**

   Cuando a alguien se le concede acceso a un proyecto mediante Compartir, hay tres niveles de permisos que se le pueden otorgar: Ver, Contribuir y Administrar. Cada nivel de permiso permite al usuario ver y hacer determinadas cosas con el proyecto.

   Por ejemplo, hay personas que podrían tener acceso al proyecto pero que no deberían ver la información financiera. Por lo tanto, puede desactivar la opción Ver finanzas para ellos.

   La configuración de acceso se puede establecer en la plantilla.
