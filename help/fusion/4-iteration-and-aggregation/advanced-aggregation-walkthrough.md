---
title: Tutorial de agregación avanzada
description: Aprenda a llamar a un servicio web para devolver detalles sobre varios países e identificar la población, agrupada por subregión, todo en [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Tutorial de agregación avanzada

## Información general

Llame a un servicio web para devolver detalles sobre varios países e identificar la población total de todos los países, agrupada por subregión.

![Una imagen del escenario de Fusion](assets/iteration-and-aggregation-3.png)

## Tutorial de agregación avanzada

Workfront recomienda ver el vídeo del tutorial de ejercicios antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12)

## URL del ejercicio

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>Para obtener instrucciones paso a paso sobre cómo completar el tutorial, vaya a la [Tutorial de agregación avanzada](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) hacer ejercicio.

## Refuerzo del principio de agregación

Cada vez que un módulo genera varios paquetes, cada módulo después de eso ejecutará cada paquete.

Para evitarlo, agregue un agregador después de un módulo que pueda producir varios paquetes.

Verá una sombra alrededor de cualquier segmento en su escenario desde un **inicio-iterador** a la **agregador final**. Esto ayuda a que estos segmentos sean fáciles de identificar en su escenario de Workfront Fusion.

## Tu turno

>[!NOTE]
>
>Los ejercicios y desafíos de práctica son opcionales y no son necesarios para completar el entrenamiento de Fusion.

Este ejercicio práctico se basa en lo que ha aprendido en el tutorial, pero no se proporciona la solución.

Cree un nuevo escenario para sumar todas las horas registradas en las tareas de los proyectos en el portafolio de marketing. A continuación, envíe un correo electrónico que indique &quot;Su equipo del proyecto {Project Name} ha registrado {summed hours} del total de {planned hours} horas planificadas, lo que le sitúa en {percentage} del plan&quot;.

**Reto:** Vea si puede hacer lo mismo, pero solo para las horas registradas este año.

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
