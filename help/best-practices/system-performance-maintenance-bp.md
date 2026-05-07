---
title: 'Práctica recomendada: rendimiento y mantenimiento del sistema'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre el rendimiento y el mantenimiento del sistema de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10927
exl-id: c3f32975-96f4-4e62-8c3a-5b985b45bbbf
TQID: https://experienceleague.adobe.com/2tq7aNHE96fep1EFCPrjcCo13t5lQ24A6c-ORDUmlpY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 638
ht-degree: 93%

---

# Práctica recomendada: rendimiento y mantenimiento del sistema

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El área &quot;¿Por qué son estas prácticas recomendadas?&quot;, que se encuentra después de la lista de alto nivel, proporciona más detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de rendimiento y mantenimiento del sistema

* Revise las notas de la versión del producto antes de la fecha de lanzamiento.

* Cree diferentes tipos de informes de excepciones que resalten datos y configuraciones que faltan o son incorrectas.

* Cree un proceso de desactivación del usuario que incluya una revisión de los objetos que son de su propiedad o que se le asignan para que los usuarios que ya no forman parte de la empresa no permanezcan activos en el sistema y creen confusión para otros usuarios.

* Mantenga las configuraciones de flujo de trabajo tan sencillas como sea posible para asegurarse de que son escalables y se puedan mantener en su ausencia.

* Utilice filtros en informes y listas de objetos para reducir el número de filas que se muestran al mismo tiempo y centre el equipo en información importante.

* Borre con regularidad la caché del explorador y las cookies para mejorar el rendimiento en Workfront.

* Empiece a limpiar el sistema en las principales áreas de Adobe Workfront que suelen estar más saturadas, como formularios personalizados, plantillas, proyectos y usuarios.

* Sepa en qué clúster se encuentra su instancia de Workfront para que pueda ver las actualizaciones, las ventanas de mantenimiento, etc.

* Mantenga los proyectos cortos.

* Siempre que sea posible, mantenga los informes “livianos” con pocos filtros sencillos para mejorar el rendimiento.

</br>
</br>

## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Revise las notas de la versión del producto antes de la fecha de lanzamiento.



**A continuación se explica por qué**

Las notas de la versión indican la nueva funcionalidad y herramientas que se proporcionan en el sistema Workfront. Si revisa estas notas y experimenta con las nuevas funcionalidades del entorno de vista previa de la zona protegida, tiene la oportunidad de aprender, practicar y resolver cualquier error con las nuevas mejoras antes de su lanzamiento a producción.

</br>
</br>

**Práctica recomendada**

Cree diferentes tipos de informes de excepciones que resalten datos y configuraciones que faltan o son incorrectas.



**A continuación se explica por qué**

Estos informes incluyen los que indican qué usuarios deben desactivarse, qué proyectos muestran un porcentaje de finalización del 100 %, pero no se marcan como completados, qué plantillas nunca se han utilizado, etc.



Coloque informes como estos y otros en un tablero y proporcione acceso a otros administradores de sistemas y grupos para mantener un sistema limpio de manera oportuna. Por ejemplo, el panel de control de limpieza de Workfront y el panel de control de uso de Workfront incluyen ejemplos de informes que puede crear.



Para ayudarle a recordar estos informes, al menos trimestralmente, cree un proyecto con tareas trimestrales y asígnelas a usted mismo, y a los administradores de sistemas y grupos. Asegúrese de que estas tareas tengan asociadas horas planificadas para que los usuarios asignados a estos elementos de trabajo puedan distribuir adecuadamente su tiempo.

</br>
</br>

**Práctica recomendada**

Mantenga los proyectos cortos.



**A continuación se explica por qué**

Cada vez que guarda un proyecto o una tarea dentro del proyecto, se ejecuta un cálculo de una cronología para actualizar todas las dependencias. En función del número de tareas del proyecto, el cálculo puede tardar mucho tiempo en ejecutarse.
