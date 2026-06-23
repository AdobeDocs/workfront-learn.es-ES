---
title: Aplicar un proceso de aprobación de problema en una cola de solicitudes
description: Implemente un proceso de aprobación predeterminado para optimizar los flujos de trabajo de solicitud, lo que garantiza que las solicitudes aprobadas cambien su estado correctamente a "Nuevo". Aborde la confusión de las solicitudes rechazadas seleccionando un cambio de estado a "No se resuelve".
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: '2025-03-26T00:00:00.000Z'
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T15:58:59.618Z'
source-git-commit: 03d522789acef5234d60733543ad10bf4bb8e092
workflow-type: tm+mt
source-wordcount: 291
ht-degree: 24%

---

# Aplicar un proceso de aprobación de problema en una cola de solicitudes

>[!PREREQUISITES]
>
>* [Crear un flujo de solicitud en Workfront](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Crear y administrar procesos de aprobación](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


En el vídeo se explica el proceso de aplicación de un proceso de aprobación predeterminado al crear una cola de solicitudes. Cuando se crea una solicitud, comienza con el estado &quot;Nuevo - Pendiente de aprobación&quot; y se envía una notificación de aprobación al aprobador designado. Si se aprueba, el estado cambia a &quot;Nuevo&quot;, lo que permite que las personas asignadas comiencen a trabajar. Si se rechaza, el estado puede volver incorrectamente a &quot;Nuevo&quot; debido a un error común en la configuración del proceso de aprobación. palo de golf
El vídeo resalta que el proceso de aprobación se activa cuando el estado se establece en &quot;Nuevo&quot;, que es el predeterminado para las nuevas solicitudes. Si se rechaza, el sistema vuelve a cambiar el estado al anterior de forma predeterminada, lo que no es ideal para nuevas solicitudes. En su lugar, se debe elegir un estado diferente, como &quot;No se resolverá&quot;. El vídeo también indica que no hay un estado &quot;Rechazado&quot; proporcionado de forma predeterminada, pero un administrador del sistema puede crear uno si es necesario. palo de golf

>[!VIDEO](https://video.tv.adobe.com/v/3455027/?captions=spa&quality=12&learn=on&enablevpops=1)

## Principales conclusiones

* **Proceso de aprobación predeterminado:** Al crear una cola de solicitudes, puede aplicar un proceso de aprobación predeterminado que asigne automáticamente un flujo de trabajo de aprobación a cada solicitud.
* **Cambios de estado tras la aprobación:** Las solicitudes aprobadas cambian su estado de &quot;Nuevo - pendiente de aprobación&quot; a &quot;Nuevo&quot;, lo que permite que las personas asignadas empiecen a trabajar en ellas.
* **Error común en la administración de rechazos:** Si se rechaza una solicitud, el estado volverá a ser &quot;Nuevo&quot; debido a una configuración predeterminada del sistema en el proceso de aprobación.
* **Estado recomendado para las solicitudes rechazadas:** En lugar de volver al estado anterior (&quot;Nuevo&quot;), es mejor elegir un estado diferente, como &quot;No se resuelve&quot;, para evitar confusiones.
* **Opciones de estado personalizado:** No hay ningún estado &quot;Rechazado&quot; proporcionado de forma predeterminada, pero un administrador del sistema puede crear uno si es necesario para una mejor claridad en el proceso de aprobación.


## Tutoriales recomendados sobre este tema

* [Delegar tareas, problemas y aprobaciones de forma eficaz](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Explicación de los procesos de aprobación específicos del grupo](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Creación de un flujo de solicitud en Workfront](/help/manage-work/request-queues/create-a-request-flow.md)
* [Creación y administración de procesos de aprobación](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)

