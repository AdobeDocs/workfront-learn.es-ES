---
title: 'Práctica recomendada: Informes de modo de texto'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de la creación de informes de modo de texto de Workfront.
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10928
exl-id: c624545c-ba42-4cc3-aafe-8be15baadb75
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Práctica recomendada: Informes de modo de texto

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de informes de modo texto

* Utilice expresiones de valor de modo de texto en lugar de campos personalizados calculados siempre que sea posible en columnas de informe de lista.

* Coloque los cálculos utilizados en un cálculo de modo de texto en la descripción del informe.

</br>
</br>

## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Utilice expresiones de valor de modo de texto en lugar de campos personalizados calculados siempre que sea posible en columnas de informes de lista.



**He aquí la razón**

Las expresiones de valor del modo de texto se calculan en el momento de ejecutar el informe y se vuelven a calcular cada vez que se actualiza el informe. Esto significa que siempre tendrá datos actualizados e informes precisos.



Los campos personalizados calculados (que se utilizan en formularios personalizados) no se actualizan automáticamente cuando los datos se muestran en Workfront. En su lugar, muestran los resultados del cálculo más reciente almacenado en Workfront. Esto significa que esos valores pueden estar &quot;obsoletos&quot; o desactualizados en un momento determinado. Los campos personalizados calculados deben actualizarse manualmente, ya sea recalculando la expresión o editando y guardando el objeto que contiene el campo calculado. Esto puede consumir tiempo, así como fácil de olvidar hacer.


</br>
</br>

**Práctica recomendada**

Coloque los cálculos utilizados en un cálculo de modo de texto en la descripción del informe.



**He aquí la razón**

Incluir cálculos en modo de texto en la descripción del informe ayuda a otros a comprender cómo se generó el cálculo y qué tipo de información debería mostrar. También recuerda a los administradores del sistema cómo se creó el informe, en caso de que se necesiten actualizaciones en el futuro.
