---
title: 'Práctica recomendada: licencias y niveles de acceso'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de licencias y niveles de acceso de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '1253'
ht-degree: 100%

---

# Práctica recomendada: licencias y niveles de acceso

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El punto &quot;¿Por qué estas son prácticas recomendadas?&quot; se encuentra después de la lista de alto nivel, proporciona mayores detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., cuya implementación se debe considerar al trabajar con Workfront.

</br>
</br>

## Prácticas recomendadas sobre licencias y niveles de acceso

* Comience con menos acceso para los usuarios al configurar los niveles de acceso.

* Al asignar licencias de revisión y solicitud, normalmente se usa de forma predeterminada Revisar porque proporciona al usuario más permisos en Adobe Workfront.

* Desmarque la casilla “Compartir todo el sistema” de cada objeto en todos los niveles de acceso a menos que desee que esos usuarios puedan hacerlo específicamente.

* Considere la posibilidad de activar el ajuste “No permitir que los usuarios eliminen comentarios” en Establecer restricciones adicionales en un nivel de acceso.

* Limite el número de administradores del sistema en favor de los administradores del grupo.

* Copie un nivel de acceso existente y realice modificaciones, en lugar de crear un nuevo nivel de acceso desde cero.

* Documente lo que puede hacer cada nivel de acceso en el cuadro Descripción.

* Limitarse a los niveles de acceso necesarios para lograr sus objetivos de trabajo, idealmente cuatro o cinco que captan las necesidades de la mayoría de los usuarios del sistema.

* Asigne al menos dos usuarios al nivel de acceso del administrador global del sistema.

* Restringir lo que los usuarios pueden hacer con los elementos de Workfront mediante el uso compartido, en lugar de eliminar una funcionalidad en un nivel de acceso.

</br>
</br>


## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Comience con menos acceso para los usuarios al configurar los niveles de acceso.



**A continuación se explica por qué**

Inicie a los usuarios en el acceso mínimo que necesitarán para realizar su trabajo. Si no pueden realizar su trabajo debido a derechos de acceso insuficientes, generalmente deberán solicitar un acceso adicional. Conceder a los usuarios demasiado acceso de inmediato podría provocar problemas de seguridad. Además, siempre es mejor dar a los usuarios más acceso que quitarlo.

</br>
</br>



**Práctica recomendada**

Al asignar licencias de revisión y solicitud, normalmente se usa de forma predeterminada Revisar porque proporciona al usuario más permisos en Adobe Workfront.



**A continuación se explica por qué**

Aunque las licencias de Revisión y Solicitud se pueden asignar a un número ilimitado de usuarios en Workfront, las licencias de solicitud se limitan a realizar y actualizar solicitudes. Una licencia de Revisión tiene más acceso a proyectos y tareas que una licencia de Solicitud, así como la posibilidad de ver carteras y programas, editar documentos y acceder a herramientas de administración de recursos.

</br>
</br>

**Práctica recomendada**

Desmarque la casilla “Compartir todo el sistema” de cada objeto en todos los niveles de acceso, a menos que exista una razón específica por la que los usuarios deban poder compartir en todo el sistema.



**A continuación se explica por qué**

El uso compartido de un objeto en todo el sistema se utiliza a menudo como una herramienta para permitir a ciertos usuarios ver elementos en Workfront. Esto sucede cuando falta la estructura del grupo de Workfront o cuando los permisos de uso compartido no se comprenden completamente. Cuando los elementos se comparten en todo el sistema, significa que todos pueden ver el elemento que se comparte. Dependiendo del tipo de información que se mantenga en el sistema, esto podría llevar a problemas de privacidad.



Por ejemplo, es posible que esté trabajando con varios proveedores dentro de Workfront para comprobar el progreso, proporcionar aprobaciones, etc. Si la casilla de verificación “Compartir todo el sistema” es una opción, podría seleccionarse o establecerse como predeterminada, poniendo la información a disposición de todos los proveedores.



Al desmarcar la opción por completo, habilita que un usuario, con el permiso para compartir, deba determinar la persona o personas específicas (a través de una compañía, grupo o equipo) con las que desee compartir el objeto.

</br>
</br>

**Práctica recomendada**

