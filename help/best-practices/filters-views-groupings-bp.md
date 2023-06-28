---
title: 'Práctica recomendada: Filtros, vistas y agrupaciones'
description: Explore las recomendaciones sobre prácticas recomendadas de los expertos de Adobe Workfront acerca de la configuración, administración y uso de filtros, vistas y agrupaciones de Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Práctica recomendada: Filtros, vistas y agrupaciones

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de filtros, vistas y agrupaciones

* Reduzca el número de informes personalizados que crea aprovechando los filtros, las vistas y las agrupaciones de una lista de objetos para obtener los datos que necesita.

* Utilice los controles de lista de las plantillas de diseño para ocultar los filtros, las vistas y las agrupaciones innecesarios para los objetos de uso común (proyectos, tareas, programas, etc.).

* Comparta filtros, vistas y agrupaciones personalizadas relevantes para los flujos de trabajo y procesos de su organización a través de los controles de lista en las plantillas de diseño.

* Al crear filtros para el estado del proyecto, el estado de la tarea o el estado del problema, utilice el nombre de campo (objeto)>>Estado es igual al origen/campo con el modificador Igual, en lugar de con el nombre de campo/origen del campo Proyecto>>Estado.

</br>
</br>

## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Reduzca el número de informes personalizados que crea aprovechando los filtros, las vistas y las agrupaciones de una lista de objetos para obtener los datos que necesita.

**He aquí la razón**

La creación de informes de un solo uso para cada segmento de datos que desee ver es una tarea laboriosa que agota el sistema de Workfront.

</br>
</br>

**Práctica recomendada**

Utilice los controles de lista de las plantillas de diseño para ocultar los filtros, las vistas y las agrupaciones innecesarios para los objetos de uso común (proyectos, tareas, programas, etc.).

**He aquí la razón**

Menos es más. Al ocultar las opciones de filtro, vista y agrupación de listas que no son relevantes para los flujos de trabajo diarios de los usuarios, se reducen las listas, lo que facilita a los usuarios encontrar lo que necesitan más rápido.

</br>
</br>

**Práctica recomendada**

Comparta filtros, vistas y agrupaciones personalizadas relevantes para los flujos de trabajo y procesos de su organización a través de los controles de lista en las plantillas de diseño.

**He aquí la razón**

Si ha creado filtros, vistas y agrupaciones que muestran información específica de los procesos diarios de los usuarios, es fácil compartirlas a través de las plantillas de diseño. Esto garantiza que todos los usuarios asignados a esa plantilla de diseño tengan opciones de filtro, vista y agrupación relevantes para sus flujos de trabajo.

La personalización de la información que desea que sea visible para los usuarios a través de las plantillas de diseño también ahorra tiempo a los administradores de sistemas y grupos, ya que no tendrán que compartir cada opción de filtro, vista o agrupación de forma individual.

</br>
</br>

**Práctica recomendada**

Al crear filtros para el estado del proyecto, el estado de la tarea o el estado del problema, utilice el nombre de campo (objeto)>>Estado es igual al origen/campo con el modificador Igual, en lugar de con el nombre de campo/origen del campo Proyecto>>Estado.

**He aquí la razón**

Al utilizar (objeto)>>Igual que, se incluyen todos los estados personalizados que tienen ese estado específico asignado en el campo Igual que con en las configuraciones de estado. Mientras que la configuración del filtro como (objeto)>>Estado > Igual requiere que seleccione estados específicos para el filtro. Esto podría suponer un desafío de mantenimiento si necesita tener en cuenta estos nuevos estados en varios filtros. Cada filtro tendría que abrirse y actualizarse con el nuevo estado.

Por ejemplo, si desea ver todos los proyectos actuales, puede configurar el filtro para que lea Proyecto > Estado > Igual > Actual. Sin embargo, si alguien agrega un estado personalizado denominado Activo y lo equipara a Actual, ese filtro no encontrará proyectos con el estado Activo. Sin embargo, si utiliza el proyecto > Estado es igual a > Igual a > Actual, el filtro encuentra objetos con el estado Actual o Activo porque ambos tienen Actual en el campo Igual a.
