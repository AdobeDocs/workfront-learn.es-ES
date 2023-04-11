---
title: Introducción a la agregación avanzada
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
source-git-commit: 57b112921738c01fe4222e50403c8953c412a0f7
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Introducción a la agregación avanzada

Llame a un servicio Web para devolver detalles sobre varios países e identificar la población total de todos los países, agrupados por subregiones.

![Una imagen del escenario de fusión](assets/iteration-and-aggregation-3.png)

## Introducción a la agregación avanzada

Workfront recomienda ver el vídeo tutorial del ejercicio antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on)

## Ejercitar direcciones URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>Para obtener instrucciones paso a paso sobre cómo completar el tutorial, vaya a la [Introducción a la agregación avanzada](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) ejercicio.

## Fortalecimiento del principio de agregación

Cada vez que un módulo genera varios paquetes, cada módulo después de eso ejecutará cada paquete.

Para evitarlo, agregue un agregador después de un módulo que potencialmente produce varios paquetes.

Verá una sombra alrededor de cualquier segmento de su escenario desde un **iterador inicial** a **agregador final**. Esto ayuda a que estos segmentos sean fáciles de identificar en el escenario de Workfront Fusion.

## Su turno

>[!NOTE]
>
>Los ejercicios prácticos y los desafíos son opcionales y no son necesarios para completar la formación de Fusion.

Este ejercicio de práctica se basa en lo aprendido en el tutorial, pero no se proporciona la solución.

Cree un nuevo escenario para sumar todas las horas que haya iniciado sesión en tareas en proyectos del portafolio de marketing. A continuación, envíe un correo electrónico que indique &quot;Su equipo de proyecto de {Nombre del proyecto} ha registrado {horas acumuladas} del total de {horas programadas} horas planificadas, lo que le sitúa en el {porcentaje} del plan&quot;.

**Desafío:** Vea si puede hacer lo mismo pero solo para las horas registradas este año.

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
