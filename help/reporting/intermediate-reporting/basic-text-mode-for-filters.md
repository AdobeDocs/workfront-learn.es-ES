---
title: Comprender el modo de texto básico de los filtros
description: Obtenga información sobre el modo de texto, camel case y algunos modos de texto básicos que puede utilizar en los filtros de informes en Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-07-30T00:00:00Z
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 88%

---

# Comprender el modo de texto básico de los filtros

>[!PREREQUISITES]
>
>* [Comprensión de los elementos de creación de informes](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-task-report.html?lang=es)
>* [Información sobre los componentes del sistema de informes](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=es)
>* [Crear un filtro básico](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=es)


>[!TIP]
>
>* Para comprender mejor el modo de texto, le recomendamos que consulte el evento de seminario web grabado [Pregunte al experto: introducción a la creación de informes en modo de texto](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), que dura una hora.
>* Para obtener más información acerca del modo de texto, le recomendamos que consulte los tutoriales de [Creación de informes avanzada](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=es), que tienen una duración de cinco horas y media en total.
>* Haga clic aquí para acceder al [[!UICONTROL Explorador de la API]](https://developer.adobe.com/workfront/api-explorer/)


En este vídeo, aprenderá sobre lo siguiente:

* Modo de texto
* Mayúsculas y minúsculas
* Algunos _bloques de código en modo texto_ que puede usar en los filtros de informe

>[!VIDEO](https://video.tv.adobe.com/v/3412683/?captions=spa&quality=12&learn=on&enablevpops=0)

## Actividades de &quot;Comprender el modo de texto básico de los filtros&quot;


### Tarea: filtre las tareas en las que he marcado “Listo con mi parte”

El siguiente modo de texto excluirá las tareas en las que el usuario ha marcado “Listo con mi parte”. Todo lo que tiene que hacer es crear un filtro de tareas, agregar cualquier regla de filtro que desee, luego cambiar al modo de texto y pegar el código siguiente después de cualquier modo de texto que vea en el filtro.


>[!WARNING]
>
> Esto no está pensado para su uso en filtros de calendario.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

### Tarea: Mostrar todas las tareas que esperan mi aprobación

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Tarea: Mostrar todas las tareas que he aprobado

Cree un informe de tarea con los filtros que desee, vaya a la pestaña Filtro y haga clic en Cambiar al modo Texto. Agregue este código a lo que ya esté allí:

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### Tarea: Muéstreme todas las tareas que tengan al menos un predecesor entre proyectos

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Tarea: Mostrar todas las tareas que asigné a otros

Cree un informe de tarea con los filtros que desee, vaya a la pestaña Filtro y haga clic en Cambiar al modo Texto. Agregue este código a lo que ya esté allí:

>[!WARNING]
> 
> Esto no está pensado para su uso en filtros de calendario.

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Esto le mostrará todas las tareas en las que el usuario que ha iniciado sesión asignó al menos a uno de los usuarios asignados actualmente. Si varias personas asignaron a los usuarios, solo el nombre de la primera persona que asignó a alguien aparecerá como “Solicitado por” en la página de destino de la tarea.

### Tarea: mostrar todas las tareas completadas, pendiente de aprobación

```
status=CPL:A
status_Mod=in
```


### Problema: Mostrar todos los problemas completados y pendientes de aprobación

```
status=CPL:A
status_Mod=in
```


### Proyecto: Mostrar todos los proyectos completados y pendientes de aprobación

```
status=CPL:A
status_Mod=in
```


### Nota: Mostrar todos los comentarios en los que estoy etiquetado

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### Informe de parámetros/campo personalizado: muestra los campos personalizados que no están adjuntos a un formulario personalizado (muy útil en los trabajos de limpieza)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
