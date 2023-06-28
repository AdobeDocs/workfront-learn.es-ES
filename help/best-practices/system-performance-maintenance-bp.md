---
title: 'Práctica recomendada: rendimiento y mantenimiento del sistema'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront acerca del rendimiento y mantenimiento del sistema de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Práctica recomendada: rendimiento y mantenimiento del sistema

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de rendimiento y mantenimiento del sistema

* Revise las notas de la versión del producto antes de la fecha de lanzamiento.

* Cree diferentes tipos de informes de excepciones que resalten los datos y la configuración que faltan o son incorrectos.

* Cree un proceso de desactivación de usuarios que incluya una revisión de los objetos que son propiedad de ellos o que se les han asignado para que los usuarios que ya no forman parte de la compañía no permanezcan activos en el sistema y creen confusión para otros usuarios.

* Mantenga las configuraciones de flujo de trabajo tan sencillas como sea posible para asegurarse de que son escalables y se pueden mantener en su ausencia.

* Utilice filtros en informes y listas de objetos para reducir el número de filas mostradas a la vez y enfocar el equipo en información importante.

* Borre regularmente la caché del explorador y las cookies para ayudar a mejorar el rendimiento en Workfront.

* Limpie el sistema en las principales áreas de Adobe Workfront que suelen estar más saturadas, como formularios personalizados, plantillas, proyectos y usuarios.

* Sepa en qué clúster se encuentra la instancia de Workfront para poder ver las actualizaciones, tener en cuenta los períodos de mantenimiento, etc.

* Utilice proyectos cortos.

* Cuando sea posible, mantenga los informes &quot;ligeros&quot; con muy pocos filtros y sin complicaciones para mejorar el rendimiento.

</br>
</br>

## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Revise las notas de la versión del producto antes de la fecha de lanzamiento.



**He aquí la razón**

Las notas de la versión le indican las nuevas funciones y herramientas que llegan al sistema de Workfront. Al revisar estas notas y jugar con la nueva funcionalidad en el entorno de vista previa de espacio aislado, tiene la oportunidad de conocer, practicar y resolver cualquier error con nuevas mejoras antes de que se publique en producción.

</br>
</br>

**Práctica recomendada**

Cree diferentes tipos de informes de excepciones que resalten los datos y la configuración que faltan o son incorrectos.



**He aquí la razón**

Estos informes incluyen los que indican qué usuarios deben desactivarse, qué proyectos muestran un porcentaje de finalización del 100 % pero no se marcan como completados, qué plantillas nunca se han utilizado, etc.



Coloque estos informes, como estos y otros, en un panel y proporcione a otros administradores de sistemas y grupos acceso a este panel para mantener un sistema limpio de manera oportuna. Por ejemplo, el Tablero de limpieza de Workfront y el Tablero de uso de Workfront incluyen ejemplos de informes que puede crear.



Para ayudarle a recordar que debe comprobar estos informes, al menos trimestralmente, cree un proyecto con tareas trimestrales y asígnelas a usted mismo y a los administradores de sistemas y grupos. Asegúrese de que estas tareas tengan horas planificadas asociadas para que las personas asignadas a estos elementos de trabajo puedan asignar correctamente su tiempo.

</br>
</br>

**Práctica recomendada**

Utilice proyectos cortos.



**He aquí la razón**

Cada vez que se guarda un proyecto o una tarea dentro del proyecto, se ejecuta un cálculo de escala de tiempo para actualizar todas las dependencias. En función del número de tareas del proyecto, la actualización puede tardar mucho tiempo en ejecutarse.
