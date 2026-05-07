---
title: 'Práctica recomendada: Solicitar colas'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de colas de solicitudes de Workfront.
feature: Resource Management
role: Admin, Leader, User
level: Beginner
jira: KT-10921
exl-id: dbb961f9-c207-49f1-9545-ec127f983c15
TQID: https://experienceleague.adobe.com/qp6rMfRSCtQfsrU-1zzHWYWrvMnFJAJBYoqXKGP3GeQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 1492
ht-degree: 91%

---

# Práctica recomendada: Solicitar colas

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El área &quot;¿Por qué son estas prácticas recomendadas?&quot;, que se encuentra después de la lista de alto nivel, proporciona más detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de la cola de solicitudes

* Incluya una descripción para cada elemento de una cola de solicitudes: el proyecto de la cola de solicitudes, los grupos de temas, los temas de la cola y las reglas de enrutamiento.

* Cree un estado de proyecto llamado “Cola de solicitudes” u “Operativo” que coincida con “Actual” para distinguir los proyectos de la cola de solicitudes de otros proyectos.

* Si planea utilizar aprobaciones de problemas con solicitudes enviadas a través de una cola, cree un estado de problema llamado Rechazado.

* Asigne formularios personalizados “universales” para solicitar colas para capturar tantos datos coherentes en toda la empresa como sea posible.

* Evite compartir colas de solicitud con “todos”. Configure la configuración de detalles de la cola para que los usuarios solo vean las colas relevantes para sus necesidades.

* Cree y asigne un tablero que contenga informes de cola de solicitudes para que los administradores de tráfico, administradores de sistemas o usuarios asignados puedan trabajar directamente en los problemas.

* Utilice plantillas de diseño para eliminar las opciones de configuración de la cola de solicitudes del menú del panel izquierdo de los proyectos para los usuarios que no necesiten crear colas.

* Cree una cola de solicitudes del administrador del sistema para que los usuarios hagan preguntas relacionadas con Workfront, soliciten configuraciones del sistema, programen nueva formación del usuario, etc.

* Audite las colas de solicitud regularmente para identificar y dejar de compartir las colas que no se están utilizando.

* Utilice grupos de temas para organizar más de 10 temas de cola en una cola de solicitudes y crear listas más cortas y fáciles de administrar.

* Para controlar el número total de colas de solicitud disponibles para los usuarios, desglose una cola de solicitudes mediante grupos de temas y temas de cola, en lugar de crear varias colas.

* Configure las reglas de enrutamiento para cada tema de la cola. Como mínimo, configure una regla de enrutamiento predeterminada.

* Utilice los grupos de temas y los temas de cola cuando sea necesario el enrutamiento selectivo.

* Envía solicitudes a un equipo, en lugar de a un individuo.


</br>
</br>


## ¿Por qué estas son prácticas recomendadas?


**Práctica recomendada**

Incluya una descripción para cada elemento de una cola de solicitudes: el proyecto de la cola de solicitudes, los grupos de temas, los temas de la cola y las reglas de enrutamiento.

**A continuación se explica por qué**

Las descripciones permiten a los administradores de grupos, futuros administradores del sistema u otras personas que mantienen colas de solicitud saber exactamente qué hace cada parte de la cola de solicitudes.

La información de descripción también aparece al pasar el puntero por encima del icono de información del campo en la nueva ventana de solicitud.

La descripción no tiene que ser larga, solo un breve comentario sobre el propósito o el uso del elemento.

</br>
</br>

**Práctica recomendada**

Cree un estado de proyecto llamado “Cola de solicitudes” u “Operativo” que coincida con “Actual” para distinguir los proyectos de la cola de solicitudes de otros proyectos.

**A continuación se explica por qué**

Una cola de solicitud se encuentra en un proyecto y debe tener un estado igual a Actual para que la cola esté activa.

Para distinguir una solicitud de los proyectos de trabajo reales con un estado &quot;Actual&quot;, cree un estado para utilizarlo solo en colas de solicitudes llamadas &quot;Cola de solicitudes&quot; o &quot;Operativo&quot;. A continuación, puede utilizar este estado para ayudar a excluir o incluir proyectos de colas de solicitudes al escribir informes.

</br>
</br>

**Práctica recomendada**

Cree un estado de problema denominado “Rechazado” al utilizar aprobaciones de problemas y establecer la opción Si rechazado en el estado “Rechazado”.

**A continuación se explica por qué**

Al utilizar el estado “Rechazado”, esto deja en claro que la solicitud se revisó y rechazó.

</br>
</br>

**Práctica recomendada**

Asigne formularios personalizados “universales” para solicitar colas para capturar tantos datos coherentes en toda la empresa como sea posible.

**A continuación se explica por qué**

Un formulario personalizado “universal” recopila la información estándar necesaria para la solicitud, independientemente del tipo de solicitud que se envíe.

Tener un formulario personalizado “universal” reduce el número de formularios personalizados que debe crear y mantener. También garantiza que todas las solicitudes recopilen la misma información de la misma manera, lo que conduce a informes y análisis de datos coherentes.

</br>
</br>

**Práctica recomendada**

Evite compartir colas de solicitud con “todos”.  Configure la configuración de detalles de la cola para que los usuarios solo vean las colas relevantes para sus necesidades.

**A continuación se explica por qué**

