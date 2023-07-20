---
title: Cree una expresión de datos SUB, SUM, DIV o PROD
description: Aprenda a utilizar y crear las expresiones matemáticas básicas en un campo calculado de Adobe  [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
jira: KT-8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 80%

---

# Cree una expresión de datos SUB, SUM, DIV o PROD

Este vídeo contiene información sobre:

* Qué hacen las expresiones SUB, SUM, DIV y PROD
* Creación de una expresión de datos SUB en un campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12&learn=on)

## Información adicional: expresión ROUND

### Creación de una expresión ROUND

La expresión ROUND toma cualquier número y lo redondea a un determinado número de decimales.

La mayoría de las veces, la expresión de datos ROUND se utiliza junto con otra expresión de datos y cuando el campo de formato se deja como Texto o Número.

Vamos a crear un campo calculado para determinar la diferencia entre el número de horas planificadas y las horas realmente registradas en una tarea, que requiere la expresión SUB y tiene este aspecto:

**SUB({workRequired},{actualWorkRequired})**

Dado que el tiempo se rastrea en minutos y el formato preferido es mostrar la información en horas, la expresión también necesita dividirse en 60 y tener este aspecto:

**DIV(SUB({workRequired},{actualWorkRequired}),60)**

Si el formato se cambia a Número al crear el campo calculado en el formulario personalizado, puede cambiar el formato de número al agregar el campo en una vista.

![Equilibrador de carga de trabajo con informe de utilización](assets/round01.png)

Sin embargo, si el formato del campo al crear un campo personalizado se deja como Texto, el formato no se puede cambiar fácilmente dentro de la vista. La expresión ROUND debe utilizarse para evitar ver números como este en el proyecto:

![Equilibrador de carga de trabajo con informe de utilización](assets/round02.png)

<b>Utilizar la expresión de datos ROUND en un campo calculado</b>

La expresión ROUND incluye el nombre de la expresión (ROUND) y, normalmente, dos puntos de datos. Estos puntos de datos pueden ser una expresión o un campo en Workfront, seguido de un número para indicar cuántos lugares decimales desea utilizar.

Una expresión está estructurada de esta manera: ROUND(punto de datos, #)

En la expresión que calcula la diferencia entre las horas planificadas y las reales, utilice esta expresión: DIV(SUB({workRequired},{actualWorkRequired}),60) como primer punto de datos. A continuación, asegúrese de que el número que proviene de esa expresión no vaya más de 2 lugares a la derecha del decimal.

![Equilibrador de carga de trabajo con informe de utilización](assets/round03.png)

La expresión podría escribirse de esta manera: ROUND(DIV(SUB({workRequired},{actualWorkRequired}),60),2).
