---
title: 'Práctica recomendada: licencias y niveles de acceso'
description: Explore las prácticas recomendadas por los expertos de Adobe Workfront para configurar, administrar y utilizar las licencias y los niveles de acceso de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 0%

---

# Práctica recomendada: licencias y niveles de acceso

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de licencias y niveles de acceso

* Comience con menos acceso para los usuarios al configurar los niveles de acceso.

* Al asignar licencias de revisión y solicitud, el valor predeterminado suele ser Revisar porque proporciona al usuario más permisos en Adobe Workfront.

* Desmarque la casilla &quot;Compartir en todo el sistema&quot; en cada objeto de todos sus niveles de acceso a menos que desee que esos usuarios puedan hacerlo.

* Considere la posibilidad de activar la opción &quot;Nunca permitir que los usuarios eliminen comentarios&quot; en Establecer restricciones adicionales en un nivel de acceso.

* Limite el número de administradores del sistema en favor de los administradores del grupo.

* Copie un nivel de acceso existente y realice modificaciones, en lugar de crear un nuevo nivel de acceso desde cero.

* Documente lo que cada nivel de acceso puede hacer en el cuadro Descripción.

* Limítese únicamente a los niveles de acceso necesarios para lograr sus objetivos de trabajo, idealmente cuatro o cinco que capturan las necesidades de la mayoría de los usuarios del sistema.

* Asigne al menos dos usuarios al nivel de acceso de administrador global del sistema.

* Restrinja lo que los usuarios pueden hacer con los elementos de Workfront compartiendo en lugar de eliminar una capacidad en un nivel de acceso.

</br>
</br>


## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Comience con menos acceso para los usuarios al configurar los niveles de acceso.



**He aquí la razón**

Inicie los usuarios con el acceso mínimo que necesitarán para realizar su trabajo. Si no pueden realizar su trabajo debido a derechos de acceso insuficientes, normalmente solicitarán acceso adicional. Conceder a los usuarios demasiado acceso de inmediato podría provocar problemas de seguridad. Además, siempre es mejor dar a los usuarios más acceso que quitarles el acceso.

</br>
</br>



**Práctica recomendada**

Al asignar licencias de revisión y solicitud, el valor predeterminado suele ser Revisar porque proporciona al usuario más permisos en Adobe Workfront.



**He aquí la razón**

Aunque las licencias de revisión y solicitud se pueden asignar a un número ilimitado de usuarios en Workfront, las licencias de solicitud se limitan prácticamente a realizar y actualizar solicitudes. Una licencia de revisión tiene más acceso a proyectos y tareas que una licencia de solicitud, así como la posibilidad de ver portafolios y programas, editar documentos y acceder a herramientas de administración de recursos.

</br>
</br>

**Práctica recomendada**

Desmarque la casilla &quot;Compartir en todo el sistema&quot; en cada objeto en todos sus niveles de acceso, a menos que haya una razón específica por la que los usuarios deban poder compartir en todo el sistema.



**He aquí la razón**

Compartir un objeto en todo el sistema se utiliza a menudo como una muleta para permitir que ciertos usuarios vean elementos en Workfront. Esto sucede cuando falta la estructura de grupo de Workfront o cuando los permisos de uso compartido no se comprenden completamente. Cuando los elementos se comparten en todo el sistema, significa que todos pueden ver el elemento compartido. Según el tipo de información que se mantenga en el sistema, esto podría provocar problemas de privacidad.



Por ejemplo: puede estar trabajando con varios proveedores dentro de Workfront para comprobar el progreso, proporcionar aprobaciones, etc. Si la casilla &quot;Compartir en todo el sistema&quot; es una opción, se puede seleccionar o establecer como predeterminada, haciendo que la información esté disponible para todos los proveedores.



Al desmarcar la opción por completo, hace que un usuario, con permiso para compartir, deba determinar la persona o personas específicas (ya sea a través de una compañía, un grupo o un equipo) con las que desee compartir el objeto.

</br>
</br>

**Práctica recomendada**

Considere la posibilidad de activar la opción &quot;Nunca permitir que los usuarios eliminen comentarios&quot; en Establecer restricciones adicionales en un nivel de acceso.



