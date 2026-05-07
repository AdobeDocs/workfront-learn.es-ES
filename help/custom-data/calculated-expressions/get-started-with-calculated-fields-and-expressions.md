---
title: Introducción a los campos calculados y las expresiones
description: Obtenga información sobre cómo crear expresiones en campos calculados para recopilar datos personalizados únicos sobre el trabajo que realiza su organización.
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: gs-calc-fields-expressions.png
exl-id: fbd17f01-9e97-4ead-9a56-7ce4f81255ec
TQID: https://experienceleague.adobe.com/M1mfJ1cT5sXOC8-0qJAihKIBAJBHt1hCQJux3o3UEf8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: d3cdead0-685a-4489-9250-4bb709942f66
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 505
ht-degree: 100%

---

# Introducción a los campos calculados y las expresiones

<!--
**Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.
-->

Workfront proporciona una variedad de campos que son comunes en múltiples áreas de negocio y que se utilizan habitualmente para la administración del trabajo. Campos como fecha planificada de finalización, presupuesto del proyecto, nombre del usuario asignado de la tarea, etc.

Sin embargo, cada organización tiene datos específicos de su sector y compañía que deben recopilarse para comprender si se cumplen los objetivos de la empresa. Por ejemplo, su organización desea realizar un seguimiento de lo siguiente:

* La línea de negocio a la que contribuirá un proyecto.
* Si la financiación proviene de proveedores, internos o ambos.
* La resolución que se necesita para las imágenes utilizadas.

Aunque estos campos no están integrados de forma inherente en [!DNL Workfront], puede crear campos de entrada de datos personalizados y campos de respuesta rellenados previamente y de selección múltiple mediante un formulario personalizado.

Esta ruta de aprendizaje se centra en el campo calculado. Aprenderá qué es un campo calculado, los diferentes tipos de información que puede extraer del campo calculado a través de expresiones de datos y cómo crear esos campos calculados para mejorar la recopilación de datos y la creación de informes.

![La administración de recursos configura un localizador](assets/GS01.png)

## ¿Qué es un campo calculado?

Un campo calculado contiene datos personalizados creados mediante expresiones de datos y campos de Workfront existentes.

![Equilibrador de carga de trabajo con informe de utilización](assets/GS02.png)

Por ejemplo, su organización tiene un sistema específico de numeración de proyecto o número de trabajo que incluye lo siguiente:

* El año en el que se creó el proyecto.
* Las iniciales del propietario del proyecto.
* El número de referencia del proyecto de [!DNL Workfront].


Con las expresiones en un campo calculado, puede tomar cada parte de la información ya almacenada en [!DNL Workfront] y crear ese ID de proyecto único, o número de trabajos, que luego puede agregar a un informe de esta manera:

![Equilibrador de carga de trabajo con informe de utilización](assets/GS03.png)

Según los datos específicos necesarios, los campos calculados pueden ser simples, utilizar una o dos expresiones o, lo que es más complicado, utilizar varias expresiones incrustadas. Tenga en cuenta que Workfront solo puede utilizar datos ya almacenados o extraídos del sistema para campos calculados.

## Expresiones de texto

Las expresiones de texto buscan, diseccionan y combinan información encontrada en [!DNL Workfront] para crear datos más significativos u obtener una buena perspectiva sobre el trabajo que realiza su organización.

Por ejemplo, las expresiones de texto se pueden utilizar para lo siguiente:

* Mostrar “Más de 5000 dólares” cuando los gastos del proyecto superen los 5000 dólares o &quot;Menos de 5000 dólares&quot; cuando los gastos estén por debajo de eso, en una columna de la vista del proyecto.

* Asigne a cada proyecto un número único que incluya el año en que se creó el proyecto, el número de referencia de [!DNL Workfront] del proyecto, el nombre y las iniciales del propietario del proyecto.

* Cree un informe que enumere todos los proyectos que no estén asignados a un portafolio o a un programa para que pueda utilizarlos en las reuniones del administrador.

Las expresiones de texto se pueden utilizar en un campo personalizado para realizar estos tipos de búsquedas y combinaciones en Workfront.

Al consultar las posibles expresiones de texto, encontrará varias opciones.

![La administración de recursos configura un localizador](assets/TE01.png)

Hay seis expresiones de texto que se utilizan con más frecuencia:

* CONCAT
* IZQUIERDA/DERECHA
* CONTAINS
* IF
* ISBLANK