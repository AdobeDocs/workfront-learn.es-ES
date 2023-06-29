---
title: 'Práctica recomendada: filtros, vistas y agrupamientos'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront acerca de la configuración, administración y uso de filtros, vistas y agrupaciones de Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '700'
ht-degree: 100%

---

# Práctica recomendada: filtros, vistas y agrupamientos

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El punto &quot;¿Por qué estas son prácticas recomendadas?&quot; se encuentra después de la lista de alto nivel, proporciona mayores detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., cuya implementación se debe considerar al trabajar con Workfront.

</br>
</br>

## Prácticas recomendadas de filtros, vistas y agrupaciones

* Para obtener los datos que necesita, reduzca el número de informes personalizados que crea mediante filtros, vistas y agrupaciones en una lista de objetos.

* Utilice los controles de lista en las plantillas de diseño para ocultar los filtros, vistas y agrupaciones innecesarios para los objetos que use con más frecuencia (proyectos, tareas, programas, etc.).

* Comparta filtros personalizados, vistas y agrupaciones relevantes para los flujos de trabajo y procesos de su organización a través de los controles de lista de las plantillas de diseño.

* Al crear filtros para el estado del proyecto, de la tarea o del problema, emplee el origen/nombre de campo (objeto)>>Estado equivale a con el modificador Igual, en lugar de Proyecto>>Estado.

</br>
</br>

## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Para obtener los datos que necesita, reduzca el número de informes personalizados que crea mediante filtros, vistas y agrupaciones en una lista de objetos.

**A continuación se explica por qué**

La creación de informes de un solo uso para cada segmento de datos que desee ver es un proceso laborioso y satura el sistema de Workfront.

</br>
</br>

**Práctica recomendada**

Utilice los controles de lista en las plantillas de diseño para ocultar los filtros, vistas y agrupaciones innecesarios para los objetos que use con más frecuencia (proyectos, tareas, programas, etc.).

**A continuación se explica por qué**

Menos es más. Ocultar las opciones de filtro, vista y lista de agrupaciones que no son relevantes para los flujos de trabajo diarios de los usuarios reduce las listas, lo que facilita a los usuarios encontrar lo que necesitan más rápido.

</br>
</br>

**Práctica recomendada**

Comparta filtros personalizados, vistas y agrupaciones relevantes para los flujos de trabajo y procesos de su organización a través de los controles de lista de las plantillas de diseño.

**A continuación se explica por qué**

Si ha creado filtros, vistas y agrupaciones que muestran información específica de los procesos diarios de los usuarios, es fácil compartirlos mediante las plantillas de diseño. Esto garantiza que todos los usuarios asignados a esa plantilla de diseño tengan opciones de filtro, vista y agrupación relevantes para sus flujos de trabajo.

La personalización de la información que desea que sea visible para los usuarios a través de las plantillas de diseño también permite ahorrar tiempo para los administradores de sistemas y grupos, ya que no tienen que compartir cada opción de filtro, vista o agrupación individualmente.

</br>
</br>

**Práctica recomendada**

Al crear filtros para el estado del proyecto, de la tarea o del problema, emplee el origen/nombre de campo (objeto)>>Estado equivale a con el modificador Igual, en lugar de Proyecto>>Estado.

**A continuación se explica por qué**

Al utilizar (objeto)>>Equivale a, se incluyen todos los estados personalizados que tienen ese estado específico asignado en el campo Equivale a en la configuración de estado. Mientras que la configuración del filtro como (objeto)>>Estado > Igual requiere que seleccione estados específicos para el filtro. Esto podría suponer un desafío de mantenimiento si necesita tener en cuenta estos nuevos estados en varios filtros. Cada filtro tendría que abrirse y actualizarse con el nuevo estado.

Por ejemplo, si desea ver todos los proyectos actuales, puede configurar el filtro para que lea Proyecto>>Estado > Igual > Actual. Pero si alguien agrega un estado personalizado llamado Activo y lo equipara a Actual, ese filtro no encontrará proyectos con el estado Activo. Sin embargo, si utiliza Proyecto>>Estado equivale a > Igual > Actual, el filtro encuentra objetos con el estado Actual o Activo porque ambos tienen Actual en el campo Equivale a.
