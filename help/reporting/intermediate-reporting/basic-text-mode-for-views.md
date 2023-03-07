---
title: Comprender el modo de texto básico de las vistas
description: Aprenda qué es el modo texto, qué es camel case y algunos modos de texto básicos "plug and play" que puede utilizar en sus vistas en Workfront.
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Comprender el modo de texto básico de las vistas


>[!IMPORTANT]
>
>Requisitos previos:
>
>* Comprender los elementos de informes
>* Comprender los componentes de informes
>* Crear una vista básica


>[!TIP]
>
>* Para comprender mejor el modo de texto, le recomendamos que vea el evento del seminario web grabado [Pregunte al experto - Introducción a los informes en modo texto](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en), que tiene una hora de duración.
>* Para obtener más información acerca del modo de texto, le recomendamos que vea la [Informes avanzados](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) tutoriales, que en conjunto tienen una duración de cinco horas y media.


En este vídeo, aprenderá lo siguiente:

* Qué modo de texto es
* Qué es Camel Case
* Algunos modos de texto básicos &quot;plug and play&quot; que puede utilizar en sus vistas

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12)

## Tarea: vista de 4 elementos principales

Cree primero una columna para el Nombre de tarea y el Nombre principal y, a continuación, utilice el siguiente modo de texto para crear las otras tres columnas.

### Tarea: elemento principal del nombre principal

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

### Tarea: elemento principal del nombre principal

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

### Tarea: elemento principal del elemento principal del nombre principal

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

![Imagen de pantalla que muestra la vista de 4 elementos principales](assets/4-parents-view.png)

## Usuario: iteraciones que muestran listas en vistas de usuario

### Usuario - Todos los roles

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### Usuario - Se muestran todos los roles principales

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### Usuario - Todos los equipos

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
>Hay un campo Equipo accesible a través de la interfaz de usuario que muestra todos los equipos separados por comas, pero el uso del modo de texto anterior mostrará a cada equipo en una línea independiente.


### Usuario - Todos los grupos

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### Usuario: todos los grupos muestran el grupo de inicio

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### Usuario - Informes directos

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### Usuario - Futura PTO

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

![Imagen de pantalla que muestra la vista Listas de usuarios](assets/user-lists-view-large.png)

## Tarea: cómo mostrar las asignaciones de tareas y cómo trabajar en el estado

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

![Imagen de pantalla que muestra la vista Asignaciones y estado](assets/assignments-and-status-view.png)


## Tarea: cómo mostrar la función y la asignación en varias asignaciones de tareas

### Tarea - Rol + horas

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

![Imagen de pantalla que muestra la vista Asignaciones y roles](assets/assignments-roles-and-percent-view.png)

## Tarea: predecesoras y sucesoras entre proyectos

### Filtro de tareas (opcional)

**Mostrar todas las tareas que tengan al menos una predecesora entre proyectos**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### Tarea: mostrar los nombres de las predecesoras y el predecesor del proyecto en

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

### Tarea: mostrar los nombres de las sucesoras y la sucesora del proyecto en

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

### Tarea: mostrar la fecha proyectada de finalización de las predecesoras

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

### Tarea: mostrar el porcentaje completado del proyecto del predecesor entre proyectos

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

![Imagen de pantalla que muestra la vista Predecesoras y sucesoras entre proyectos](assets/cross-project-predecessors-and-successors.png)


## Tarea: iteración que muestra todas las personas asignadas y que asignaron cada una

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![Imagen de pantalla que muestra todas las personas asignadas y asignadas a cada una](assets/all-assignees-and-requesters.png)

## Tarea/proyecto: iteración que muestra todos los formularios personalizados en un proyecto o tarea

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![Imagen de pantalla que muestra todos los formularios personalizados de un proyecto](assets/all-custom-forms-on-a-project.png)


## Proyecto: Iteración que muestra todos los contactos principales para los solucionables en la vista de proyecto

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

![Imagen de pantalla que muestra los contactos principales de los objetos solucionables](assets/primary-contacts-for-resolvables.png)

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

![Imagen de pantalla que muestra todos los integrantes del equipo del proyecto](assets/all-project-team-members.png)

## Proyecto: iteración que muestra la entryDate de todos los problemas solucionables de un proyecto

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

![Imagen de pantalla que muestra entryDate de todos los problemas que se pueden resolver de un proyecto](assets/resolvables-entry-date.png)

## Proyecto: mostrar el grupo de inicio del solicitante del proyecto original

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![Imagen de pantalla que muestra el grupo de inicio del solicitante del proyecto](assets/requestor-home-group.png)

## Proyecto: mostrar si el proyecto es una cola de solicitudes

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

![Imagen de pantalla que muestra si el proyecto es una cola de solicitudes](assets/project-is-a-request-queue.png)

## Problema: iteración que muestra todos los miembros del equipo del proyecto resueltos

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

![Imagen de pantalla que muestra todos los integrantes del equipo del proyecto de resolución](assets/all-resolve-project-team-members.png)

## Problema: iteración que muestra todos los equipos del contacto principal del problema

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

![Imagen de pantalla que muestra todos los equipos de contacto principales](assets/all-primary-contact-teams.png)

## Documento: iteración que muestra la carpeta en un informe de documento

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

## Documento: iteración que muestra la carpeta principal en un informe de documento

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![Imagen de pantalla que muestra la carpeta principal de un informe de documento](assets/parent-folder-in-a-document-report.png)

## Documento - Fechas de aprobación del documento

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

![Imagen de pantalla que muestra la vista Fechas de aprobación del documento](assets/document-approval-dates.png)

## Aprobaciones de revisión

### Aprobación de revisión - Mostrar nombre del proyecto

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### Aprobación de revisión - Mostrar nombre de tarea

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![Imagen de pantalla que muestra el proyecto y la tarea de una aprobación de prueba](assets/proof-approval-project-and-task.png)
