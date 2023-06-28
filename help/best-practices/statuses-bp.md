---
title: 'Práctica recomendada: estados'
description: Explore las recomendaciones sobre prácticas recomendadas de los expertos de Adobe Workfront acerca de la configuración, administración y uso de los estados de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Práctica recomendada: estados

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de estados

* Al cambiar el nombre de los estados predeterminados de Workfront, mantenga el mismo propósito original del estado.

* Si crea un estado de proyecto personalizado para Cancelado, equipare el estado con Inactivo.

* Mantenga los estados personalizados globales al mínimo.

* No utilice estados de proyecto en lugar de tareas para indicar la progresión de un proyecto.


</br>
</br>



## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Al cambiar el nombre de los estados predeterminados de Workfront, mantenga el mismo propósito original del estado.



**He aquí la razón**

Algunas acciones en Workfront se activan por los estados predeterminados del sistema. Cambiar la intención de un estado puede afectar al comportamiento de Workfront en determinadas situaciones, a la creación de informes, etc.



Por ejemplo, el estado de tarea predeterminado Completar indica a Workfront que cambie el porcentaje completado de una tarea a 100%. El estado Completo también permite a Workfront saber que se puede empezar a trabajar en tareas dependientes. Si ha cambiado el nombre del estado a En espera, para indicar que un trabajo en una tarea está en pausa, Workfront va a pensar que la tarea ha finalizado y pondrá en marcha los pasos siguientes del proyecto.

</br>
</br>



**Práctica recomendada**

Si crea un estado de proyecto personalizado para Cancelado, equipare el estado con Inactivo.



**He aquí la razón**

Si iguala Cancelado con Completado, no puede utilizar el estado para cancelar un proyecto a menos que todas las tareas se marquen como completadas y todos los problemas estén cerrados. Pero si se equipara Cancelado con Muerto, se puede cancelar el proyecto sin cambiar nada en el registro histórico.


</br>
</br>

**Práctica recomendada**

Mantenga los estados personalizados globales al mínimo.



**He aquí la razón**

Menos es más. Además de crear mantenimiento innecesario, demasiados estados personalizados crean confusión, especialmente cuando se trabaja en proyectos interfuncionales. En su lugar, haga que los estados personalizados sean específicos del grupo. Esto mantiene su entorno de Workfront más limpio y mejor posicionado para la expansión a otros grupos en el futuro. Trabaje con el comité de gobernanza/supervisión y las partes interesadas para identificar los estados que deben utilizar los grupos de su organización.


</br>
</br>

**Práctica recomendada**

No utilice estados de proyecto en lugar de tareas para indicar la progresión de un proyecto.



**He aquí la razón**

Mantenga los estados de proyecto simples para indicar fases de progreso de alto nivel, como Planificación, Actual, Completada, etc. Permita que las tareas, los estados de las tareas y el porcentaje completado de la tarea le indiquen el progreso general del trabajo en el proyecto. Estos indicadores de nivel de tarea se acumulan en el porcentaje completado del proyecto, la condición del proyecto y el estado del progreso del proyecto, todos los cuales son mejores indicadores y más precisos de la progresión del proyecto que un estado del proyecto. Además, esta información de nivel de tarea proporciona mejores informes de proyecto.
