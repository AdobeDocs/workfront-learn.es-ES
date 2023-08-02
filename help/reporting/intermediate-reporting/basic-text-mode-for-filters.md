---
title: Comprender el modo de texto básico de los filtros
description: Aprenda qué es el modo de texto, qué son las palabras agrupadas en mayúsculas y minúsculas y algún modo de texto básico de “plug and play” que puede utilizar en los filtros de informe en Workfront.
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: ht
source-wordcount: '416'
ht-degree: 100%

---

# Comprender el modo de texto básico de los filtros

>[!IMPORTANT]
>
>Requisitos previos:
>
>* Comprensión de los elementos de creación de informes
>* Información sobre los componentes del sistema de informes
>* Creación de un filtro básico

>[!TIP]
>
>* Para comprender mejor el modo de texto, le recomendamos que consulte el evento de seminario web grabado [Pregunte al experto: introducción a la creación de informes en modo de texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=es), que dura una hora.
>* Para obtener más información acerca del modo de texto, le recomendamos que consulte los tutoriales de [Creación de informes avanzada](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=es), que tienen una duración de cinco horas y media en total.


Este vídeo contiene información sobre:

* Qué es el modo de texto
* Qué son las palabras agrupadas en mayúsculas y minúsculas
* Algunos modos de texto &quot;plug and play&quot; básicos que se pueden usar en los filtros de informe

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## Tarea: filtre las tareas en las que he marcado “Listo con mi parte”

El siguiente modo de texto excluirá las tareas en las que el usuario ha marcado “Listo con mi parte”. Todo lo que tiene que hacer es crear un filtro de tareas, agregar cualquier regla de filtro que desee, luego cambiar al modo de texto y pegar el código siguiente después de cualquier modo de texto que vea en el filtro.

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

Cree un informe de tarea con los filtros que desee, vaya a la pestaña Filtro y haga clic en Cambiar al modo Texto. Agregue este código a lo que ya esté allí:

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

## Tarea: Mostrar todas las tareas que asigné a otros

Cree un informe de tarea con los filtros que desee, vaya a la pestaña Filtro y haga clic en Cambiar al modo Texto. Agregue este código a lo que ya esté allí:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Esto le mostrará todas las tareas en las que el usuario que ha iniciado sesión asignó al menos a uno de los usuarios asignados actualmente. Si varias personas asignaron a los usuarios, solo el nombre de la primera persona que asignó a alguien aparecerá como “Solicitado por” en la página de aterrizaje de la tarea.

## Tarea: mostrar todas las tareas completadas, pendiente de aprobación

```
status=CPL:A
status_Mod=in
```


## Problema: Mostrar todos los problemas completados y pendientes de aprobación

```
status=CPL:A
status_Mod=in
```


## Proyecto: Mostrar todos los proyectos completados y pendientes de aprobación

```
status=CPL:A
status_Mod=in
```


## Nota: Mostrar todos los comentarios en los que estoy etiquetado

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## Informe de parámetros/campo personalizado: muestra los campos personalizados que no están adjuntos a un formulario personalizado (muy útil en los trabajos de limpieza)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