**He aquí la razón**

La activación de esta opción garantiza que las comunicaciones anteriores no se eliminen de Workfront. Algunas organizaciones requieren que se conserve el historial completo de comentarios para fines de auditoría.

</br>
</br>

**Práctica recomendada**

Limite el número de administradores del sistema en favor de los administradores del grupo.



**He aquí la razón**

Los administradores del sistema tienen acceso a todo lo que hay en Workfront, incluida la configuración global del sistema. El administrador del sistema controla las opciones de configuración a las que pueden acceder los administradores del grupo y se aplican únicamente a ese grupo específico.



Tener administradores de grupo permite a los administradores de sistemas delegar muchas responsabilidades, lo que les permite centrarse en elementos de mayor alcance, en lugar del mantenimiento diario de Workfront. Los administradores de grupos pueden mantenerse en contacto con mayor facilidad con las necesidades de sus grupos, lo que proporciona un mejor servicio para los usuarios.

</br>
</br>


**Práctica recomendada**

Copie un nivel de acceso existente y realice modificaciones, en lugar de crear un nuevo nivel de acceso desde cero.



**He aquí la razón**

Copiar un nivel de acceso existente proporciona una base coherente para nuevos niveles de acceso, lo que garantiza que la configuración inicial sea idéntica. Esto también ahorra tiempo, ya que los administradores del sistema no tienen que configurar un nivel de acceso completamente desde cero.

</br>
</br>

**Práctica recomendada**

Documente lo que cada nivel de acceso puede hacer en el cuadro Descripción.



**He aquí la razón**

Obtenga información detallada con la descripción, donde se enumeran los ajustes de cada tipo de objeto. Esto ayuda a los administradores de sistemas (presentes y futuros) a saber exactamente qué hace cada nivel de acceso sin tener que sumergirse en el propio nivel de acceso para revisar la configuración.



Esto también puede facilitar la comparación de los niveles de acceso al verlos en un informe. El campo de descripción se puede añadir rápidamente a la vista para ver rápidamente cómo difieren y, posiblemente, por qué se creó un nivel de acceso diferente.

</br>
</br>

**Práctica recomendada**

Limítese únicamente a los niveles de acceso necesarios para lograr sus objetivos de trabajo, idealmente cuatro o cinco que capturan las necesidades de la mayoría de los usuarios del sistema.


**He aquí la razón**

El nivel de acceso garantiza que, cuando se comparta un objeto de Workfront con un usuario, este tenga los derechos necesarios para editarlo, eliminarlo, etc. Puede hacer que los niveles de acceso sean más generales, ya que el uso compartido de elementos individuales se puede configurar para que sean más específicos.


Además, tener menos niveles de acceso puede facilitar el mantenimiento de un sistema sin desorden e implementar una estrategia, lo que también puede llevar a una incorporación más rápida cuando las personas se unen a la compañía o cambian de departamento.

</br>
</br>

**Práctica recomendada**

Asigne al menos dos usuarios al nivel de acceso de administrador global del sistema.

**He aquí la razón**

Más de una persona debe comprender por qué Workfront se configuró de la forma en que estaba, cómo administrarlo/mantenerlo y cómo admitir usuarios. Si una persona está fuera de la oficina, abandona la organización, está ocupada, etc., esto garantiza que haya otra persona que tenga la información y los conocimientos necesarios para administrar correctamente el sistema.

</br>
</br>

**Práctica recomendada**

Restrinja lo que los usuarios pueden hacer con los elementos de Workfront compartiendo en lugar de eliminar una capacidad en un nivel de acceso.


**He aquí la razón**

Los niveles de acceso controlan lo que los usuarios pueden hacer con elementos específicos en un nivel global. Los permisos de uso compartido de cada proyecto, tarea, portafolio, documento, etc. controlan lo que un usuario individual puede hacer con ese elemento específico. En lugar de eliminar una capacidad para todas las personas con un nivel de acceso específico, ajuste los permisos de uso compartido en elementos específicos para que los usuarios tengan controles limitados.
