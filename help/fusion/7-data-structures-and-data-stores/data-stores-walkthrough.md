---
title: Recorrido por las tiendas de datos
description: Aprenda a utilizar un almacén de datos para sincronizar nombres de empresas entre una lista de empresas y Workfront mediante [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Recorrido por las tiendas de datos

## Información general

En este ejercicio utilizamos un almacén de datos para sincronizar los nombres de las empresas entre una lista de empresas y Workfront.

Esto forma parte de una sincronización unidireccional de empresas en Workfront y en otros sistemas. Por ahora, solo se sincronizará entre un archivo CSV y Workfront. Sin embargo, también mantendrá una tabla en un almacén de datos que realizará un seguimiento del Workfront ID (WFID) y el ID de la empresa en el archivo CSV (CID) para cada empresa. Esto nos permitirá hacer de esto una sincronización bidireccional en algún momento en el futuro.

![Imagen de un escenario de fusión](assets/data-structures-and-data-stores-2.png)

## Recorrido por las tiendas de datos

Workfront recomienda ver el vídeo tutorial del ejercicio antes de intentar recrear el ejercicio en su propio entorno.

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>Para obtener instrucciones paso a paso sobre cómo completar el tutorial, vaya a la [Recorrido por las tiendas de datos](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) ejercicio.


## Nota final

Ahora que ha terminado de aprender sobre estructuras de datos y almacenes de datos, puede que se esté preguntando: &quot;¿Cuándo deben usarse?&quot;

Las estructuras de datos se utilizan habitualmente para serializar o analizar formatos de datos como JSON, XML, CSV y otros. Las estructuras de datos permiten controlar la estructura de los datos e incluso validar los datos. La razón más común por la que utiliza una estructura de datos es crear datos válidos para enviarlos a una API que espere JSON o XML. En estos casos, debe utilizar la aplicación JSON o XML junto con la estructura de datos para asegurarse de que los datos tengan el formato correcto.

Los almacenes de datos solo deben utilizarse para almacenar datos persistentes a los que es necesario acceder mediante más de una ejecución de escenario. Por ejemplo, puede almacenar metadatos sobre el último registro procesado para casos de uso avanzados que requieran un control preciso sobre el procesamiento.

Los almacenes de datos no están diseñados para utilizarse como almacén de datos o registro. No se puede acceder a los almacenes de datos fuera de Workfront Fusion y la mayoría de las interacciones con almacenes de datos se realizan a través de un escenario de Workfront Fusion. Por lo tanto, no es posible conectar un almacén de datos a una herramienta de análisis o de informes que se esperaría para casos de uso de registro y almacén de datos. La función de Workfront Fusion en casos de uso como estos sería rellenar un sistema apropiado para organizar y almacenar datos (por ejemplo, SQL, MariaDB).

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
