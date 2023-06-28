---
title: 'Práctica recomendada: Explorador de API'
description: Explore las prácticas recomendadas de los expertos en Adobe Workfront para configurar, administrar y utilizar el Explorador de API de Workfront.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Práctica recomendada: Explorador de API

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas del Explorador de API

* Establezca una convención de nombres para los campos personalizados que se utilizan con integraciones de sistemas de terceros.

* Rastree todos los campos personalizados utilizados en integraciones mediante un proyecto de Workfront.

* Agregue el campo de ID de objeto a los informes que utilice el administrador del sistema.

</br>
</br>

## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Establezca una convención de nombres para los campos personalizados que se utilizan con integraciones de sistemas de terceros.

**He aquí la razón**

Asegúrese de que todos los que crean formularios personalizados conozcan la convención de nomenclatura para que no utilicen accidentalmente un campo reservado para una integración. En función de las integraciones y los flujos de trabajo, el uso del mismo campo de varias formas podría provocar que se modifiquen o sobrescriban datos, y podría provocar que los datos de los informes sean incorrectos.

</br>
</br>


**Práctica recomendada**

Rastree todos los campos personalizados utilizados en integraciones mediante un proyecto de Workfront.

**He aquí la razón**

Un proyecto es el lugar perfecto para registrar nombres de campos personalizados, con qué integración se utilizan, etc. Esto le ayudará a evitar la creación de campos personalizados redundantes o a utilizar el mismo campo personalizado con varias integraciones.

</br>
</br>


**Práctica recomendada**

Agregue el campo de ID de objeto a los informes que utilice el administrador del sistema.

**He aquí la razón**

Los administradores del sistema suelen necesitar hacer referencia a objetos en Workfront por sus números de ID al utilizar API u otras integraciones. Incluya el campo ID en las vistas de los objetos en los que trabaje (proyectos, tareas, problemas, plantillas, formularios personalizados, etc.) para facilitar el acceso y la copia.
