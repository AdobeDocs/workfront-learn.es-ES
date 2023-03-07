---
title: Comprender el modo de texto básico de las agrupaciones
description: Aprenda qué es el modo texto, qué es camel case y algunos modos de texto básicos "plug and play" que puede utilizar en sus agrupaciones en Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Comprender el modo de texto básico de las agrupaciones

>[!IMPORTANT]
>
>Requisitos previos:
>
>* Comprender los elementos de informes
>* Comprender los componentes de informes
>* Crear una agrupación básica


>[!TIP]
>
>* Para comprender mejor el modo de texto, le recomendamos que vea el evento del seminario web grabado [Pregunte al experto - Introducción a los informes en modo texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tiene una hora de duración.
>* Para obtener más información acerca del modo de texto, le recomendamos que vea la [Informes avanzados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriales, que en conjunto tienen una duración de cinco horas y media.


En este vídeo, aprenderá lo siguiente:

* Qué modo de texto es
* Qué es Camel Case
* Algunos modos de texto básicos &quot;plug and play&quot; que puede utilizar en sus agrupaciones

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12)

## Tarea: agrupación de 4 elementos principales

El siguiente modo de texto agrupará las tareas en función de hasta cuatro niveles de elementos primarios y dejará en blanco los elementos primarios que no existan.

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![Imagen de pantalla que muestra las tareas del proyecto agrupadas por 4 elementos principales](assets/4-parents-grouping.png)


## Tarea - Agrupación de porcentaje completado

El siguiente modo de texto agrupará las tareas en función del porcentaje completado. Las tareas caerán en una de las siguientes categorías cuando se agrupen:

* 0%
* Del 1% al 25%
* Del 26% al 50%
* Del 51% al 75%
* del 76 % al 99 %
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![Imagen de pantalla que muestra las tareas del proyecto agrupadas por porcentaje completado](assets/percent-complete-grouping.png)

## Tarea: statusEquatesWith y luego status

El siguiente modo de texto agrupará las tareas por statusEquatesWith y luego por status.

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

![Imagen de pantalla que muestra las tareas del proyecto agrupadas por statusEquatesWith](assets/status-equates-with.png)


## Aprobación de revisión - Agrupar por nombre de proyecto

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![Imagen de pantalla que muestra las aprobaciones de prueba agrupadas por nombre de proyecto](assets/proof-approvals-grouped-by-project-name.png)

