---
title: 'Práctica recomendada: Explorador de API'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de la API Explorer de Workfront.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
kt: 10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Práctica recomendada: Explorador de API

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las mejores prácticas son directrices que representan un curso de acción eficaz y eficiente; sean adoptados fácilmente por usted y los usuarios de su empresa; y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, tenga en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco para ayudarle a guiar la configuración y el uso del sistema Workfront.

## Navegar por esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

La pregunta &quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de API Explorer

* Establezca una convención de nombres para campos personalizados que se utilicen con integraciones de sistemas de terceros.

* Rastree todos los campos personalizados utilizados en integraciones que utilizan un proyecto de Workfront.

* Agregue el campo ID de objeto a los informes que utilice el administrador del sistema.

</br>
</br>

## ¿Por qué estas prácticas recomendadas?

**Práctica recomendada**

Establezca una convención de nombres para campos personalizados que se utilicen con integraciones de sistemas de terceros.

**He aquí por qué**

Asegúrese de que todos los usuarios que crean formularios personalizados conozcan la convención de nomenclatura, de modo que no utilicen accidentalmente un campo reservado para una integración. En función de las integraciones y los flujos de trabajo, el uso del mismo campo de varias formas podría provocar la modificación o sobrescritura de los datos, lo que podría dar como resultado datos incorrectos en los informes.

</br>
</br>


**Práctica recomendada**

Rastree todos los campos personalizados utilizados en integraciones que utilizan un proyecto de Workfront.

**He aquí por qué**

Un proyecto es el lugar perfecto para registrar nombres de campo personalizados, con qué integración se utilizan, etc. Esto le ayudará a evitar la creación de campos personalizados redundantes o el uso del mismo campo personalizado con varias integraciones.

</br>
</br>


**Práctica recomendada**

Agregue el campo ID de objeto a los informes que utilice el administrador del sistema.

**He aquí por qué**

Los administradores del sistema suelen tener que hacer referencia a objetos de Workfront por sus números de ID al utilizar API u otras integraciones. Incluya el campo ID en las vistas de los objetos en los que trabaje (proyectos, tareas, problemas, plantillas, formularios personalizados, etc.) para facilitar el acceso y la copia.
