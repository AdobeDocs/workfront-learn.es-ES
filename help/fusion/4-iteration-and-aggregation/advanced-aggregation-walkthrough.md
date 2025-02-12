---
title: Tutorial de agregación avanzada
description: Aprenda a llamar a un servicio web para que devuelva los detalles acerca de varios países e identificar la población, agrupada por subregión, todo en  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 100%

---

# Tutorial de agregación avanzada

Llame a un servicio web para que le devuelva los detalles acerca de varios países e identificar la población total de todos los países, agrupados por subregión.

![Una imagen del escenario de Fusion](assets/iteration-and-aggregation-3.png)

## Tutorial de agregación avanzada

Workfront recomienda ver el vídeo tutorial del ejercicio antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops)

## Ejercitar direcciones URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`



## Fortalecimiento del principio de agregación

Cada vez que un módulo genera varios paquetes, ejecutará cada uno después.

Para evitarlo, añada un agregador después de un módulo que potencialmente produzca varios paquetes.

Verá una sombra alrededor de cualquier segmento de su escenario desde un **iterador inicial** a un **agregador final**. Esto ayuda a que estos segmentos sean fáciles de identificar en el escenario de Workfront Fusion.

## Su turno

>[!NOTE]
>
>Los ejercicios prácticos y los desafíos son opcionales y no son necesarios para completar la formación de Fusion.

Este ejercicio práctico se basa en lo aprendido en el tutorial, pero no se proporciona la solución.

Cree un nuevo escenario para sumar todas las horas registradas en tareas en proyectos del portafolios de marketing. A continuación, envíe un correo electrónico que indique “Su equipo del proyecto {nombre del proyecto} ha registrado {horas sumadas} del total de {horas planificadas} horas planificadas, lo que le sitúa en el {porcentaje} del plan”.

**Desafío:** vea si puede hacer lo mismo, pero solo para las horas registradas este año.

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=es)
