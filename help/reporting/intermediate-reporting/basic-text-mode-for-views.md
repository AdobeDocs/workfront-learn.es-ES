---
title: Comprender el modo de texto básico de las vistas
description: Aprenda qué es el modo de texto, qué es el caso del camello y algún modo de texto básico de "Plug and Play" que puede utilizar en sus vistas de Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
source-git-commit: 59ac9907b116f8abadf5e15f8de351c02a7a2909
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Comprender el modo de texto básico de las vistas


>[!IMPORTANT]
>
>Requisitos previos:
>
>* Explicación de los elementos de informes
>* Comprender los componentes del sistema de informes
>* Crear una vista básica


En este vídeo, aprenderá:

* Qué modo de texto es
* Qué caso de camello es
* Algunos modos básicos de texto &quot;Plug and Play&quot; que puede utilizar en sus vistas

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12)

## Tarea - Vista de 4 padres

Cree primero una columna para el Nombre de la tarea y el Nombre principal y, a continuación, utilice el siguiente modo de texto para crear las otras tres columnas.

### Tarea - Principal del nombre principal

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

### Tarea - Principal del Nombre Principal

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

### Tarea - Principal del Principal del Nombre Principal

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

## Usuario : iteraciones que muestran listas en las vistas de usuario

### Usuario: todas las funciones de trabajo

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### Usuario: todas las funciones de trabajo que muestran el rol principal

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### Usuario: todos los equipos

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
>Hay un campo Equipo al que se puede acceder a través de la interfaz de usuario que muestra todos los equipos separados por coma, pero al usar el modo de texto anterior se mostrará a cada equipo en una línea independiente.


### Usuario: todos los grupos

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### Usuario: todos los grupos que muestran el grupo principal

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### Usuario: informes directos

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### Usuario: futuro PTO

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

## Tarea: Cómo mostrar las asignaciones de tareas y trabajar en el estado

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


## Tarea - Cómo mostrar la función y la asignación en varias asignaciones de tareas

### Tarea - Función + horas

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### Tarea - Asignación + asignación porcentual

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

## Tarea: predecesores y sucesores de varios proyectos

### Filtro de tareas (opcional)

**Mostrar todas las tareas que tengan al menos un predecesor de proyecto cruzado**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Tarea: Mostrar nombres de predecesor y predecesor de proyecto en

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

### Tarea: Mostrar nombres de sucesores y sucesores de proyectos en

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

### Tarea: Mostrar la fecha de finalización prevista de las predecesoras

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

### Tarea: mostrar el estado de progreso de las predecesoras

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

### Tarea: Mostrar el porcentaje completado del proyecto del predecesor de proyectos cruzados

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

![Una imagen de pantalla que muestra la vista Cruzar predecesores y sucesores del proyecto](assets/cross-project-predecessors-and-successors.png)


## Tarea : iteración que muestra todas las personas asignadas y que asignaron cada una

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![Una imagen de pantalla que muestra todas las personas asignadas y que asignaron cada una](assets/all-assignees-and-requesters.png)

## Tarea/proyecto: iteración que muestra todos los formularios personalizados de un proyecto o una tarea

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


## Proyecto: Iteración que muestra todos los contactos principales para las variables resueltas en la vista del proyecto

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

![Una imagen de pantalla que muestra los contactos principales para las variables resuelvas](assets/primary-contacts-for-resolvables.png)

## Proyecto: iteración que muestra todos los miembros del equipo del proyecto

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

![Una imagen de pantalla que muestra todos los miembros del equipo del proyecto](assets/all-project-team-members.png)

## Proyecto: Iteración que muestra la entryDate de todos los problemas resolvibles de un proyecto

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

## Proyecto: muestra el grupo principal del solicitante del proyecto original

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

## Proyecto: Mostrar si el proyecto es una cola de solicitudes

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

## Problema: Iteración que muestra todos los miembros del equipo del proyecto de resolución

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

![Una imagen de pantalla que muestra todos los miembros del equipo del proyecto de resolución](assets/all-resolve-project-team-members.png)

## Problema : iteración que muestra todos los equipos del contacto principal del problema

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

## Documento: Iteración que muestra la carpeta en un informe de documento

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

## Documento: Iteración que muestra la carpeta principal en un informe de documento

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

## Documento: Fechas de aprobación del documento

```
displayname=Document Approval Dates
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

![Una imagen de pantalla que muestra la vista Fechas de aprobación del documento](assets/document-approval-dates.png)

## Aprobaciones de revisión

### Aprobación de prueba: mostrar nombre del proyecto

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### Aprobación de prueba - Mostrar nombre de tarea

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Una imagen de pantalla que muestra el proyecto y la tarea de una aprobación de prueba](assets/proof-approval-project-and-task.png)

