---
title: Respuestas a preguntas comunes sobre las colas de solicitud
description: Obtenga respuestas a preguntas comunes sobre las colas de solicitud en [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner, Intermediate
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ce2aad1cd0ecb7d568ed9a01d97147cbd126ca05
workflow-type: ht
source-wordcount: '414'
ht-degree: 100%

---

# Preguntas frecuentes sobre las colas de solicitud

**¿Por qué puedo ver una cola de solicitudes, pero mi usuario no?**

En la pestaña [!UICONTROL Detalles de cola] de la cola de solicitudes/proyecto, asegúrese de que el usuario se ajusta a los criterios del campo “¿Quién puede añadir solicitudes a esta cola?” .

**Otorgue a los usuarios acceso a la cola, pero ahora también pueden ver el proyecto de cola de solicitudes. ¿Por qué?**

Esto tiene que ver con cómo les otorgó acceso a la cola de solicitudes.

Si ha utilizado la herramienta [!UICONTROL Uso compartido] de la página de aterrizaje del proyecto de la cola de solicitudes y, a continuación, ha otorgado a estos usuarios acceso para ver el proyecto en la lista de proyectos.

Sin embargo, si desea que solo tengan acceso para enviar una solicitud a la cola, vaya a Configuración de cola y seleccione la opción adecuada en “Quién puede añadir solicitudes a este proyecto”.

**¿Puedo convertir una solicitud en un proyecto?**

Sí. Puede convertir problemas en tareas o proyectos según lo que necesite.

Consulte este artículo para obtener más información: [Convertir problemas](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=es).

**¿Dónde encuentro una cola de solicitudes para realizar ediciones?**

Puede usar el campo [!UICONTROL Buscar] en la barra de navegación o localícela en el área [!UICONTROL Proyectos].

Si abre una solicitud desde la cola de solicitudes, puede hacer clic en el nombre del proyecto en el área de rutas de exploración.

**¿Puedo transferir la información de un formulario personalizado de solicitud a un proyecto?**

Sí. Al crear un formulario personalizado, seleccione ambas [!UICONTROL Proyecto] y [!UICONTROL Problema] como tipos de objeto. Adjunte el formulario personalizado a la solicitud. Al convertir la solicitud en un proyecto, el formulario personalizado se adjuntará automáticamente al nuevo proyecto y los valores contenidos en cualquier campo aparecerán tanto en los formularios personalizados de solicitud como del proyecto.

**Estoy viendo un informe de proyecto o tarea. ¿Cómo puedo averiguar de qué solicitud se ha originado este objeto?**

Puede acceder a los campos en los orígenes de campo **[!UICONTROL Problema convertido]** y **[!UICONTROL Generador de problema convertido]** para añadir esta información a los informes de proyecto y tarea.

**¿Cuál es la mejor manera de filtrar por colas de solicitud en un informe?**

Si el filtro del proyecto incluye **Cola>>Es pública>>Igual a>>Ninguna** el informe solo mostrará los proyectos que **NO** son colas de solicitud.

Si el filtro del proyecto incluye **Cola>>Es pública>>No es igual a>>Ninguna** el informe solo mostrará los proyectos que **SON** colas de solicitud.
