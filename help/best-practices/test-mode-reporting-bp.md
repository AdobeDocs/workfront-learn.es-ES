---
title: 'Práctica recomendada: creación de informes en modo de texto'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de los informes de modo de texto de Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 100%

---

# Práctica recomendada: creación de informes en modo de texto

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El punto &quot;¿Por qué estas son prácticas recomendadas?&quot; se encuentra después de la lista de alto nivel, proporciona mayores detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., cuya implementación se debe considerar al trabajar con Workfront.

</br>
</br>

## Prácticas recomendadas para la creación de informes en modo de texto

* Utilice expresiones de valor del modo de texto en lugar de campos personalizados calculados siempre que sea posible en las columnas de lista de informes.

* Coloque los cálculos utilizados en un cálculo de modo de texto en la descripción del informe.

</br>
</br>

## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Utilice expresiones de valor del modo de texto en lugar de campos personalizados calculados siempre que sea posible en las columnas de lista de informes.



**A continuación se explica por qué**

Las expresiones de valor del modo de texto se calculan en el momento en que se ejecuta el informe y se vuelven a calcular cada vez que se actualiza el informe. Esto significa que siempre tendrá datos actualizados e informes precisos.



Los campos personalizados calculados (utilizados en formularios personalizados) no se actualizan automáticamente cuando los datos se muestran en Workfront. En su lugar, muestran los resultados del cálculo más reciente almacenado en Workfront. Esto significa que estos valores podrían estar “obsoletos” o desactualizados en un momento dado. Los campos personalizados calculados deben actualizarse manualmente, ya sea volviendo a calcular la expresión o editando y guardando el objeto que contiene el campo calculado. Esto puede llevar mucho tiempo y es fácil olvidarse de hacerlo.


</br>
</br>

**Práctica recomendada**

Coloque los cálculos utilizados en un cálculo de modo de texto en la descripción del informe.



**A continuación se explica por qué**

Incluir cualquier cálculo de modo de texto en la descripción del informe ayuda a otras personas a comprender cómo se creó el cálculo y qué tipo de información debería mostrar. También recuerda a los administradores del sistema cómo se creó el informe, en caso de que se necesiten actualizaciones en el futuro.
