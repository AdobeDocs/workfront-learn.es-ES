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
last-substantial-update: 2025-03-26T00:00:00Z
recommendations: noDisplay,catalog
doc-type: video
exl-id: 9200eeb4-db5d-45c1-9b17-28c6ca04de2d
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 10%

---

# Aplicar un proceso de aprobación de problema en una cola de solicitudes

>[!PREREQUISITES]
>
>* [Crear un flujo de solicitud](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Creación de un proceso de aprobación global y de un solo uso](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


En el vídeo se explica el proceso de aplicación de un proceso de aprobación predeterminado al crear una cola de solicitudes. palo de golf Cuando se crea una solicitud, comienza con el estado &quot;Nuevo - Aprobación pendiente&quot; y se envía una notificación de aprobación al aprobador designado. palo de golf Si se aprueba, el estado cambia a &quot;Nuevo&quot;, lo que permite que las personas asignadas comiencen a trabajar. palo de golf Si se rechaza, el estado puede volver incorrectamente a &quot;Nuevo&quot; debido a un error común en la configuración del proceso de aprobación. palo de golf
El vídeo resalta que el proceso de aprobación se activa cuando el estado se establece en &quot;Nuevo&quot;, que es el predeterminado para las nuevas solicitudes. palo de golf Si se rechaza, el sistema vuelve a cambiar el estado al anterior de forma predeterminada, lo que no es ideal para nuevas solicitudes. palo de golf En su lugar, se debe elegir un estado diferente, como &quot;No se resolverá&quot;. palo de golf El vídeo también indica que no hay un estado &quot;Rechazado&quot; proporcionado de forma predeterminada, pero un administrador del sistema puede crear uno si es necesario. palo de golf

>[!VIDEO](https://video.tv.adobe.com/v/3455027/?quality=12&learn=on&enablevpops=1&captions=spa)

## Puntos clave

* **Proceso de aprobación predeterminado:** Al crear una cola de solicitudes, puede aplicar un proceso de aprobación predeterminado que asigne automáticamente un flujo de trabajo de aprobación a cada solicitud.
* **Cambios de estado tras la aprobación:** Las solicitudes aprobadas cambian su estado de &quot;Nuevo - pendiente de aprobación&quot; a &quot;Nuevo&quot;, lo que permite que las personas asignadas empiecen a trabajar en ellas.
* **Error común en la administración de rechazos:** Si se rechaza una solicitud, el estado volverá a ser &quot;Nuevo&quot; debido a una configuración predeterminada del sistema en el proceso de aprobación.
* **Estado recomendado para las solicitudes rechazadas:** En lugar de volver al estado anterior (&quot;Nuevo&quot;), es mejor elegir un estado diferente, como &quot;No se resuelve&quot;, para evitar confusiones.
* **Opciones de estado personalizado:** No hay ningún estado &quot;Rechazado&quot; proporcionado de forma predeterminada, pero un administrador del sistema puede crear uno si es necesario para una mejor claridad en el proceso de aprobación.


## Tutoriales recomendados sobre este tema

* [Delegar tareas, problemas y aprobaciones](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [Explicación de los procesos de aprobación específicos del grupo](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [Crear un flujo de solicitud](/help/manage-work/request-queues/create-a-request-flow.md)
* [Creación de un proceso de aprobación global y de un solo uso](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
