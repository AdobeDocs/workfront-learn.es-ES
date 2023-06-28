---
title: Tutorial de almacenes de datos
description: Aprenda a utilizar un almacén de datos para sincronizar los nombres de empresa entre una lista de empresas y Workfront mediante [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# Tutorial de almacenes de datos

En este ejercicio utilizamos un almacén de datos para sincronizar nombres de compañías entre una lista de compañías y Workfront.

Esto forma parte de una sincronización unidireccional de compañías en Workfront y otros sistemas. Por ahora, solo se sincronizará entre un archivo CSV y Workfront. Pero también mantendrá una tabla en un almacén de datos que hará un seguimiento del Workfront ID (WFID) y del ID de empresa en el archivo CSV (CID) de cada empresa. Esto nos permitirá hacer de esto una sincronización bidireccional en algún momento futuro.

![Imagen de un escenario de Fusion](assets/data-structures-and-data-stores-2.png)

## Tutorial de almacenes de datos

Workfront recomienda ver el vídeo del tutorial de ejercicios antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on)

>[!TIP]
>
>Para obtener instrucciones paso a paso sobre cómo completar el tutorial, vaya a la [Tutorial de almacenes de datos](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) hacer ejercicio.


## Nota final

Ahora que ha terminado de aprender acerca de las estructuras y los almacenes de datos, es posible que se esté preguntando: &quot;¿Cuándo debe utilizarlos?&quot;

Las estructuras de datos se utilizan principalmente para serializar o analizar formatos de datos como JSON, XML, CSV y otros. Las estructuras de datos permiten controlar la estructura de los datos e incluso validar los datos. La razón más común por la que utiliza una estructura de datos es para crear datos válidos para enviarlos a una API que espere JSON o XML. En estos casos, querrá utilizar la aplicación JSON o la aplicación XML junto con la estructura de datos para asegurarse de que los datos tengan el formato correcto.

Los almacenes de datos solo deben usarse para almacenar datos persistentes a los que sea necesario acceder mediante más de una ejecución de escenario. Por ejemplo, puede almacenar metadatos sobre el último registro procesado para casos de uso avanzados que requieran un control preciso sobre el procesamiento.

Los almacenes de datos no están diseñados para utilizarse como almacén de datos o registro. No se puede acceder a los almacenes de datos fuera de Workfront Fusion y la mayoría de las interacciones con los almacenes de datos se realizan a través de un escenario de Workfront Fusion. Por lo tanto, no es posible conectar un almacén de datos a una herramienta de análisis o informes que se esperaría para los casos de uso de Data Warehouse y del registro. La función de Workfront Fusion en casos de uso como estos sería rellenar un sistema adecuado para organizar y almacenar datos (por ejemplo, SQL, MariaDB).

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
