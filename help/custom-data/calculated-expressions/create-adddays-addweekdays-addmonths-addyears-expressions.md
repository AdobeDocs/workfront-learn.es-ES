---
title: Crear DIRECCIONES DE ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS
description: Aprenda a utilizar y crear las expresiones ADD en un campo calculado en Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
source-git-commit: 9cc845d6efe2ee27e66ad7de4e1800cb9077aebd
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Crear DIRECCIONES DE ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

En este vídeo, aprenderá:

* Cálculo de las expresiones ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR
* Creación de una expresión de datos ADDWEEKDAYS en un campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## Ejemplos adicionales

A continuación se muestran algunas expresiones adicionales ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR que han creado los clientes de Adobe Workfront.

**Debería haber sido hecho por**

El cliente desea saber cuándo se debe completar la tarea en función de la fecha de inicio real y la duración planeada. La fecha de finalización prevista no funcionará en este caso porque puede moverse si la tarea está atrasada y la fecha de finalización prevista no ayuda si hay retrasos en tareas anteriores.

La expresión creada era ADDDAYS({actualStartDate},{durationMinutes}/480)

El tiempo en el campo Duración se almacena en minutos. Por lo tanto, en esta expresión, el campo Duration no puede estar solo si se desea reflejar la hora en días. Para que esto ocurra, la duración debe dividirse en 480 minutos (480 minutos = 8 horas = 1 día)

Por este motivo, la segunda ranura contiene (Duration/480).


**Fecha de finalización de factura**

Este ejemplo incluye no solo utiliza la expresión ADDDAYS, sino también un campo personalizado creado anteriormente y guardado en el formulario personalizado.

El cliente está capturando la fecha en la que se envía una factura a través de un campo de fecha personalizado llamado &quot;Fecha de envío de factura&quot;.

Una vez presentada, la factura debe completarse y presentarse en un plazo de 30 días. Para producir automáticamente esa fecha de finalización y de archivo, se utiliza un campo calculado ADDDAYS junto con el campo personalizado &quot;Fecha de envío de factura&quot;. La expresión tiene este aspecto:

ADDDAYS({DE:Fecha de envío de factura},30)
