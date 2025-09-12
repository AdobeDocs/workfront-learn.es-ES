---
title: Comprender el modo de texto básico de las vistas
description: Obtenga información acerca del modo de texto, camel case y algunos modos de texto básicos que puede utilizar en las vistas Informes en Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-12T00:00:00Z
jira: KT-11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: 062a7f3576c4d5af02b04340e9763a82a9b8c721
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 93%

---

# Comprender el modo de texto básico de las vistas


>[!PREREQUISITES]
>
>* [Comprensión de los elementos de creación de informes](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-task-report.html?lang=es)
>* [Información sobre los componentes del sistema de informes](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=es)
>* [Crear una vista básica](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-view.html?lang=es)


>[!TIP]
>
>* Para comprender mejor el modo de texto, le recomendamos que consulte el evento de seminario web grabado [Pregunte al experto: introducción a la creación de informes en modo de texto](https://experienceleague.adobe.com/es/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting), que dura una hora.
>* Para obtener más información acerca del modo de texto, le recomendamos que consulte los tutoriales de [Creación de informes avanzada](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=es), que tienen una duración de cinco horas y media en total.
>* Haga clic aquí para acceder al [[!UICONTROL Explorador de la API]](https://developer.adobe.com/workfront/api-explorer/)

Este vídeo contiene información sobre:

* Qué es el modo de texto
* Qué son las palabras agrupadas en mayúsculas y minúsculas
* Algunos _bloques de código en modo texto_ que puede usar en sus vistas de informes

>[!VIDEO](https://video.tv.adobe.com/v/3470793/?quality=12&learn=on&captions=spa)

## Actividades de &quot;Comprender el modo de texto básico para vistas&quot;

### Tarea: Vista de los cuatro elementos principales

Cree primero una columna para el Nombre de la tarea y el Nombre principal y, a continuación, utilice el siguiente modo de texto para crear las otras tres columnas.

#### Tarea: elemento principal del nombre principal

```
displayname=Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:name
textmode=true
valuefield=parent:parent:name
valueformat=HTML
```

#### Tarea: principal del nombre principal

```
displayname=Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:name
valueformat=HTML
```

#### Tarea: elemento principal de la página principal del nombre principal

```
displayname=Parent of Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:parent:name
valueformat=HTML
```

![Una imagen de pantalla que muestra la vista de los cuatro elementos principales](assets/4-parents-view.png)

### Usuario: iteraciones que muestran listas en las vistas de usuario

#### Usuario: todas las funciones

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

#### Usuario: todas las funciones que muestran el rol principal

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

#### Usuario: todos los equipos

```
displayname=All teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

>[!NOTE]
>
>Se puede acceder al campo Equipo a través de la interfaz de usuario que muestra todos los equipos separados por coma, pero al usar el modo de texto anterior se mostrará a cada equipo en una línea independiente.


#### Usuario: todos los grupos

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

#### Usuario: todos los grupos que muestran el grupo principal

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


#### Usuario: informes directos

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

#### Usuario: futuro calendario de días libres personales

```
displayname=Future PTO
listdelimiter=<br>
listmethod=nested(reservedTimes).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),"")
valueformat=HTML
width=150
```

![Una imagen de pantalla que muestra la vista Listas de usuarios](assets/user-lists-view-large.png)

### Tarea: cómo mostrar las asignaciones de tareas y trabajar en el estado

```
displayname=Assignments and Status
listdelimiter=<br>
listmethod=nested(assignments).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT({assignedTo}.{name},IF(ISBLANK({assignedTo}.{name}),"",IF({status}="AA"," - Requested",IF({status}="AD"," - Working"," - Done"))))
valueformat=HTML
width=150
```

![Una imagen de pantalla que muestra la vista Asignaciones y Estado](assets/assignments-and-status-view.png)


### Tarea: cómo mostrar la función y la asignación en varias asignaciones de tareas

#### Tarea: función + horas

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

#### Tarea: asignación + asignación porcentual

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![Una imagen de pantalla que muestra la vista Asignaciones y funciones](assets/assignments-roles-and-percent-view.png)

### Tarea: predecesores y sucesores de varios proyectos

#### Filtro de tareas (opcional)

**Mostrar todas las tareas que tengan al menos una predecesora entre proyectos o al menos una sucesora entre proyectos en los proyectos actuales**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
project:statusEquatesWith=CUR
project:statusEquatesWith_Mod=in
OR:1:project:statusEquatesWith=CUR
OR:1:project:statusEquatesWith_Mod=in
OR:1:successorsMM:ID_Mod=notblank
OR:1:successorsMM:projectID=FIELD:projectID
OR:1:successorsMM:projectID_Mod=ne
```

#### Tarea: mostrar nombres de predecesor y predecesor de proyecto

```
displayname=Predecessor names
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{predecessor}.{name}," >> PROJECT = ",{predecessor}.{project}.{name})
valueformat=HTML
width=150
```

#### Tarea: mostrar nombres de sucesores y sucesores de proyectos

```
displayname=Successor names
listdelimiter=<br>
listmethod=nested(successors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{successor}.{name}," >> PROJECT = ",{successor}.{project}.{name})
valueformat=HTML
width=150
```

#### Tarea: mostrar la fecha de finalización prevista de los predecesores

```
displayname=Predecessor projected completion dates
valueformat=atDate
listdelimiter=
textmode=true
width=90
stretch=0
valuefield=predecessor:projectedCompletionDate
type=iterate
listmethod=nested(predecessors).lists
shortview=false
```

#### Tarea: mostrar el estado de progreso de los predecesores

```
displayname=Predecessor progress status
listdelimiter=<br>
listmethod=nested(predecessors).lists
shortview=false
stretch=0
textmode=true
type=iterate
valueexpression=IF({predecessor}.{progressStatus}="OT","On Time",IF({predecessor}.{progressStatus}="LT","Late",IF({predecessor}.{progressStatus}="BH","Behind","At Risk")))
valueformat=HTML
width=90
```

#### Tarea: mostrar el porcentaje completado del proyecto del predecesor de proyectos cruzados

```
displayname=Predecessor project percent complete
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({isCP}=true,CONCAT({predecessor}.{project}.{percentComplete},"%"),"")
valueformat=HTML
width=150
```

![Una imagen de pantalla que muestra la vista predecesores y sucesores de varios proyectos](assets/cross-project-predecessors-and-successors.png)


### Tarea: iteración que muestra todas las personas asignadas y quién asignó cada una

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![Una imagen de pantalla que muestra todas las personas asignadas y quién asignó cada una](assets/all-assignees-and-requesters.png)

### Tarea/proyecto: iteración que muestra todos los formularios personalizados de un proyecto o una tarea

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![Una imagen de pantalla que muestra todos los formularios personalizados de un proyecto](assets/all-custom-forms-on-a-project.png)


### Proyecto: iteración que muestra todos los contactos principales para las variables resueltas en la vista del proyecto

```
displayname=Requestor
listdelimiter=<br>
listmethod=nested(resolvables).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=owner:name
valueformat=HTML
width=150
```

![Una imagen de pantalla que muestra los contactos principales para las variables resolubles](assets/primary-contacts-for-resolvables.png)

### Proyecto: iteración que muestra todos los integrantes del equipo del proyecto

```
displayname=Project Team Members
listdelimiter=<br>
listmethod=nested(projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

![Una imagen de pantalla que muestra todos los integrantes del equipo del proyecto](assets/all-project-team-members.png)

### Proyecto: iteración que muestra la entryDate de todos los problemas que se pueden resolver de un proyecto

```
displayname=Resolvables entry date
linkedname=direct
listdelimiter=<br>
listmethod=nested(project.resolvables).lists
listsort=string(description)
querysort=description
section=0
textmode=true
type=iterate
valuefield=entryDate
valueformat=HTML
```

![Imagen de pantalla que muestra entryDate de todos los problemas que se pueden resolver en un proyecto](assets/resolvables-entry-date.png)

### Proyecto: muestra el grupo principal del solicitante del proyecto original

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Una imagen de pantalla que muestra el grupo de inicio del solicitante del proyecto](assets/requestor-home-group.png)

### Proyecto: mostrar si el proyecto es una cola de solicitudes

```
querysort=queueDef:isPublic
valueformat=val
description=0 (None), 1 (Public), 2 (Private), 3 (Company), 4 (Group)
linkedname=direct
textmode=true
enumtype=PROJ
valuefield=queueDef:isPublic
namekey=status
type=enum
enumclass=com.attask.common.constants.ProjectStatusEnum
displayname=Public Selection
```

![Una imagen de pantalla que muestra si el proyecto es una cola de solicitudes](assets/project-is-a-request-queue.png)

### Problema: iteración que muestra todos los integrantes del equipo del proyecto de resolución

```
displayname=Resolve Project: Team Members
listdelimiter=<br>
listmethod=nested(resolveProject.projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
width=150
```

![Una imagen de pantalla que muestra todos los integrantes del equipo del proyecto de resolución](assets/all-resolve-project-team-members.png)

### Problema: iteración que muestra todos los equipos del contacto principal del problema

```
displayname=Requestor Teams
listdelimiter=<br>
listmethod=nested(owner.teams).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=name
valueformat=HTML
width=150
```

![Una imagen de pantalla que muestra todos los equipos de contacto principales](assets/all-primary-contact-teams.png)

### Documento: iteración que muestra la carpeta en un informe de documento

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![Imagen de pantalla que muestra la carpeta en un informe de documento](assets/folder-in-a-document-report.png)

### Documento: iteración que muestra la carpeta principal en un informe de documento

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![Imagen de pantalla que muestra la carpeta principal en un informe de documento](assets/parent-folder-in-a-document-report.png)

### Documento: fechas de aprobación del documento

```
displayname=Document approval dates
valueformat=HTML
listdelimiter=<br>
linkedname=direct
textmode=true
listsort=string(description)
valuefield=approvalDate
type=iterate
listmethod=nested(approvals).lists
shortview=false
section=0
```

![Una imagen de pantalla que muestra la vista fechas de aprobación del documento](assets/document-approval-dates.png)

### Aprobaciones de revisión

#### Aprobación de prueba: mostrar nombre del proyecto

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

#### Aprobación de prueba: mostrar nombre de tarea

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Una imagen de pantalla que muestra el proyecto y la tarea de una aprobación de prueba](assets/proof-approval-project-and-task.png)
