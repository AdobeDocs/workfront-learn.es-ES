---
title: Respuestas a preguntas comunes sobre las colas de solicitud
description: Obtenga respuestas a preguntas comunes sobre las colas de solicitud en [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner
last-substantial-update: 2024-09-16T00:00:00Z
recommendations: noDisplay,noCatalog
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: e9a4f2bcd39e2598ff540bb4f300e891e817e939
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 50%

---

# Respuestas a preguntas comunes sobre las colas de solicitud

**¿Por qué puedo ver una cola de solicitudes, pero mi usuario no?**

En la pestaña [!UICONTROL Detalles de cola] de la cola de solicitudes/proyecto, asegúrese de que el usuario se ajusta a los criterios del campo “¿Quién puede añadir solicitudes a esta cola?” .

Vea este vídeo para obtener más información:

>[!VIDEO](https://video.tv.adobe.com/v/3434156/?quality=12&learn=on)

**Otorgue a los usuarios acceso a la cola, pero ahora también pueden ver el proyecto de cola de solicitudes. ¿Por qué?**

En la sección &quot;¿Quién puede agregar solicitudes a esta cola?&quot; , si elige &quot;Personas con acceso de visualización en este proyecto&quot;, cualquier persona a la que conceda derechos de visualización para utilizar la cola de solicitudes también podrá ver la cola de solicitudes en una lista de proyectos. Para evitarlo, utilice las opciones &quot;Personas en la compañía de este proyecto&quot; o &quot;Personas en el grupo de este proyecto&quot;.

**¿Puedo convertir una solicitud en un proyecto?**

Sí. Puede convertir problemas en tareas o proyectos según lo que necesite.

Estos tutoriales le mostrarán cómo:

* [Convertir un problema/solicitud en un proyecto](/help/manage-work/issues-requests/create-a-project-from-a-request.md)

* [Convertir un problema/solicitud en una tarea](/help/manage-work/issues-requests/convert-issues-to-other-work-items.md)

**¿Dónde encuentro una cola de solicitudes para realizar ediciones?**

Puede usar el campo [!UICONTROL Buscar] en la barra de navegación o localícela en el área [!UICONTROL Proyectos].

Si abre una solicitud desde la cola de solicitudes, puede hacer clic en el nombre del proyecto en el área de rutas de exploración.

**¿Puedo transferir la información de un formulario personalizado de solicitud a un proyecto?**

Sí. Al crear un formulario personalizado, seleccione ambas [!UICONTROL Proyecto] y [!UICONTROL Problema] como tipos de objeto. También puede editar un formulario personalizado de proyecto para incluir el tipo de objeto de problema y viceversa.

Adjunte el formulario personalizado a la solicitud. Al convertir la solicitud en un proyecto, el formulario personalizado se adjuntará automáticamente al nuevo proyecto y los valores contenidos en cualquier campo aparecerán tanto en los formularios personalizados de solicitud como del proyecto.

**Estoy viendo un informe de proyecto o tarea. ¿Cómo puedo averiguar de qué solicitud se ha originado este objeto?**

Puede acceder a los campos en los orígenes de campo **[!UICONTROL Problema convertido]** y **[!UICONTROL Generador de problema convertido]** para añadir esta información a los informes de proyecto y tarea.

Vea este vídeo para obtener más información:

>[!VIDEO](https://video.tv.adobe.com/v/3434176/?quality=12&learn=on)


**¿Cuál es la mejor manera de filtrar por colas de solicitud en un informe?**

Si el filtro del proyecto incluye **Cola>>Es pública>>Igual a>>Ninguna** el informe solo mostrará los proyectos que **NO** son colas de solicitud.

Si el filtro del proyecto incluye **Cola>>Es pública>>No es igual a>>Ninguna** el informe solo mostrará los proyectos que **SON** colas de solicitud.

Vea este vídeo para obtener más información:

>[!VIDEO](https://video.tv.adobe.com/v/3434329/?quality=12&learn=on)

**¿Es buena idea crear un estado personalizado de la cola de solicitudes?**

Algunos clientes crean un estado personalizado de Cola de solicitudes que equivale a Actual. Pueden ejecutar un informe que muestre todas las colas de solicitudes o excluir fácilmente las colas de solicitudes de un informe. Aunque esto tiene la ventaja de ser más fácil de usar que **Cola>>Es pública>>No es igual>>Ninguna**, tiene la desventaja de que las personas que crean colas de solicitudes pueden olvidarse de usarlo, ya que el estado Actual funciona igual de bien y es lo que verán en la mayoría del material de formación. Por este motivo, muchos clientes eligen no utilizar un estado personalizado de Cola de solicitudes.

Sin embargo, si ya está usando el estado de la cola de solicitudes en su organización y solo desea una forma de asegurarse de que se está usando correctamente (o corregir casos en los que no lo esté), puede crear el informe **colas de solicitudes activas** descrito en el vídeo anterior y cambiar el filtro de **Proyecto>>Estado es igual a>>Igual>>Actual** a **Proyecto>>Estado>>Igual>>Actual**. Esto mostrará todas las colas de solicitudes activas que están utilizando el estado Actual en lugar del estado de la Cola de solicitudes que desea que utilicen. Seleccione todos los proyectos que aparecen y realice una edición masiva para cambiar los estados a Cola de solicitudes.

## Tutoriales recomendados sobre este tema

* [Explicación de las colas de solicitud](/help/manage-work/request-queues/understand-request-queues.md)
* [Crear una cola de solicitudes](/help/manage-work/request-queues/create-a-request-queue.md)
* [Explicación de la configuración de una solicitud de flujo](/help/manage-work/request-queues/understand-settings-for-a-flow-request.md)
* [Crear un flujo de solicitud](/help/manage-work/request-queues/create-a-request-flow.md)
* [Crear una cola de solicitudes de comentarios de administrador del sistema](/help/manage-work/request-queues/create-a-system-admin-feedback-request-queue.md)
