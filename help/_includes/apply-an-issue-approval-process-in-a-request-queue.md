---
source-git-commit: b150105844a42e06f5e96f787ad62a1b62185f91
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 18%

---
# Aplicar un proceso de aprobación de problema en una cola de solicitudes: COMPARTIDO

>[!PREREQUISITES]
>
>* [Crear un flujo de solicitud en Workfront](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [Crear y administrar procesos de aprobación](https://experienceleague.adobe.com/es/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


En el vídeo se explica el proceso de aplicación de un proceso de aprobación predeterminado al crear una cola de solicitudes. Cuando se crea una solicitud, comienza con el estado &quot;Nuevo - Pendiente de aprobación&quot; y se envía una notificación de aprobación al aprobador designado. Si se aprueba, el estado cambia a &quot;Nuevo&quot;, lo que permite que las personas asignadas comiencen a trabajar. Si se rechaza, el estado puede volver incorrectamente a &quot;Nuevo&quot; debido a un error común en la configuración del proceso de aprobación. &#x200B;
El vídeo resalta que el proceso de aprobación se activa cuando el estado se establece en &quot;Nuevo&quot;, que es el predeterminado para las nuevas solicitudes. Si se rechaza, el sistema vuelve a cambiar el estado al anterior de forma predeterminada, lo que no es ideal para nuevas solicitudes. En su lugar, se debe elegir un estado diferente, como &quot;No se resolverá&quot;. El vídeo también indica que no hay un estado &quot;Rechazado&quot; proporcionado de forma predeterminada, pero un administrador del sistema puede crear uno si es necesario. &#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops=1)

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

