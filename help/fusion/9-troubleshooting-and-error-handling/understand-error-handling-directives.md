---
title: Comprender las directivas de gestión de errores
description: Obtenga información acerca de las directivas del controlador de errores que permiten que continúe la ejecución y las que detienen la ejecución, en [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Comprender las directivas de gestión de errores

En este vídeo, aprenderá lo siguiente:

* Las tres directivas de tratamiento de errores que permiten que continúe la ejecución
* Las dos directivas de controlador de errores que detienen la ejecución

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12)

## Directivas: el escenario continúa

### Reanudar

* Se especifica una salida de sustitución y se suministra al módulo que encuentra un error.
* Se procesan los módulos siguientes.
* El estado de ejecución del escenario se marca como &quot;correcto&quot;.

![Imagen de una directiva Resume](assets/troubleshooting-and-error-handling-2.png)

### Descanso

* El estado de la ejecución del escenario se almacena en la cola de ejecuciones incompletas, donde el error se puede resolver manualmente. Sin embargo, hay algunas excepciones que se mencionan aquí.
* Los módulos siguientes no se procesan.
* Si hay paquetes sin procesar, la ejecución del escenario continúa de forma normal.
* El estado de ejecución del escenario se marca como &quot;advertencia&quot;.

![Imagen de una directiva Break](assets/troubleshooting-and-error-handling-3.png)

### Ignorar

* El error se ignora y los módulos posteriores no se procesan.
* Si hay paquetes sin procesar, la ejecución del escenario continúa de forma normal.
* El estado de ejecución del escenario se marca como &quot;correcto&quot;.

![Imagen de una directiva Ignore](assets/troubleshooting-and-error-handling-4.png)

## Directivas: paradas de escenario

### Reversión

* La ejecución de escenarios se detiene inmediatamente y se inicia una fase de reversión en todos los módulos para intentar revertirlos todos a su estado inicial.
* Los módulos siguientes no se procesan.
* Salvo algunos tipos de error, el escenario se desactiva después del &quot;número de errores consecutivos&quot; especificado en Configuración del escenario.
* El estado de ejecución del escenario se marca como &quot;error&quot;.

>[!NOTE]
>
>Este es el comportamiento predeterminado si no hay ninguna ruta de controlador de error adjunta al módulo y la opción &quot;Permitir el almacenamiento de ejecuciones incompletas&quot; en Configuración de escenario no está activada.

![Imagen de una directiva Rollback](assets/troubleshooting-and-error-handling-5.png)

### Confirmar

* El error se ignora y los módulos posteriores no se procesan.
* Si hay paquetes sin procesar, la ejecución del escenario continúa de forma normal.
* El estado de ejecución del escenario se marca como &quot;correcto&quot;.

![Imagen de una directiva Commit](assets/troubleshooting-and-error-handling-6.png)
