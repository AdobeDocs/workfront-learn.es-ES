---
title: Crear expresiones ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS
description: Aprenda a utilizar y crear las expresiones AÑADIR en un campo calculado en Adobe [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Crear expresiones ADDDAYS, ADDWEEKDAY, ADDMONTHS, ADDYEARS

En este vídeo, aprenderá lo siguiente:

* Cálculo de las expresiones ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR
* Cómo crear una expresión de datos ADDWEEKDAYS en un campo calculado

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12)

## Ejemplos adicionales

A continuación se muestran algunas expresiones adicionales de ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR que los clientes de Adobe Workfront han creado.

**Debería haber terminado para el**

El cliente quería saber cuándo se debería haber completado la tarea en función de la fecha de inicio real y la duración planificada. La fecha proyectada de finalización no funcionará en este caso porque puede moverse si la tarea está atrasada y la fecha planificada de finalización no ayuda si hay retrasos en tareas anteriores.

La expresión creada fue ADDDAYS({actualStartDate},{durationMinutes}/480)

El tiempo del campo Duración se almacena en minutos. Por lo tanto, en esta expresión, el campo Duración no puede ser independiente si el tiempo se va a reflejar en días. Para que esto suceda, la Duración debe dividirse en 480 minutos (480 minutos = 8 horas = 1 día)

Por este motivo, la segunda ranura de valor contiene (Duration/480).


**Fecha de finalización de factura**

Este ejemplo incluye no solo utiliza la expresión ADDDAYS, sino un campo personalizado creado y guardado anteriormente en el formulario personalizado.

El cliente está registrando la fecha en la que se envía una factura mediante un campo de fecha personalizado denominado &quot;Fecha de envío de factura&quot;.

Una vez enviada, la factura debe completarse y archivarse en un plazo de 30 días. Para producir automáticamente esa fecha de finalización y presentación, se utiliza un campo calculado ADDDAYS junto con el campo personalizado &quot;Fecha de envío de factura&quot;. La expresión tiene este aspecto:

ADDDAYS({DE:Fecha de envío de factura},30)
