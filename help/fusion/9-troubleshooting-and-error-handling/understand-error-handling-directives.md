---
title: Comprender las directivas de la gestión de errores
description: Obtenga información sobre las directivas del controlador de error que permiten que la ejecución continúe y las que detienen la ejecución, en  [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 100%

---

# Comprender las directivas de la gestión de errores

Este vídeo contiene información sobre:

* Las tres directivas del controlador de error que permiten que la ejecución continúe
* Las dos directivas del controlador de error que detienen la ejecución

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on&enablevpops)

## Directivas: el escenario continúa

### Reanudar

* Se especifica una salida sustitutiva que se suministra al módulo que encuentra un error.
* Los módulos posteriores se procesan.
* El estado de ejecución del escenario se marca como “éxito”.

![Una imagen de una directiva de reanudación](assets/troubleshooting-and-error-handling-2.png)

### Salto

* El estado de la ejecución del escenario se almacena en la cola de ejecuciones incompletas, donde el error se puede resolver manualmente. Sin embargo, hay algunas excepciones que se mencionan aquí.
* Los módulos siguientes no se procesan.
* Si hay paquetes sin procesar, la ejecución del escenario continúa normalmente.
* El estado de ejecución del escenario se marca como “advertencia”.

![Una imagen de una directiva de Salto](assets/troubleshooting-and-error-handling-3.png)

### Ignorar

* El error se ignora y los módulos posteriores no se procesan.
* Si hay paquetes sin procesar, la ejecución del escenario continúa con normalidad.
* El estado de ejecución del escenario se marca como “éxito”.

![Una imagen de una directiva Ignorar](assets/troubleshooting-and-error-handling-4.png)

## Directivas: paradas de escenario

### Reversión

* La ejecución del escenario se detiene inmediatamente y se inicia una fase de reversión en todos los módulos en un intento de revertirlos a su estado inicial.
* Los módulos siguientes no se procesan.
* A excepción de algunos tipos de error, el escenario se desactiva después del “número de errores consecutivos” especificado en Configuración del escenario.
* El estado de ejecución del escenario está marcado como “error”.

>[!NOTE]
>
>Este es el comportamiento predeterminado si no hay ninguna ruta de controlador de error adjunta al módulo y el ajuste “Permitir almacenamiento de ejecuciones incompletas” en la configuración de escenario no está seleccionado.

![Una imagen de una directiva de Reversión](assets/troubleshooting-and-error-handling-5.png)

### Confirmar

* El error se ignora y los módulos posteriores no se procesan.
* Si hay paquetes sin procesar, la ejecución del escenario continúa con normalidad.
* El estado de ejecución del escenario se marca como “éxito”.

![Imagen de una directiva de Compromiso](assets/troubleshooting-and-error-handling-6.png)
