---
title: 'Práctica recomendada: estados'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de los estados de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
kt: 10926
exl-id: c3a4fe42-339c-4063-ad67-045868bbc6b1
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# Práctica recomendada: estados

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las mejores prácticas son directrices que representan un curso de acción eficaz y eficiente; sean adoptados fácilmente por usted y los usuarios de su empresa; y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, tenga en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco para ayudarle a guiar la configuración y el uso del sistema Workfront.

## Navegar por esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

La pregunta &quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas sobre los estados

* Al cambiar el nombre de los estados predeterminados de Workfront, mantenga el propósito original del estado igual.

* Si crea un estado de proyecto personalizado para Cancelado, equipare el estado con Muerto.

* Mantenga los estados personalizados globales al mínimo.

* No utilice estados de proyecto en lugar de tareas para indicar la progresión de un proyecto.


</br>
</br>



## ¿Por qué estas prácticas recomendadas?

**Práctica recomendada**

Al cambiar el nombre de los estados predeterminados de Workfront, mantenga el propósito original del estado igual.



**He aquí por qué**

Algunas acciones de Workfront se activan mediante los estados predeterminados del sistema. Cambiar la intención de un estado puede afectar al comportamiento de Workfront en determinadas situaciones, afectar a los informes, etc.



Por ejemplo, el estado de tarea predeterminado de Complete indica a Workfront que cambie el porcentaje completado de una tarea al 100%. El estado Complete también permite a Workfront saber que se puede iniciar el trabajo en tareas dependientes. Si ha cambiado el nombre del estado a Esperando, para indicar que un trabajo en una tarea está en pausa, Workfront va a pensar que la tarea ha finalizado y dar los pasos siguientes en el proyecto.

</br>
</br>



**Práctica recomendada**

Si crea un estado de proyecto personalizado para Cancelado, equipare el estado con Muerto.



**He aquí por qué**

Si se equipara Cancelado con Finalizado, no se puede utilizar el estado para cancelar un proyecto a menos que todas las tareas estén marcadas como Completas y que se hayan cerrado todos los problemas. Pero si se equipara Cancelado con Muerto, se puede cancelar el proyecto sin cambiar nada en el registro histórico.


</br>
</br>

**Práctica recomendada**

Mantenga los estados personalizados globales al mínimo.



**He aquí por qué**

Menos es más. Además de crear mantenimiento innecesario, demasiados estados personalizados crean confusión, especialmente al trabajar en proyectos interfuncionales. En su lugar, haga que los estados personalizados sean específicos del grupo. Esto mantiene el entorno de Workfront más limpio y mejor posicionado para la expansión a otros grupos en el futuro. Trabaje con su comité de gobernanza/supervisión y con las partes interesadas para identificar los estados que deben utilizar los grupos de su organización.


</br>
</br>

**Práctica recomendada**

No utilice estados de proyecto en lugar de tareas para indicar la progresión de un proyecto.



**He aquí por qué**

Mantenga los estados del proyecto sencillos para indicar fases de progreso de alto nivel, como Planificación, Actual, Complete, etc. Permita que las tareas, los estados de las tareas y el porcentaje de finalización de la tarea le digan cómo progresa el trabajo en general en el proyecto. Estos indicadores de nivel de tarea se resumen en el porcentaje de finalización del proyecto, la condición del proyecto y el estado del progreso del proyecto, todos los cuales son indicadores mejores y más precisos de la progresión del proyecto que un estado del proyecto. Además, esta información de nivel de tarea proporciona mejores informes de proyecto.
