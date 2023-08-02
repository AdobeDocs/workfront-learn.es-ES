---
title: Crear expresiones de ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS
description: Aprenda a utilizar y crear las expresiones ADD en un campo calculado en Adobe [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: ht
source-wordcount: '273'
ht-degree: 100%

---

# Crear expresiones de ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

Este vídeo contiene información sobre:

* Qué se calcula con las expresiones ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR
* Cómo crear una expresión de datos ADDWEEKDAYS en un campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## Ejemplos adicionales

A continuación se muestran algunas expresiones adicionales ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR que han creado los clientes de Adobe Workfront.

**Debería haberse terminado el**

El cliente desea saber cuándo se debe completar la tarea en función de la fecha de inicio real y la duración planificada. La fecha de finalización prevista no funcionará en este caso porque puede moverse si la tarea está atrasada y la fecha planificada de finalización no ayuda si hay retrasos en tareas anteriores.

La expresión creada era ADDDAYS({actualStartDate}, {durationMinutes}/480)

El tiempo en el campo Duración se almacena en minutos. Por lo tanto, en esta expresión, el campo Duración no puede mantenerse por sí solo si se desea reflejar la hora en días. Para que esto ocurra, la duración debe dividirse en 480 minutos (480 minutos = 8 horas = 1 día)

Por este motivo, el segundo espacio contiene (Duración/480).


**Fecha de finalización de la factura**

Este ejemplo incluye no solo la utilización de la expresión ADDDAYS, sino también un campo personalizado creado anteriormente y guardado en el formulario personalizado.

El cliente está capturando la fecha en la que se presenta una factura a través de un campo de fecha personalizado denominado &quot;Fecha de envío de factura&quot;.

Una vez presentada, la factura debe completarse y cumplimentarse en un plazo de 30 días. Para producir automáticamente esa fecha de finalización y de archivo, se utiliza un campo calculado ADDDAYS junto con el campo personalizado “Fecha de envío de la factura”. La expresión tiene el aspecto siguiente:

ADDDAYS({DE:Fecha de envío de factura},30)
