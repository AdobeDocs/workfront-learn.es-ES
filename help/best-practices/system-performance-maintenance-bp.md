---
title: 'Práctica recomendada: rendimiento y mantenimiento del sistema'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre el rendimiento y el mantenimiento del sistema de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Práctica recomendada: rendimiento y mantenimiento del sistema

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las mejores prácticas son directrices que representan un curso de acción eficaz y eficiente; sean adoptados fácilmente por usted y los usuarios de su empresa; y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, tenga en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco para ayudarle a guiar la configuración y el uso del sistema Workfront.

## Navegar por esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

La pregunta &quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de rendimiento y mantenimiento del sistema

* Revise las notas de la versión del producto antes de la fecha de lanzamiento.

* Cree diferentes tipos de informes de excepciones que resalten datos y configuraciones que faltan o son incorrectas.

* Cree un proceso de desactivación de usuario que incluya una revisión de los objetos que son propiedad de ellos o que se les asigna para que los usuarios que ya no forman parte de la empresa no permanezcan activos en el sistema y creen confusión para otros usuarios.

* Mantenga las configuraciones de flujo de trabajo tan sencillas como sea posible para asegurarse de que son escalables y se pueden mantener en su ausencia.

* Utilice filtros en informes y listas de objetos para reducir el número de filas que se muestran al mismo tiempo y centre el equipo en información importante.

* Borre con regularidad la caché del explorador y las cookies para ayudar a mejorar el rendimiento en Workfront.

* Empiece a limpiar el sistema en las principales áreas de Adobe Workfront que suelen estar más saturadas, como formularios personalizados, plantillas, proyectos y usuarios.

* Sepa en qué clúster se encuentra su instancia de Workfront para que pueda ver las actualizaciones, las ventanas de mantenimiento, etc.

* Mantenga los proyectos cortos.

* Siempre que sea posible, mantenga los informes &quot;livianos&quot; con filtros muy pocos y sencillos para mejorar el rendimiento.

</br>
</br>

## ¿Por qué estas prácticas recomendadas?

**Práctica recomendada**

Revise las notas de la versión del producto antes de la fecha de lanzamiento.



**He aquí por qué**

Las notas de la versión indican las nuevas funciones y herramientas que se proporcionan en el sistema Workfront. Al revisar estas notas y jugar con la nueva funcionalidad del entorno de vista previa de espacio aislado, tiene la oportunidad de aprender, practicar y resolver cualquier error con las nuevas mejoras antes de su lanzamiento a producción.

</br>
</br>

**Práctica recomendada**

Cree diferentes tipos de informes de excepciones que resalten datos y configuraciones que faltan o son incorrectas.



**He aquí por qué**

Estos informes incluyen informes que indican qué usuarios deben desactivarse, qué proyectos muestran un porcentaje de finalización del 100 % pero no se marcan como completados, qué plantillas nunca se han utilizado, etc.



Coloque estos informes como estos y otros en un tablero y proporcione a otros administradores de sistemas y grupos acceso a este tablero para mantener un sistema limpio de manera oportuna. Por ejemplo, el panel de limpieza de Workfront y el panel de uso de Workfront incluyen ejemplos de informes que puede crear.



Para recordar comprobar estos informes, al menos trimestralmente, cree un proyecto con tareas trimestrales y asígnelas a usted mismo, y a los administradores de sistemas y grupos. Asegúrese de que estas tareas tengan asociadas horas planificadas para que los usuarios asignados de estos elementos de trabajo puedan asignar correctamente su tiempo.

</br>
</br>

**Práctica recomendada**

Mantenga los proyectos cortos.



**He aquí por qué**

Cada vez que guarda un proyecto o una tarea dentro del proyecto, se ejecuta un cálculo de línea de tiempo para actualizar todas las dependencias. En función del número de tareas del proyecto, el cálculo puede tardar mucho tiempo en ejecutarse.
