---
title: 'Práctica recomendada: explorador de API'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso del Explorador de API de Workfront.
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 100%

---

# Práctica recomendada: explorador de API

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El punto &quot;¿Por qué estas son prácticas recomendadas?&quot; se encuentra después de la lista de alto nivel, proporciona mayores detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., cuya implementación se debe considerar al trabajar con Workfront.

</br>
</br>

## Prácticas recomendadas del Explorador de API

* Establezca una convención de nomenclatura para campos personalizados que se usan con integraciones de sistemas de terceros.

* Rastree todos los campos personalizados usados en integraciones que utilizan un proyecto de Workfront.

* Añada el campo ID de objeto a los informes que utilice el administrador del sistema.

</br>
</br>

## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Establezca una convención de nomenclatura para campos personalizados que se usan con integraciones de sistemas de terceros.

**A continuación se explica por qué**

Asegúrese de que quienes crean formularios personalizados conocen la convención de nomenclatura, para que no utilicen accidentalmente un campo reservado para una integración. En función de las integraciones y de los flujos de trabajo, el uso del mismo campo de varias formas podría provocar la modificación o sobrescritura de los datos, lo que podría dar como resultado datos incorrectos en los informes.

</br>
</br>


**Práctica recomendada**

Rastree todos los campos personalizados usados en integraciones que utilizan un proyecto de Workfront.

**A continuación se explica por qué**

Un proyecto es el lugar perfecto para registrar nombres de campo personalizados, con qué integración se usan, etc. Esto ayuda a evitar la creación de campos personalizados redundantes o el uso del mismo campo personalizado con varias integraciones.

</br>
</br>


**Práctica recomendada**

Añada el campo ID de objeto a los informes que utilice el administrador del sistema.

**A continuación se explica por qué**

Los administradores del sistema a menudo tienen que hacer referencia a objetos de Workfront por sus números de ID al utilizar API u otras integraciones. Incluya el campo ID en las vistas de los objetos en los que trabaje (proyectos, tareas, problemas, plantillas, formularios personalizados, etc.) para facilitar el acceso y la copia.
