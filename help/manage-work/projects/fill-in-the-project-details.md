---
title: Rellene los detalles del proyecto
description: Conozca qué 12 campos de detalles del proyecto [!DNL  Workfront] recomienda rellenar al crear un proyecto.
feature: Work Management
thumbnail: fill-in-the-project-details.jpeg
type: Tutorial
role: User
level: Intermediate
kt: 10140
exl-id: a62b9421-627a-4f23-ab66-da1f29114225
source-git-commit: 27e8f0aada77488bd6cfc2e786b997f759fd0a17
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 1%

---

# Rellene los detalles del proyecto

No se preocupe ... no tiene que rellenar todos los campos y casillas de verificación de los detalles del proyecto con cada proyecto que cree en [!DNL  Workfront]. Utilice plantillas para rellenar previamente la información y, a continuación, preste atención a los 12 campos de detalles del proyecto más importantes que se enumeran a continuación.

1. **Nombre**

   Un nombre de proyecto descriptivo ayuda a todos a identificar el propósito del proyecto. Asegúrese de seguir la convención de nomenclatura de proyectos de su organización, que puede requerir que se incluya cierta información en el nombre del proyecto (como un número de referencia, un nombre de departamento o un indicador de categoría).

1. **Descripción**

   Cuando varias personas trabajan en un proyecto, usted (como director del proyecto) debe asegurarse de que todos estén a la altura del propósito y las expectativas del proyecto.

   Haga esto con una descripción del proyecto que proporcione información básica, responda preguntas y permita que el equipo del proyecto avance con su trabajo. Por ejemplo, &quot;Una campaña tiene como objetivo aumentar el trabajo generador de ingresos en un 50%&quot; o &quot;Nuevo upgrade del sistema para mejorar la eficiencia en todo el departamento&quot;.

   Algunos clientes de Workfront incluyen una muestra del aspecto que debe tener la descripción de un proyecto en las plantillas de proyecto.

1. **Estado**

   El estado se utiliza en Workfront para indicar dónde o en qué fase del flujo de trabajo se encuentra un proyecto. El estado se utiliza en muchos informes de Workfront para realizar un seguimiento del progreso del trabajo.

   Workfront recomienda que el estado se establezca en Planning mientras amplía y finaliza el plan de proyecto. Lo principal con el estado de Planning es que las notificaciones de Workfront no van a los destinatarios asignados a tareas sobre el proyecto mientras esté en este estado.

   A continuación, una vez que el proyecto esté listo para ejecutarse, cambie el estado a Actual. Es entonces cuando Workfront envía notificaciones a las personas adecuadas sobre las tareas a las que se les han asignado.

   >[!TIP]
   >
   >  Al realizar cambios en el proyecto (como cambiar las fechas de vencimiento), puede volver a pasar el estado a Planning o desactivar la función de guardado automático para evitar que las notificaciones se publiquen hasta que se hayan completado los cambios.

   El administrador del sistema puede establecer el estado de Planning como Workfront global predeterminado.

1. **Modo de horario**

   Los proyectos de Workfront se pueden programar desde una fecha de inicio o de finalización. Esa selección importante determina cómo se calculan las fechas planificadas de cada tarea.

   La opción Fecha de inicio toma la fecha de inicio del proyecto (introducida por usted) y la duración y los predecesores de cada tarea para calcular cuándo finalizará el proyecto. Workfront recomienda utilizar esta opción, ya que es la más común y facilita la planificación de las fechas del proyecto.

   Sin embargo, puede utilizar una fecha de finalización. Workfront observa la fecha de finalización (introducida por usted) y el trabajo que se va a realizar (en función de las duraciones y predecesores) y, a continuación, trabaja hacia atrás para calcular la fecha de inicio del proyecto. Workfront recomienda esperar a utilizar la fecha de finalización después de establecer un cierto nivel de competencia en Workfront.

   Sea cual sea la opción que elija, no olvide seleccionar una fecha del calendario emergente.

   La opción Modo de programación se puede configurar en la plantilla.

1. **Grupo**

   Un grupo es una unidad organizativa de Workfront que a menudo se alinea con un departamento. Este campo se puede establecer en la plantilla del proyecto. Si no es así, el campo se establece automáticamente en el grupo de inicio de la persona que crea el proyecto. Puede cambiar el grupo según sea necesario.

   Generalmente, la mayoría de las personas que trabajan en el proyecto provienen de este grupo. Sin embargo, esto no restringe a las personas de otros grupos a los que se asigna trabajo en el proyecto.

   El grupo del proyecto también determina qué proyecto, tarea y preferencias de problema usará el proyecto. Estas preferencias, como un estado personalizado para un grupo específico, las establece el administrador del sistema o un administrador del grupo.

   La configuración del grupo es una manera conveniente, a través de los informes, de mostrar todos los proyectos en los que trabaja un departamento.

