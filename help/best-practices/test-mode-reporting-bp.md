---
title: 'Práctica recomendada: creación de informes en modo de texto'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de los informes de modo de texto de Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
kt: 10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Práctica recomendada: creación de informes en modo de texto

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las mejores prácticas son directrices que representan un curso de acción eficaz y eficiente; sean adoptados fácilmente por usted y los usuarios de su empresa; y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, tenga en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco para ayudarle a guiar la configuración y el uso del sistema Workfront.

## Navegar por esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

La pregunta &quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas para la creación de informes en modo de texto

* Utilice expresiones de valor del modo de texto en lugar de campos personalizados calculados siempre que sea posible en las columnas de informes de lista.

* Coloque los cálculos utilizados en un cálculo de modo de texto en la descripción del informe.

</br>
</br>

## ¿Por qué estas prácticas recomendadas?

**Práctica recomendada**

Utilice expresiones de valor del modo de texto en lugar de campos personalizados calculados siempre que sea posible en las columnas de informes de lista.



**He aquí por qué**

Las expresiones de valor del modo de texto se calculan en el momento en que se ejecuta el informe y se vuelven a calcular cada vez que se actualiza el informe. Esto significa que siempre tendrá datos actualizados e informes precisos.



Los campos personalizados calculados (utilizados en formularios personalizados) no se actualizan automáticamente cuando los datos se muestran en Workfront. En su lugar, muestran los resultados del cálculo más reciente almacenado en Workfront. Esto significa que estos valores podrían estar &quot;obsoletos&quot; o desactualizados en un momento dado. Los campos personalizados calculados deben actualizarse manualmente, ya sea volviendo a calcular la expresión o editando y guardando el objeto que contiene el campo calculado. Esto puede llevar mucho tiempo, así como ser fácil de olvidar.


</br>
</br>

**Práctica recomendada**

Coloque los cálculos utilizados en un cálculo de modo de texto en la descripción del informe.



**He aquí por qué**

Incluir cualquier cálculo de modo de texto en la descripción del informe ayuda a otros a comprender cómo se creó el cálculo y qué tipo de información debería mostrar. También recuerda a los administradores del sistema cómo se creó el informe, en caso de que se necesiten actualizaciones en el futuro.
