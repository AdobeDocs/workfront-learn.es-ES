---
title: 'Práctica recomendada: estados'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de los estados de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 100%

---

# Práctica recomendada: estados

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El punto &quot;¿Por qué estas son prácticas recomendadas?&quot; se encuentra después de la lista de alto nivel, proporciona mayores detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., cuya implementación se debe considerar al trabajar con Workfront.

</br>
</br>

## Prácticas recomendadas sobre los estados

* Al cambiar el nombre de los estados predeterminados de Workfront, mantenga el propósito original del estado igual.

* Si crea un estado de proyecto personalizado para Cancelado, equipare el estado con Inactivo.

* Mantenga los estados personalizados globales al mínimo.

* No utilice estados de proyecto en lugar de tareas para indicar la progresión de un proyecto.


</br>
</br>



## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Al cambiar el nombre de los estados predeterminados de Workfront, mantenga el propósito original del estado igual.



**A continuación se explica por qué**

Algunas acciones de Workfront se activan mediante los estados predeterminados del sistema. Cambiar la intención de un estado puede afectar al comportamiento de Workfront en determinadas situaciones, afectar a los informes, etc.



Por ejemplo, el estado de tarea predeterminado de Completado indica a Workfront que cambie el porcentaje completado de una tarea al 100 %. El estado Completado también permite a Workfront saber que se puede iniciar el trabajo en tareas dependientes. Si ha cambiado el nombre del estado a Esperando, para indicar que un trabajo en una tarea está en pausa, Workfront va a pensar que la tarea ha finalizado y dar los pasos siguientes en el proyecto.

</br>
</br>



**Práctica recomendada**

Si crea un estado de proyecto personalizado para Cancelado, equipare el estado con Inactivo.



**A continuación se explica por qué**

Si se equipara Cancelado con Completado, no se puede utilizar el estado para cancelar un proyecto a menos que todas las tareas estén marcadas como completadas y que se hayan cerrado todos los problemas. Pero si se equipara Cancelado con Inactivo, se puede cancelar el proyecto sin cambiar nada en el registro histórico.


</br>
</br>

**Práctica recomendada**

Mantenga los estados personalizados globales al mínimo.



**A continuación se explica por qué**

Menos es más. Además de crear mantenimiento innecesario, demasiados estados personalizados crean confusión, especialmente al trabajar en proyectos interfuncionales. En su lugar, haga que los estados personalizados sean específicos del grupo. Esto mantiene el entorno de Workfront más limpio y mejor posicionado para la expansión a otros grupos en el futuro. Trabaje con su comité de gobernanza/supervisión y con las partes interesadas para identificar los estados que deben utilizar los grupos de su organización.


</br>
</br>

**Práctica recomendada**

No utilice estados de proyecto en lugar de tareas para indicar la progresión de un proyecto.



**A continuación se explica por qué**

Mantenga los estados del proyecto simples para indicar fases de progresión de alto nivel, como Planificación, Actual, Completado, etc. Permita que las tareas, los estados de las tareas y el porcentaje completado de la tarea le digan cómo progresa el trabajo en general en el proyecto. Estos indicadores de nivel de tarea se resumen en el porcentaje completado del proyecto, la condición y el estado de progreso del proyecto, todos los cuales son mejores indicadores y más precisos de la progresión del proyecto que un estado del proyecto. Además, esta información de nivel de tarea proporciona una mejor creación de informes de proyecto.
