---
title: Comprender las ejecuciones incompletas
description: Descubra cuáles son las ejecuciones incompletas y cómo gestionar un error que da lugar a una ejecución incompleta en  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
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
autotag-review: '2026-05-06T16:07:51.152Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 100%

---

# Comprender las ejecuciones incompletas

Las ejecuciones incompletas se pueden almacenar en Workfront Fusion, donde posteriormente se pueden revisar y resolver. Información sobre cómo aprovechar esta increíble función.

Este vídeo contiene información sobre:

* Qué son las ejecuciones incompletas
* Cómo gestionar un error que resulta en una ejecución incompleta

>[!VIDEO](https://video.tv.adobe.com/v/3418147/?captions=spa&quality=12&learn=on&enablevpops=1)

## Errores que dan lugar a ejecuciones incompletas

Existen varias categorías de errores que surgen del almacenamiento de ejecuciones incompletas.

Los distintos tipos de error recibidos dependerán de las API a las que se conecte. El error podría ser uno de validación derivado de datos incompletos o erróneos, principalmente debido a la falta de un elemento que se espera para procesar correctamente todos los datos que pasan por un módulo. O los errores podrían producirse a partir de la falta de disponibilidad del destino final debido a un error de conexión temporal o a largo plazo (por ejemplo, durante la conexión con un correo electrónico o un servidor FTP remoto).

Si se produce un error en el primer módulo del escenario, la ejecución se detiene inmediatamente y no se almacena ninguna ejecución incompleta.

Si se produce un error en cualquier otro módulo y no hay ninguna ruta de controlador de error adjunta, entonces puede ocurrir lo siguiente:

* Si el tipo de error es ConnectionError, RateLimitError, OutOfSpaceError o ModuleTimeoutError, se almacena un registro de ejecución incompleto CON reintento automático.
* Si el tipo de error es DataError, InvalidConfigurationError, InvalidAccessTokenError, UnestimatedError, MaxFileSizeExcededError o MaxResultsExcededError, se almacena un registro de ejecución incompleto SIN reintento automático.
* Si el tipo de error es cualquier cosa que no sea lo anterior, la ejecución falla.

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
