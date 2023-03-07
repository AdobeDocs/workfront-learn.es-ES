---
title: Comprender el modo de texto básico de los filtros
description: Aprenda qué es el modo de texto, qué es camel case y algunos modos de texto básicos "plug and play" que puede utilizar en los filtros de informes en Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Comprender el modo de texto básico de los filtros

>[!IMPORTANT]
>
>Requisitos previos:
>
>* Comprender los elementos de informes
>* Comprender los componentes de informes
>* Creación de un filtro básico


>[!TIP]
>
>* Para comprender mejor el modo de texto, le recomendamos que vea el evento del seminario web grabado [Pregunte al experto - Introducción a los informes en modo texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tiene una hora de duración.
>* Para obtener más información acerca del modo de texto, le recomendamos que vea la [Informes avanzados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriales, que en conjunto tienen una duración de cinco horas y media.



En este vídeo, aprenderá lo siguiente:

* Qué modo de texto es
* Qué es Camel Case
* Algunos modos de texto básicos &quot;Plug and Play&quot; que puede utilizar en los filtros de informes

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)


## Tarea: filtre las tareas en las que haya marcado &quot;Listo con mi parte&quot;

El siguiente modo de texto excluirá las tareas en las que un usuario haya marcado &quot;Listo con mi parte&quot;. Todo lo que tiene que hacer es crear un filtro de tareas, agregar las reglas de filtro que desee, luego cambiar al modo de texto y pegar el código siguiente después de cualquier modo de texto que vea en el filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Tarea: mostrarme todas las tareas pendientes de aprobación

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## Tarea - Mostrarme todas las tareas que he aprobado

Cree un informe de tareas con los filtros que desee, vaya a la pestaña Filtro y haga clic en Cambiar a modo de texto. Agregue este código a lo que ya esté allí:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## Tarea: mostrarme todas las tareas que tienen al menos una predecesora entre proyectos

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## Tarea - Mostrarme todas las tareas que he asignado a otras personas

Cree un informe de tareas con los filtros que desee, vaya a la pestaña Filtro y haga clic en Cambiar a modo de texto. Agregue este código a lo que ya esté allí:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Esto le mostrará todas las tareas en las que el usuario que ha iniciado sesión ha asignado al menos a uno de los usuarios asignados actualmente. Si varias personas han asignado a las personas, solo el nombre de la primera persona que asignó a alguien aparecerá como &quot;Solicitado por&quot; en la página de aterrizaje de la tarea.

## Tarea - Mostrar todas las tareas completadas - Aprobación pendiente

```
status=CPL:A
status_Mod=in
```


## Problema - Mostrar todos los problemas completados - Aprobación pendiente

```
status=CPL:A
status_Mod=in
```


## Proyecto - Mostrar todos los proyectos completados - Aprobación pendiente

```
status=CPL:A
status_Mod=in
```


## Nota: muéstreme todos los comentarios en los que esté etiquetado

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Informe de parámetros/campos personalizados: mostrarme campos personalizados que no están adjuntos a un formulario personalizado (muy útiles en las tareas de limpieza)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
