---
title: Comprender las ejecuciones incompletas
description: Descubra cuáles son las ejecuciones incompletas y cómo gestionar un error que resulta en una ejecución incompleta en [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Comprender las ejecuciones incompletas

Las ejecuciones incompletas se pueden almacenar en Workfront Fusion, donde posteriormente se pueden revisar y resolver. Aprenda a aprovechar esta increíble función.

En este vídeo, aprenderá:

* ¿Qué ejecuciones incompletas son
* Cómo gestionar un error que resulta en una ejecución incompleta

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on)

## Errores que resultan en ejecuciones incompletas

Existen varias categorías de errores que resultan en el almacenamiento de ejecuciones incompletas.

Los distintos tipos de error recibidos dependerán de las API a las que se conecte. El error podría ser un error de validación derivado de datos incompletos o erróneos, principalmente debido a la falta de un elemento que se espera para procesar correctamente todos los datos que pasan por un módulo. O los errores podrían producirse a partir de la falta de disponibilidad del destino final debido a un error de conexión temporal o a largo plazo (por ejemplo, durante la conexión con un correo electrónico o un servidor FTP remoto).

Si se produce un error en el primer módulo del escenario, la ejecución se detiene inmediatamente y no se almacena ninguna ejecución incompleta.

Si se produce un error en cualquier otro módulo y no hay ninguna ruta de controlador de error adjunta, entonces:

* Si el tipo de error es ConnectionError, RateLimitError, OutOfSpaceError o ModuleTimeoutError, se almacena un registro de ejecución incompleto CON reintento automático.
* Si el tipo de error es DataError, InvalidConfigurationError, InvalidAccessTokenError, UnestimatedError, MaxFileSizeExcededError o MaxResultsExcededError, se almacena un registro de ejecución incompleto SIN reintento automático.
* Si el tipo de error es cualquier cosa que no sea lo anterior, la ejecución falla.

## ¿Desea obtener más información? Recomendamos lo siguiente:

[Documentación de Workfront Fusion](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
