---
title: 'Práctica recomendada: creación de informes en modo de texto'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de los informes de modo de texto de Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
TQID: https://experienceleague.adobe.com/k8DYutzVcGrJc7p0x74B2iQ3nkiohWeQu1egOWZ34AI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 90%

---

# Práctica recomendada: creación de informes en modo de texto

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, encontrará en primer lugar una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

El área &quot;¿Por qué son estas prácticas recomendadas?&quot;, que se encuentra después de la lista de alto nivel, proporciona más detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

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