Considere la posibilidad de activar el ajuste “No permitir que los usuarios eliminen comentarios” en Establecer restricciones adicionales en un nivel de acceso.



**A continuación se explica por qué**

Activar esta opción garantiza que las comunicaciones anteriores no se eliminen de Workfront. Algunas organizaciones necesitan que se mantenga el historial completo de comentarios para fines de auditoría.

</br>
</br>

**Práctica recomendada**

Limite el número de administradores del sistema en favor de los administradores del grupo.



**A continuación se explica por qué**

Los administradores del sistema tienen acceso a todo lo que hay en Workfront, incluida la configuración global del sistema. La configuración a la que pueden acceder los administradores de grupos está controlada por el administrador del sistema y solo se aplica a ese grupo específico.



Tener administradores de grupos permite que los administradores del sistema deleguen muchas responsabilidades, lo que les permite centrarse en asuntos más importantes, en lugar del mantenimiento diario de Workfront. Los administradores de grupos pueden mantenerse más fácilmente en contacto con las necesidades de sus miembros, lo que proporciona un mejor servicio a los usuarios.

</br>
</br>


**Práctica recomendada**

Copie un nivel de acceso existente y realice modificaciones, en lugar de crear un nuevo nivel de acceso desde cero.



**A continuación se explica por qué**

Copiar un nivel de acceso existente proporciona una base coherente para nuevos niveles de acceso, lo que garantiza que la configuración inicial sea idéntica. Con esto también se ahorra tiempo, ya que los administradores del sistema no tendrán que configurar un nivel de acceso desde cero.

</br>
</br>

**Práctica recomendada**

Documente lo que puede hacer cada nivel de acceso en el cuadro Descripción.



**A continuación se explica por qué**

Tenga en cuenta la descripción e indique cuáles son los ajustes de cada tipo de objeto. Esto ayuda a los administradores del sistema (presentes y futuros) a saber exactamente qué hace cada nivel de acceso sin tener que sumergirse en el nivel de acceso mismo para revisar la configuración.



Esto también puede facilitar la comparación de los niveles de acceso al consultarlos en un informe. El campo de descripción se puede agregar rápidamente a la vista para ver cómo difieren y, posiblemente, por qué se creó un nivel de acceso diferente.

</br>
</br>

**Práctica recomendada**

Limitarse a los niveles de acceso necesarios para lograr sus objetivos de trabajo, idealmente cuatro o cinco que captan las necesidades de la mayoría de los usuarios del sistema.


**A continuación se explica por qué**

El nivel de acceso garantiza que, cuando un objeto de Workfront se comparte con un usuario, este tenga los derechos necesarios para editarlo, eliminarlo, etc. Los niveles de acceso se pueden hacer más generales porque el uso compartido en elementos individuales se puede configurar para que sean más específicos.


Además, tener menos niveles de acceso puede facilitar el mantenimiento de un sistema sin desorden e implementar una estrategia, lo que también puede llevar a una incorporación más rápida cuando las personas se unen a la empresa o cambian de departamento.

</br>
</br>

**Práctica recomendada**

Asigne al menos dos usuarios al nivel de acceso del administrador global del sistema.

**A continuación se explica por qué**

Más de una persona debe comprender por qué Workfront se configuró del modo en que estaba, cómo administrarlo/mantenerlo y cómo apoyar a los usuarios. Si una persona está fuera de la oficina, abandona la organización, está ocupada, etc., esto garantiza que haya otra persona que tenga la información y el conocimiento para administrar con éxito el sistema.

</br>
</br>

**Práctica recomendada**

Restringir lo que los usuarios pueden hacer con los elementos de Workfront mediante el uso compartido, en lugar de eliminar una funcionalidad en un nivel de acceso.


**A continuación se explica por qué**

Los niveles de acceso controlan lo que los usuarios pueden hacer con elementos específicos a nivel global. Los permisos de uso compartido de cada proyecto, tarea, portafolio, documento, etc. controlan lo que un usuario puede hacer con ese elemento específico. En lugar de eliminar una capacidad para todos los usuarios con un nivel de acceso específico, ajuste los permisos de uso compartido en elementos específicos para que los usuarios tengan controles limitados.
