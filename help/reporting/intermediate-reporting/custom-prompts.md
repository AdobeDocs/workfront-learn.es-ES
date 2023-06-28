---
title: Creación de mensajes personalizados
description: Descubra qué es una solicitud personalizada, cómo crear una solicitud personalizada mediante el modo de texto y algunos ejemplos que puede utilizar en la creación de informes en Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 2%

---

# Creación de mensajes personalizados

En este vídeo, aprenderá lo siguiente:

* Qué es un mensaje personalizado
* Cómo crear una solicitud personalizada mediante el modo de texto
* Algunos ejemplos que puede utilizar en los informes

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## Actividad: Crear indicadores personalizados

1. Cree una solicitud personalizada que muestre los siguientes estados de proyecto en el menú desplegable de solicitudes:
   * Planificación
   * Al día
   * Finalizado
   * Inactivo
1. Modifique la solicitud para mostrar los proyectos actuales con vencimiento para este mes.

## Respuestas

1. Los mensajes personalizados deben tener un aspecto similar a este y tener el siguiente modo de texto:

   ![Imagen de la pantalla para crear un nuevo filtro en modo de texto](assets/cp-01.png)

   Una vez guardado el mensaje personalizado, el menú desplegable del mensaje debería tener este aspecto:

1. El modo de texto del mensaje personalizado debería tener este aspecto:

![Imagen de la pantalla para crear un nuevo filtro en modo de texto](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

Y la etiqueta desplegable de las peticiones de datos activas debe actualizarse para reflejar el cambio en el código de esta manera:

![Imagen de la pantalla para crear un nuevo filtro en modo de texto](assets/cp-02a.png)
