---
title: Comprender el modo de texto básico de los filtros
description: Aprenda qué es el modo de texto, qué es el caso del camello y algún modo de texto básico de "Plug and Play" que puede utilizar en los filtros de informe en Workfront.
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
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Comprender el modo de texto básico de los filtros

>[!IMPORTANT]
>
>Requisitos previos:
>
>* Explicación de los elementos de informes
>* Comprender los componentes del sistema de informes
>* Crear un filtro básico


>[!TIP]
>
>* Para comprender mejor el modo de texto, le recomendamos que consulte el evento de seminario web grabado [Pregunte al experto: Introducción a los informes de modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tiene una hora de longitud.
>* Para obtener más información sobre el modo de texto, le recomendamos que consulte [Informes avanzados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriales, que juntos tienen una duración de cinco horas y media.



En este vídeo, aprenderá:

* Qué modo de texto es
* Qué caso de camello es
* Algunos modos de texto &quot;Plug and Play&quot; básicos que se pueden usar en los filtros de informe

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## Tarea: filtre las tareas en las que he marcado &quot;Listo con mi parte&quot;

El siguiente modo de texto excluirá las tareas en las que el usuario ha marcado &quot;Listo con mi parte&quot;. Todo lo que tiene que hacer es crear un filtro de tareas, agregar cualquier regla de filtro que desee, luego cambiar al modo de texto y pegar el código siguiente después de cualquier modo de texto que vea en el filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Tarea: Mostrar todas las tareas que esperan mi aprobación

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## Tarea: Mostrar todas las tareas que he aprobado

Cree un informe de tarea con los filtros que desee, vaya a la ficha Filtro y haga clic en Cambiar al modo Texto. Agregue este código a lo que ya esté allí:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## Tarea: Muéstreme todas las tareas que tengan al menos un predecesor entre proyectos

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## Tarea: Mostrar todas las tareas que asigné a otras

Cree un informe de tarea con los filtros que desee, vaya a la ficha Filtro y haga clic en Cambiar al modo Texto. Agregue este código a lo que ya esté allí:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Esto le mostrará todas las tareas en las que el usuario que ha iniciado sesión asignó al menos a uno de los usuarios asignados actualmente. Si varias personas asignaron a los usuarios, solo el nombre de la primera persona que asignó a alguien aparecerá como &quot;Solicitado por&quot; en la página de aterrizaje de la tarea.

## Tarea - Mostrar todas las tareas completadas - Pendiente de aprobación

```
status=CPL:A
status_Mod=in
```


## Problema: Muéstrame todos los problemas completados - Pendiente de aprobación

```
status=CPL:A
status_Mod=in
```


## Proyecto: Mostrar todos los proyectos completados - Pendiente de aprobación

```
status=CPL:A
status_Mod=in
```


## Nota: Muéstrame todos los comentarios en los que estoy etiquetado

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Parámetro/Informe de campo personalizado : muestra los campos personalizados que no están adjuntos a un formulario personalizado (muy útil en los esfuerzos de limpieza)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
