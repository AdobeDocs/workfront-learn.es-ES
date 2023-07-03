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
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 100%

---

# Comprender las ejecuciones incompletas

Las ejecuciones incompletas se pueden almacenar en Workfront Fusion, donde posteriormente se pueden revisar y resolver. Información sobre cómo aprovechar esta increíble función.

Este vídeo contiene información sobre:

* Qué son las ejecuciones incompletas
* Cómo gestionar un error que resulta en una ejecución incompleta

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on)

## Errores que dan lugar a ejecuciones incompletas

Existen varias categorías de errores que surgen del almacenamiento de ejecuciones incompletas.

Los distintos tipos de error recibidos dependerán de las API a las que se conecte. El error podría ser uno de validación derivado de datos incompletos o erróneos, principalmente debido a la falta de un elemento que se espera para procesar correctamente todos los datos que pasan por un módulo. O los errores podrían producirse a partir de la falta de disponibilidad del destino final debido a un error de conexión temporal o a largo plazo (por ejemplo, durante la conexión con un correo electrónico o un servidor FTP remoto).

Si se produce un error en el primer módulo del escenario, la ejecución se detiene inmediatamente y no se almacena ninguna ejecución incompleta.

Si se produce un error en cualquier otro módulo y no hay ninguna ruta de controlador de error adjunta, entonces puede ocurrir lo siguiente:

* Si el tipo de error es ConnectionError, RateLimitError, OutOfSpaceError o ModuleTimeoutError, se almacena un registro de ejecución incompleto CON reintento automático.
* Si el tipo de error es DataError, InvalidConfigurationError, InvalidAccessTokenError, UnestimatedError, MaxFileSizeExcededError o MaxResultsExcededError, se almacena un registro de ejecución incompleto SIN reintento automático.
* Si el tipo de error es cualquier cosa que no sea lo anterior, la ejecución falla.

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=es)
