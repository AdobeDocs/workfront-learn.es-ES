---
title: 'Práctica recomendada: programaciones'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de las programaciones de Workfront.
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10925
exl-id: 508d6f90-f9f4-4f12-9bf1-5e89246f3e3a
TQID: https://experienceleague.adobe.com/Lxc0Ymk5tPPsIvM4iKGS68o7eJpFCjgOwWtcQ67aWp4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d3382524-5489-431b-bde9-271ab257bc37
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 560
ht-degree: 100%

---

# Práctica recomendada: programaciones

## ¿Qué es una “práctica recomendada” de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de “por qué”.

La pregunta “¿Por qué son estas prácticas recomendadas?” se encuentra después de la lista de alto nivel, proporciona mayores detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., cuya implementación se debe considerar al trabajar con Workfront.

</br>
</br>

## Programa las prácticas recomendadas

* Limite el número de programaciones que crea en Adobe Workfront.

* El total de horas de trabajo de cada día laborable de la programación debe ser igual al número de horas de un día especificado en las preferencias globales del proyecto.

* Añada un recordatorio al calendario del administrador del sistema de Adobe Workfront para actualizar las programaciones cada año a una hora determinada.


Para obtener instrucciones sobre cómo crear y administrar programaciones, consulte el tutorial [Crear y administrar programaciones](/help/administration-and-setup/configure-system-defaults/create-and-manage-schedules.md).

</br>
</br>

## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Limite el número de programaciones que crea en Adobe Workfront.



**He aquí por qué**

No cree decenas de programaciones para grupos, equipos o personas diferentes. Una menor cantidad de programaciones implica un menor mantenimiento por parte de los administradores del sistema o del grupo.



Es posible que se necesiten programas separados cuando:

* Los empleados están en diferentes zonas horarias (EE. UU. Pacífico vs. Este de EE. UU.) o en diferentes regiones (EMEA frente a APAC).

* Tiene trabajadores a tiempo parcial que trabajan menos de 40 horas por semana.

* Los trabajadores no trabajan las ocho horas normales diarias, de lunes a viernes, como los trabajadores de fin de semana o los que trabajan cuatro días durante 10 horas al día.

</br>
</br>

**Práctica recomendada**

El total de horas de trabajo de cada día laborable de la programación debe ser igual al número de horas de un día especificado en las preferencias globales del proyecto.



**He aquí por qué**

Si el total de horas de trabajo no coincide, puede dar como resultado cálculos de fecha y hora aparentemente incorrectos en la cronología del proyecto y en los informes.

Por ejemplo, si la preferencia del sistema es de ocho horas diarias y la programación asignada a un proyecto solo tiene siete horas laborables al día, verá que una tarea con una duración de un día tarda más de un día en completarse, porque está intentando encajar las ocho horas.

**Nota**: La configuración del proyecto global del sistema se realiza en Configuración > Preferencias del proyecto > Cálculos de cronología > Horas típicas por día laboral.

</br>
</br>


**Práctica recomendada**

Añada un recordatorio al calendario del administrador del sistema de Adobe Workfront para actualizar las programaciones cada año a una hora determinada.

**He aquí por qué**

Actualice las programaciones en la instancia de Workfront con días festivos nacionales, días festivos de la compañía y otros días en los que los usuarios no trabajan. Haga esto en un momento determinado cada año, ya sea al final del año o cuando Recursos Humanos publique las programaciones de vacaciones, de modo que las cronologías del proyecto, la planificación de recursos, etc., reflejen la disponibilidad precisa del usuario.
