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
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:33:27.197Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 258
ht-degree: 91%

---

# Tutorial de agregación avanzada

Llame a un servicio web para que le devuelva los detalles acerca de varios países e identificar la población total de todos los países, agrupados por subregión.

![Una imagen del escenario de Fusion](assets/iteration-and-aggregation-3.png)

## Tutorial de agregación avanzada

Workfront recomienda ver el vídeo tutorial del ejercicio antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on&enablevpops=1)

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

Cree un nuevo escenario para sumar todas las horas registradas en tareas en proyectos del portafolios de marketing. A continuación, envíe un mensaje de correo electrónico que indique &quot;Su equipo del proyecto {Project Name} ha registrado {summed hours} del total de {planned hours} horas planificadas, lo que le sitúa en {percentage} del plan&quot;.

**Desafío:** vea si puede hacer lo mismo, pero solo para las horas registradas este año.

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