1. **Propietario del proyecto**

   El propietario del proyecto es el término que Workfront emplea para el administrador del proyecto. Es la persona responsable de la planificación y/o gestión del proyecto.

   El propietario del proyecto tiene permisos de administración completos en el proyecto, por lo que debe tener una licencia del plan.

   Normalmente, este campo se deja en blanco en la plantilla y rellena automáticamente con el nombre de la persona que crea el proyecto. Si se introduce un nombre en la plantilla, ese es el propietario predeterminado del proyecto.

1. **Patrocinador de proyecto**

   El patrocinador del proyecto es generalmente la persona que solicitó el proyecto. A menudo se trata de una parte interesada interna, como un administrador o un ejecutivo, que tiene la responsabilidad general del proyecto.

   El patrocinador recibe automáticamente permisos de visualización para el proyecto y debe ser un usuario con licencia de Workfront.

   El patrocinador del proyecto se puede establecer en la plantilla.

1. **Gerente de recursos**

   Los usuarios de Workfront enumerados en este campo pueden utilizar las herramientas de planificación y administración de recursos de Workfront para los proyectos específicos en los que aparecen en la lista. Se pueden enumerar hasta 30 nombres en el campo Administrador de recursos y cada uno debe tener una licencia de Plan.

   El campo Administrador de recursos se puede establecer en la plantilla.

1. **Formularios personalizados**

   Workfront proporciona campos nativos para cosas como el nombre del proyecto y la fecha de inicio. Pero hay información adicional que necesita como administrador de proyectos o que necesitará el equipo del proyecto. Los datos únicos son igualmente importantes y se pueden almacenar fácilmente en estos formularios. Detalles como fechas de publicación, tamaño de recurso de impresión, canales de envío, etc.

   Los formularios personalizados pueden capturar esta información y se pueden incluir en listas e informes de Workfront, lo que facilita la visualización y edición de la información.

   Los formularios personalizados se pueden adjuntar a las plantillas con antelación.

1. **Horario**

   El trabajo se realiza las 24 horas del día, ya que muchas empresas tienen empleados en todo el mundo.

   Workfront le permite aplicar una programación común a los proyectos. Los crea el administrador del sistema. Las programaciones reflejan los días y las horas de trabajo de los equipos, además de los días en que los empleados no estarán trabajando (por ejemplo, días festivos).

   Como planificador, asegúrese de que está aplicando la programación correcta al proyecto correcto. La configuración de programación afecta a los cálculos de la cronología, teniendo en cuenta el tiempo de espera y las zonas horarias.

   La programación asignada al proyecto debe ser la que se aplique a la mayoría de los asignadores de tareas. Si no se especifica ninguna programación para el proyecto, se utilizará la programación marcada como Predeterminada.

   La programación se puede configurar en la plantilla.

1. **Conjuntos de recursos**

   Los grupos de recursos son colecciones de usuarios de Workfront que se necesitan al mismo tiempo para completar proyectos en su organización. Se puede asignar un grupo de recursos a varios proyectos, lo que significa que tiene proyectos que compiten por los recursos.

   Tener grupos de recursos asignados a un proyecto es un requisito previo para usar el Planificador de recursos y otras herramientas de administración de recursos en Workfront.

   Se puede configurar un grupo de recursos predeterminado en la plantilla.

1. **Acceso al proyecto para visualizadores y colaboradores**

   Cuando alguien tiene acceso a un proyecto, hay tres niveles de permisos que se pueden otorgar inicialmente cuando un proyecto se pone en marcha: Ver, Contribuir y Administrar. Cada nivel de permiso permite al usuario ver y realizar ciertas cosas con el proyecto.

   Por ejemplo, hay personas que pueden tener acceso al proyecto pero no deberían ver la información financiera. De este modo, puede desactivar la opción Ver finanzas para visualizadores y colaboradores.

   Puede ajustar esta configuración de permisos en proyectos individuales en cualquier momento. Sin embargo, una vez que un proyecto ha pasado de Planning al estado actual, los ajustes basados en permisos deben realizarse a través del proyecto Compartido.

   La configuración de acceso se puede establecer en la plantilla .