En la mayoría de los casos, una cola de solicitudes solo debe compartirse con un determinado conjunto de personas, como un equipo, un proveedor, clientes, etc. Cuando los solicitantes ven solo lo que necesitan en la lista de colas de solicitudes, les facilita la búsqueda y la navegación.

</br>
</br>


**Práctica recomendada**

Cree y asigne un tablero que contenga informes de cola de solicitudes para que los administradores de tráfico, administradores de sistemas o usuarios asignados puedan trabajar directamente en los problemas.

**A continuación se explica por qué**

Dar a los usuarios acceso rápido y fácil a las solicitudes entrantes significa que el trabajo no se pierde en la redistribución.

</br>
</br>

**Práctica recomendada**

Utilice plantillas de diseño para eliminar las opciones de configuración de la cola de solicitudes del menú del panel izquierdo de los proyectos para los usuarios que no necesiten crear colas.


**A continuación se explica por qué**

Esto garantiza que todas las colas de solicitud pasen por el proceso adecuado de creación (como ser revisadas por un comité de gobierno) y sean configuradas correctamente por un administrador de sistema o de grupos.

Además, esto mantiene la lista de colas organizada y centrada en los tipos de solicitudes que necesita su organización.

</br>
</br>

**Práctica recomendada**

Cree una cola de solicitudes del administrador del sistema para que los usuarios hagan preguntas relacionadas con Workfront, soliciten configuraciones del sistema, programen nueva formación del usuario, etc.

**A continuación se explica por qué**

Esto proporciona una ubicación centralizada para que los usuarios envíen preguntas y para que los administradores recopilen, supervisen y respondan a los problemas relacionados con Workfront.

Además, esta información se puede utilizar para mostrar al liderazgo el tiempo, esfuerzo y valor de la función del administrador del sistema y como justificación para un administrador del sistema adicional.

</br>
</br>


**Práctica recomendada**

Audite las colas de solicitud regularmente para identificar y dejar de compartir las colas que no se están utilizando.

**A continuación se explica por qué**

Una auditoría periódica de las configuraciones y los elementos del sistema de Adobe Workfront ayuda a mantenerlo ordenado y libre de elementos innecesarios. Si una cola ya no se usa o monitoriza, asegúrese de que los usuarios ya no puedan acceder a ella para que las solicitudes de trabajo no queden en blanco.

</br>
</br>


**Práctica recomendada**

Utilice grupos de temas para organizar más de 10 temas de cola en una cola de solicitudes y crear listas más cortas y fáciles de administrar.

**A continuación se explica por qué**

Los grupos de temas aumentan la adopción por parte del usuario y crean menos confusión al reducir la lista inicial de opciones entre las que seleccionar. Esto permite a los usuarios encontrar fácilmente lo que buscan sin agobiarles al intentar enviar una solicitud.

Además, permite a los administradores de sistemas o a los gestores de cola de solicitudes tener la oportunidad de crear una ruta de navegación fluida para los usuarios y una mejor manera de organizar e informar sobre los tipos de solicitudes que se envían.

</br>
</br>

**Práctica recomendada**

Para controlar el número total de colas de solicitud disponibles para los usuarios, desglose una cola de solicitudes mediante grupos de temas y temas de cola, en lugar de crear varias colas.

**A continuación se explica por qué**

Demasiadas colas de solicitud dificultan a los usuarios encontrar lo que necesitan.

Un menor número de colas también ayuda a los coordinadores de tráfico, administradores de sistemas u otras personas que gestionan las colas, lo que les permite encontrar la información que necesitan más rápidamente, sin tener que navegar a varios proyectos de la cola de solicitudes.

Cree varias colas de solicitud si se necesita un acceso diferente para las colas de solicitud o si la consolidación de colas puede resultar confusa para los usuarios.

</br>
</br>

**Práctica recomendada**

Configure las reglas de enrutamiento para cada tema de la cola. Como mínimo, configure una regla de enrutamiento predeterminada.

**A continuación se explica por qué**

Las reglas de enrutamiento aseguran que a alguien siempre se le asigne la solicitud entrante para que el trabajo no quede relegado a un segundo plano.

</br>
</br>

**Práctica recomendada**

Utilice los grupos de temas y los temas de cola cuando sea necesario el enrutamiento selectivo.

**A continuación se explica por qué**

Las reglas de enrutamiento no se pueden aplicar a campos de un formulario personalizado. Por lo tanto, si es necesario enrutar distintos tipos de solicitudes a diferentes equipos o personas, haga que cada tipo de solicitud tenga su propio tema de grupo de temas o de cola para que el trabajo se pueda enrutar correctamente.

</br>
</br>

**Práctica recomendada**

Envía solicitudes a un equipo, en lugar de a un individuo.

**A continuación se explica por qué**

Cuando se envían solicitudes al equipo, esto da visibilidad a todo el equipo sobre las solicitudes que se están realizando y sobre qué podría implicar el trabajo futuro. Todos pueden ver la página Equipo en busca de nuevos elementos o realizar un seguimiento de las novedades de un informe en un tablero.

También garantiza que cuando el administrador de tráfico u otra persona a cargo de la revisión o asignación de las solicitudes entrantes no esté disponible, una copia de seguridad esté disponible automáticamente y tenga acceso a la información de la solicitud.
