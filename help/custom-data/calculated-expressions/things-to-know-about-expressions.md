---
title: Aspectos que se deben conocer sobre las expresiones de campo calculado
description: Obtenga información sobre lista de conceptos que son útiles para conocer al trabajar con campos calculados personalizados en [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: to-know-expressions.png
exl-id: 512a3071-f47f-4fd4-bf5f-9b18bef8ba59
source-git-commit: 71f9ec5fad80664cc1d1f12c6772b131ee46c59c
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 0%

---

# Aspectos que se deben conocer sobre las expresiones de campo calculado

A continuación se muestra una lista de conceptos útiles para saber al trabajar con campos calculados personalizados en Workfront.

## Carcasa las materias en los nombres de expresiones

Cuando se trata de nombres de expresiones, el uso de mayúsculas y minúsculas importa. Al escribir inicialmente un nombre de expresión, puede utilizar mayúsculas, minúsculas o una combinación de ambas.

![Mensaje de error sin mayúsculas en el nombre de la expresión](assets/T2K01.png)

Sin embargo, la expresión debe escribirse en mayúsculas para que el sistema reconozca la expresión y guarde el campo.



## Las horas se almacenan en minutos

Las horas de la base de datos de Workfront se almacenan en minutos. Si hace referencia a campos como Horas planificadas u Horas reales, divida entre 60 para mostrar el tiempo en horas y no en minutos.

## El espaciado no afecta a las expresiones

La forma recomendada de escribir expresiones es con poco o ningún espacio entre cada expresión.

* IF(ISBLANK({description}),&quot;Sin descripción&quot;,&quot;Tiene descripción&quot;)

![Expresiones sin espaciado entre campos](assets/T2K02.png)

Sin embargo, si el espaciado le ayuda a ver lo que está sucediendo, se puede añadir algo de espacio a las expresiones. Los espacios adicionales no deben impedir que la expresión recopile o calcule un valor en [!DNL Workfront].

* IF (ISBLANK ({description}), &quot;Sin descripción&quot; , &quot;Tiene descripción&quot; )

![Expresiones con espaciado entre campos](assets/T2K03.png)

Las únicas cosas que no pueden tener espacios entre ellos son los campos y las llaves. De lo contrario, recibirá un mensaje de error y no podrá guardar el campo ni el formulario personalizado.

![Error al espaciar el nombre del campo con el corchete](assets/T2K04.png)

## Las comillas deben ser rectas

Cuando utilice comillas en una expresión, asegúrese de que las comillas sean rectas (&quot;). Si las comillas son curvas (&quot;), la variable [!DNL Workfront] El sistema seguirá mostrando el mensaje &quot;Expresión personalizada no válida&quot;.

![Error con comillas curvas](assets/T2K05.png)

## Actualización de cálculos al guardar el formulario y editar objetos

Este es un aspecto importante de los campos calculados que se debe comprender.

La información mostrada en un campo calculado sigue siendo la misma y queda obsoleta a menos que se recalcule el formulario personalizado.

Las expresiones se pueden actualizar utilizando la opción Recalcular expresiones del menú Más de un objeto.

Desea ver el número de días que se ha abierto un problema. Cree un campo calculado llamado &quot;Días abiertos&quot; con la expresión DATEDIFF.

* Nombre de campo = Días abiertos
* Expresión = DATEDIFF({entryDate},$$TODAY)

Una vez guardado, el número de días entre el momento en que se creó el problema o se introdujo en Workfront, y la fecha de hoy se puede mostrar en la página de detalles de un objeto o en una vista de informe.

Al ver la misma página de detalles o vista de informe al día siguiente, espera que ese número se incremente en uno. Si el número es 5 hoy, deberían ser 6 mañana. El día siguiente debe ser 7, luego 8, etc.

Sin embargo, el campo seguirá mostrando 5 cada día. El campo debe &quot;volver a ejecutarse&quot; o recalcularse para actualizar la información.

Para actualizar un campo mediante la opción Recalcular expresiones:

* Haga clic en el nombre del objeto para abrirlo.
* Haga clic en el menú Más.
* Seleccione Recalcular expresiones en la lista.

![Opción de recalcular expresión en el objeto](assets/T2K06.png)

También puede recalcular varias expresiones al mismo tiempo mediante la función de &quot;edición masiva&quot; en una lista o informe. Supongamos que ha creado un informe que muestra una lista de problemas con el cálculo de Días abiertos que aparece en una columna. Si desea volver a calcular todos los problemas a la vez:

* Seleccione todos los problemas en el informe.
* Seleccione la opción Editar para editar por lotes todos los problemas seleccionados.
* Haga clic en la etiqueta de Forms personalizada a la izquierda para desplazarse hacia abajo hasta la sección de formularios personalizados.
* Marque la casilla Recalcular expresiones personalizadas en la parte inferior de la sección Forms personalizado.
* Haga clic en Guardar cambios.

![Opción Recalcular expresión para varios objetos](assets/T2K07.png)

La pantalla se actualiza para mostrar información actualizada en el campo calculado.

**Nota**: Aunque hay otras formas de actualizar o volver a calcular las expresiones en un campo calculado, esta es la forma más rápida y sencilla.

## Los cálculos pueden variar de un formulario a otro dentro del mismo campo

Tan pronto como se guarda un campo calculado en un formulario personalizado y se guarda el formulario personalizado, el campo calculado se agrega a la Biblioteca de campos para que se pueda utilizar en otros formularios personalizados.

Sin embargo, si tiene un campo calculado en el formulario A y el mismo campo calculado en el formulario B, la idea inicial es que los cálculos sean exactamente los mismos. No siempre es así. El campo calculado en el formulario A podría estar calculando de una manera completamente diferente en el formulario B.

Cuando se selecciona un campo personalizado calculado de la biblioteca de campos y se agrega a un formulario personalizado, el campo se agrega pero el cálculo está en blanco. Una razón por la que esto sucede es que el cálculo puede hacer referencia a campos que no existen para otro tipo de objeto.

Por ejemplo, ha creado un campo calculado, &quot;Días para completar&quot;, para determinar cuánto tiempo se tardó en completar una tarea en un proyecto.

* WEEKDAYDIFF({actualStartDate},{actualCompletionDate})

Desea hacer lo mismo para una iteración. Puede utilizar la misma expresión; sin embargo, los campos disponibles para un objeto de tarea no siempre están disponibles para un objeto de iteración. Entonces [!DNL Workfront] le da la oportunidad de generar el cálculo con los campos de objeto correctos.

**Sugerencia profesional**: copie la expresión calculada del cuadro Cálculo al campo Instrucciones al crear campos personalizados. Este campo no se borra cuando se agrega un campo personalizado calculado al formulario personalizado desde la biblioteca de campos.

Según la necesidad, los campos calculados en los formularios personalizados pueden ser bastante simples o muy complejos. Las expresiones pueden incrustar o anidar otras expresiones y valores para proporcionar el nivel de detalle necesario y obtener una mejor imagen de lo que está pasando con el trabajo realizado en su organización.

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you’re ready to start building your own calculated custom fields.-->
