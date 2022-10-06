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
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# Crear DIRECCIONES DE ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

En este vídeo, aprenderá:

* Cálculo de las expresiones ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR
* Creación de una expresión de datos ADDWEEKDAYS en un campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## Ejemplos adicionales

A continuación se muestran algunos Adobes adicionales de expresiones ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR [!DNL Workfront] Los clientes de han creado.

**Debería haber sido hecho por**

El cliente desea saber cuándo se debe completar la tarea en función de la fecha de inicio real y la duración planeada. La fecha de finalización prevista no funcionará en este caso porque puede moverse si la tarea está atrasada y la fecha de finalización prevista no ayuda si hay retrasos en tareas anteriores.

La expresión creada era ADDDAYS(Fecha de inicio real,(Duración/480))

El tiempo en el campo Duración se almacena en minutos. Por lo tanto, en esta expresión, el campo Duration no puede estar solo si se desea reflejar la hora en días. Para que esto ocurra, la duración debe dividirse en 480 minutos (480 minutos = 8 horas = 1 día)

Por este motivo, la segunda ranura contiene (Duration/480).


**Fecha de finalización de factura**

Este ejemplo incluye otro campo calculado, ya creado y guardado en el sistema, dentro de la expresión .

El cliente capturaba la fecha en que se envió la factura a través de un campo de fecha personalizado, titulado &quot;Fecha de envío de factura&quot;, en el formulario personalizado. Una vez enviadas, tienen 30 días para completar y archivar la factura. Para producir automáticamente esa fecha de finalización y de archivo, crearon un campo calculado con ADDDAYS y el campo Fecha de envío de factura . La expresión tenía este aspecto:

ADDDAYS(Fecha de envío de factura,30)
