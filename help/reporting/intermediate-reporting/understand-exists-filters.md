---
title: Crear filtros EXISTENTES para informes complejos
description: Descubra qué es un filtro EXISTS, para qué sirve y cómo puede crear uno desde cero. Además, vea muchos ejemplos útiles de filtros EXISTS.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
exl-id: f518a919-0c44-4122-873a-e2f10e3162d5
source-git-commit: 66bab1a0b2316a31cb99916220500303e49797ad
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 4%

---

# Crear filtros EXISTENTES para informes complejos

Los filtros EXISTS son filtros avanzados de modo de texto, que nos permiten solucionar la limitación de 2 saltos de tabla/campo en un Report Builder estándar. O bien, se pueden utilizar para identificar objetos en el sistema que carecen de una condición de relación específica mediante NOTEXISTS.

En este vídeo aprenderá a crear un filtro EXISTE para ver &quot;Aprobaciones de pruebas en proyectos actuales&quot; en un informe de aprobaciones de pruebas.

Para obtener un tutorial más detallado sobre el funcionamiento de EXISTS, consulte la documentación de [Creación de filtros de modo de texto complejos con instrucciones EXISTS](https://experienceleague.adobe.com/en/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements).

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops=1)

## Ejemplos de filtros EXISTS

### El informe del proyecto EXISTE

Esto utiliza la tarea como objeto de vinculación, comparando el ID de proyecto encontrado en el nivel de tarea y haciendo coincidir con el campo ID de nivel de proyecto. Esto nos permite comparar los usuarios de asignación de la tarea con un comodín $$USER.ID. Esto hace que se devuelvan solo los proyectos en los que el usuario que está viendo está asignado a una
tarea, independientemente de si es el principal asignado o no.

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


Utiliza el problema (optask) como objeto de vinculación, comparando también el ID de proyecto encontrado en el nivel de problema (optask) y haciendo coincidir ese ID con el campo ID de nivel de proyecto. A continuación, comprueba si alguno de estos problemas (optasks) tiene una fecha de entrada dentro del intervalo especificado. En este caso, devolverá cualquier proyecto que tenga
No se ha registrado un problema (optask) en los últimos 30 días, debido a NOTEXISTS.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### El informe de plantilla EXISTE

Este filtro mostrará todas las plantillas que no se hayan utilizado para crear un proyecto o que se hayan adjuntado a un proyecto en el último año. Una advertencia es que, para averiguar si una plantilla se utilizó o no como datos adjuntos, depende de que esa plantilla tenga tareas en ella.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### El informe de tareas EXISTE

Utiliza la tabla Usuario como objeto de vinculación, conectándose mediante el identificador de tarea de asignaciones y el identificador de tarea. A continuación, se comprueba la recopilación de ID de equipos de con los ID de equipo del usuario, devolviendo la tarea si alguno de los usuarios asignados está en el mismo equipo que el usuario que la visualiza.

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### El informe del usuario EXISTE

Esto devolverá todos los usuarios que no hayan publicado una actualización en las últimas 3 semanas. Utiliza el objeto de nota para reducir la brecha y compara el ownerID con un ID de usuario. A continuación, devuelve ese usuario si ninguna nota de su propiedad tiene una fecha de entrada mayor que 3 semanas atrás.

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

Esto devolverá todos los usuarios que no hayan registrado horas en la última semana. Utiliza un método extremadamente similar al ejemplo anterior, pero en su lugar utiliza la información del propietario de la hora y la fecha de entrada de hora para basar en qué usuarios devuelve.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

En un informe de usuario, muestre una lista de usuarios que coincida con la ficha Personas de un proyecto.

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### El informe de categoría (formulario personalizado) EXISTE

Este texto le ofrece una lista de todos los formularios de proyecto que no se han utilizado en ningún proyecto en absoluto. Esto debe usarse junto con la especificación del tipo de objeto del formulario en el que nos centramos. En este caso, el enfoque es PROJ, por lo que debemos incluir los rótulos en las líneas de objTypes. Esto podría usarse
para otros tipos de objeto cambiando las partes relacionadas con el código de objeto. Esto comprueba la colección de proyectos de formularios adjuntos, a los formularios enumerados y devuelve si no hay ninguna coincidencia.

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### El informe de parámetros (campo personalizado) EXISTE

Devuelve cualquier campo personalizado que no esté adjunto actualmente a un formulario personalizado en el sistema.

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### El informe EXISTE

Esto devolverá cualquier informe que utilice un valor específico en sus filtros.

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

Esto devolverá cualquier informe que esté adjunto a cualquier tablero.

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### El informe de aprobación de pruebas EXISTE

Esto devolverá las aprobaciones de prueba solo en los proyectos con el estado Actual. Esto utiliza el objeto Document para reducir el espacio entre la aprobación de pruebas y el proyecto comprobando currentVersionID y documentVersionID. De ahí saltamos al estado de los proyectos.

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
