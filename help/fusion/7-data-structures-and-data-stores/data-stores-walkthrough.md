---
title: Tutorial de los almacenes de datos
description: Aprenda a utilizar un almacén de datos para sincronizar nombres de compañías entre una lista de compañías y de Workfront con  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
recommendations: noDisplay,catalog
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:18:10.872Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 411
ht-degree: 100%

---

# Tutorial de los almacenes de datos

En este ejercicio utilizamos un almacén de datos para sincronizar los nombres de las compañías entre una lista de compañías y de Workfront.

Esto forma parte de una sincronización unidireccional de compañías en Workfront y en otros sistemas. Por ahora, solo se sincronizará entre un archivo CSV y Workfront. Sin embargo, también mantendrá una tabla en un almacén de datos que realizará un seguimiento del ID de Workfront (WFID) y el ID de la compañía en el archivo CSV (CID) para cada compañía. Esto nos permitirá hacer de esto una sincronización bidireccional en algún momento en el futuro.

![Una imagen de un escenario de Fusion](assets/data-structures-and-data-stores-2.png)

## Tutorial de los almacenes de datos

Workfront recomienda ver el vídeo tutorial del ejercicio antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/3417968/?captions=spa&quality=12&learn=on&enablevpops=1)



## Nota final

Ahora que ha terminado de aprender sobre estructuras de datos y almacenes de datos, puede que se esté preguntando: “¿cuándo deben usarse?”

Las estructuras de datos se utilizan habitualmente para serializar o analizar formatos de datos como JSON, XML, CSV y otros. Las estructuras de datos permiten controlar la estructura de los datos e incluso validarlos. La razón más común por la que utiliza una estructura de datos es crear datos válidos para enviarlos a una API que espera una aplicación JSON o XML. En estos casos, debe utilizar la aplicación JSON o XML junto con la estructura de datos para asegurarse de que los datos tengan el formato correcto.

Los almacenes de datos solo deben utilizarse para almacenar datos persistentes a los que es necesario acceder mediante más de una ejecución de escenario. Por ejemplo, puede almacenar metadatos sobre el último registro procesado para casos de uso avanzados que requieran un control preciso sobre el procesamiento.

Los almacenes de datos no están diseñados para utilizarse como almacén de datos o registro. No se puede acceder a los almacenes de datos fuera de Workfront Fusion y la mayoría de las interacciones con almacenes de datos se realizan a través de un escenario de Workfront Fusion. Por lo tanto, no es posible conectar un almacén de datos a una herramienta de análisis o de creación de informes que se esperaría para casos de uso de registro y almacén de datos. La función de Workfront Fusion en casos de uso como estos sería rellenar un sistema apropiado para organizar y almacenar datos (por ejemplo, SQL, MariaDB).

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
