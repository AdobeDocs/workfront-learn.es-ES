---
title: Crear mensajes personalizados
description: Conozca qué es un mensaje personalizado, cómo crear un mensaje personalizado usando el modo de texto y algunos ejemplos que puede usar en los informes en Workfront.
activity: use
feature: Text Mode Reporting
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 100%

---

# Crear mensajes personalizados

Este vídeo contiene información sobre:

* Qué es un mensaje personalizado
* Cómo crear una solicitud personalizada mediante el modo de texto
* Algunos ejemplos que se pueden usar en los informes

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on&enablevpops)

## Actividad: Crear mensajes personalizados

1. Cree un mensaje personalizado que muestre los siguientes estados de proyecto en el menú desplegable de solicitudes:
   * Planificación
   * Al día
   * Finalizado
   * Inactivo
1. Modifique la solicitud para mostrar los proyectos actuales que vencen este mes.

## Respuestas

1. Las indicaciones personalizadas deben tener un aspecto similar al siguiente y el siguiente modo de texto:

   ![Imagen de la pantalla para crear un nuevo filtro en el modo de texto](assets/cp-01.png)

   Una vez guardado el mensaje personalizado, el menú desplegable del mensaje debería tener este aspecto:

1. El modo de texto en el mensaje personalizado debería tener este aspecto:

![Imagen de la pantalla para crear un nuevo filtro en el modo de texto](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

Y la etiqueta desplegable para las solicitudes activas debe actualizarse para reflejar el cambio en el código de esta manera:

![Imagen de la pantalla para crear un nuevo filtro en el modo de texto](assets/cp-02a.png)
