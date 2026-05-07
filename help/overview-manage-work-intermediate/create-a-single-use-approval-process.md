---
title: Crear un proceso de aprobación global y de un solo uso
description: Obtenga información sobre cómo crear un proceso de aprobación global y de un solo uso en un proyecto, tarea o problema.
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-8962
hide: true
doc-type: video
exl-id: e80dd36f-7aab-4cf1-873c-92dba684c13c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:20:03.459Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 448
ht-degree: 95%

---

# Crear un proceso de aprobación global y de un solo uso

Los procesos de aprobación de proyectos, tareas y problemas permiten al administrador de proyectos obtener la confirmación por parte de los expertos de que el trabajo se ha realizado justo antes de continuar. El administrador del proyecto puede crear un proceso de aprobación para cada situación (lo que se conoce como proceso de aprobación de un solo uso) o elegir de una lista de, posiblemente, muchos procesos de aprobación que se hayan creado previamente para satisfacer necesidades comunes (se conocen como procesos de aprobación globales).

En cualquier caso, cuando el estado del objeto cambia a uno especificado en el proceso de aprobación, se notifica al aprobador de varias formas para que revise el trabajo y lo apruebe o rechace. Dado que todo el proyecto puede estar en pausa a la espera de una aprobación, los aprobadores deben saber de antemano que se les puede pedir una aprobación. Si un aprobador se encuentra fuera de la oficina por cualquier motivo, puede delegar sus aprobaciones a un sustituto cualificado. Consulte [Delegar tareas, problemas y aprobaciones](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md) para obtener más información.

En este vídeo, aprenderá a crear un proceso de aprobación global y un proceso de aprobación de un solo uso en un proyecto, tarea o problema.

>[!VIDEO](https://video.tv.adobe.com/v/3434690/?captions=spa&quality=12&learn=on&enablevpops=1)

>[!TIP]
>
>Puede añadir un proceso de aprobación de un solo uso a una plantilla de proyecto.

>[!NOTE]
>
>Puede configurar una aprobación de un solo uso en proyectos y problemas del mismo modo que se describe para las tareas en el vídeo.

## Cómo aplicar aprobaciones automáticas de problemas en una cola de solicitudes

Si quiere configurar aprobaciones automáticas de problemas en una cola de solicitudes, estas solo pueden realizarse mediante un proceso de aprobación global de problemas y aplicarse en un [!UICONTROL tema de la cola].

Al crear o editar un [!UICONTROL tema de la cola], seleccione el proceso de aprobación global en el campo **[!UICONTROL Aprobación predeterminada]**.

![Imagen que muestra cómo seleccionar un proceso de aprobación predeterminado en un tema de la cola](assets/automatic-issue-approval-1.png)

Es posible que necesite editar el proceso de aprobación del problema para asegurarse de que el **[!UICONTROL Estado anterior]** no corresponde al del problema establecido cuando se rechaza la aprobación. Esto se debe a que el estado anterior es **[!UICONTROL Nuevo]** y este también es el estado que acciona el proceso de aprobación, por lo que es el estado que se establecerá cuando se apruebe. Para evitar confusiones cuando se rechaza la aprobación del problema, es mejor establecer un estado como **[!UICONTROL No se puede resolver]** o un estado personalizado creado para este fin.

![Imagen que muestra el cambio de estado que se usará cuando se rechace el problema](assets/automatic-issue-approval-2.png)


## Tutoriales recomendados sobre este tema

* [Delegar tareas, problemas y aprobaciones](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Explicación de los procesos de aprobación específicos del grupo](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Crear un flujo de solicitud](/help/manage-work/request-queues/create-a-request-flow.md)

