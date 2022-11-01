---
title: Comprender el modo de texto básico de los filtros
description: Aprenda qué es el modo de texto, qué es el caso del camello y algún modo de texto básico de "Plug and Play" que puede utilizar en los filtros de informe en [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 59ac9907b116f8abadf5e15f8de351c02a7a2909
workflow-type: tm+mt
source-wordcount: '356'
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


En este vídeo, aprenderá:

* Qué modo de texto es
* Qué caso de camello es
* Algunos modos de texto &quot;Plug and Play&quot; básicos que se pueden usar en los filtros de informe

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

El siguiente modo de texto excluirá las tareas en las que el usuario ha marcado &quot;Listo con mi parte&quot;. Todo lo que tiene que hacer es crear un filtro de tareas, agregar cualquier regla de filtro que desee, luego cambiar al modo de texto y pegar el código siguiente después de cualquier modo de texto que vea en el filtro.

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## Filtros adicionales del modo Plug and Play de texto

### Tarea: Mostrar todas las tareas que esperan mi aprobación

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### Tarea: Mostrar todas las tareas que he aprobado

Cree un informe de tarea con los filtros que desee, vaya a la ficha Filtro y haga clic en Cambiar al modo Texto. Agregue este código a lo que ya esté allí:

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

### Tarea: Mostrar todas las tareas que asigné a otras

Cree un informe de tarea con los filtros que desee, vaya a la ficha Filtro y haga clic en Cambiar al modo Texto. Agregue este código a lo que ya esté allí:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Esto le mostrará todas las tareas en las que el usuario que ha iniciado sesión asignó al menos a uno de los usuarios asignados actualmente. Si varias personas asignaron a los usuarios, solo el nombre de la primera persona que asignó a alguien aparecerá como &quot;Solicitado por&quot; en la página de aterrizaje de la tarea.

## Actividad: Preguntas sobre el modo de texto

1. ¿Cómo escribiría el caso de camello para el campo titulado &quot;Introducido por ID&quot;?
1. En un informe de problemas, cree un filtro para mostrar los problemas que se han marcado como cerrados pero que están pendientes de aprobación.

### Respuestas

1. El caso de camello para el campo &quot;Introducido por ID&quot; debe escribirse de esta manera: enteredByID
1. El modo de texto debería tener este aspecto en el filtro de informe de problemas:

   ![Imagen de la pantalla para crear un nuevo filtro en el modo de texto](assets/btm-answer.png)
