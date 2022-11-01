---
title: Comprender el modo de texto básico de las agrupaciones
description: Aprenda qué es el modo de texto, qué es el caso del camello y algún modo de texto básico de "plug and play" que puede usar en sus agrupaciones en Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11369
source-git-commit: 6a695f84e92b576795e69aa843dd96f88b53a355
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 1%

---


# Comprender el modo de texto básico de las agrupaciones

>[!IMPORTANT]
>
>Requisitos previos:
>
>* Explicación de los elementos de informes
>* Comprender los componentes del sistema de informes
>* Crear una agrupación básica


En este vídeo, aprenderá:

* Qué modo de texto es
* Qué caso de camello es
* Algunos modos de texto &quot;plug and play&quot; básicos que puede usar en sus agrupaciones

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12)

## 4 grupos principales

El siguiente modo de texto agrupa tareas basadas en hasta cuatro niveles de elementos principales y deja en blanco a los que no existen.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![Una imagen de pantalla que muestra las tareas del proyecto agrupadas por 4 elementos principales](assets/4-parents-grouping.png)


## Agrupación de porcentaje completado

El siguiente modo de texto agrupa las tareas en función de su porcentaje completado. Las tareas se clasificarán en una de las siguientes categorías cuando se agrupen:

* 0%
* 1% a 25%
* del 26 % al 50 %
* 51% a 75%
* del 76 % al 99 %
* 100 %

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![Imagen de pantalla que muestra las tareas del proyecto agrupadas por porcentaje completado](assets/percent-complete-grouping.png)

## statusEquatesWith, luego status

El siguiente modo de texto agrupa las tareas por statusEquatesWith y, a continuación, por estado.

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![Una imagen de pantalla que muestra las tareas del proyecto agrupadas por statusEquatesWith](assets/status-equates-with.png)


