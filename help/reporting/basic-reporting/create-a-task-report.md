---
title: Creación de un informe de tareas
description: 'Aprenda a crear un informe de tareas con un filtro complejo y a encontrar los informes que crea en Workfront. Actividad: crear un informe de notas con instrucciones.'
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
jira: KT-8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 100%

---

# Creación de un informe de tareas

Este vídeo contiene información sobre:

* Cómo crear un informe de tareas con un filtro complejo
* Cómo encontrar los informes que crea

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## Actividad: Creación de un informe de notas con instrucciones

Cree un informe de Notas que pueda usar para buscar notas del usuario (es decir, comentarios o actualizaciones) o notas del sistema basadas en el contenido, el autor, la fecha de entrada, el nombre del proyecto o el tipo de auditoría. Asigne al informe el nombre “Búsqueda de notas”.

Cuando se utiliza la instrucción Texto de nota, este informe buscará dentro de los hilos de actualización para extraer rápidamente cualquiera que cumpla los criterios especificados. Al ejecutar el informe, no es necesario rellenar todas las instrucciones, solo las que le interesen. Las que están en blanco se ignoran automáticamente.

La vista debe incluir columnas para lo siguiente:

* Texto de nota
* Auditar texto
* Fecha de entrada
* Propietario: Nombre
* Tipo de auditoría
* Nombre de la tarea
* Nombre del problema

Deje la pestaña Filtro en blanco.

Grupo en Nombre del proyecto.

Incluya instrucciones para lo siguiente:

* Auditar texto
* Texto de nota
* Nombre del propietario
* Fecha de entrada
* Nombre del proyecto
* Tipo de auditoría

## Respuesta

1. Seleccione **[!UICONTROL Informes]** desde el **[!UICONTROL Menú principal]**.
1. Haga clic en el menú **[!UICONTROL Nuevo informe]** y seleccione **[!UICONTROL Nota]**.
1. En **[!UICONTROL Columnas (Vista)]**, configure las columnas para incluir lo siguiente:

   ![Una imagen de la pantalla para crear columnas de informes de notas](assets/note-report-columns.png)

   * [!UICONTROL Nota] > [!UICONTROL Texto de nota]
   * [!UICONTROL Nota] > [!UICONTROL Texto de auditoría]
   * [!UICONTROL Nota] > [!UICONTROL Fecha de entrada]
   * [!UICONTROL Propietario] > [!UICONTROL Nombre]
   * [!UICONTROL Nota] > [!UICONTROL Tipo de auditoría]
   * [!UICONTROL Tarea] > [!UICONTROL Nombre]
   * [!UICONTROL Problema] > [!UICONTROL Nombre]

1. Seleccione la columna **[!UICONTROL Fecha de entrada]** y cambie a **[!UICONTROL Orden de bajada]**.
1. En la pestaña **[!UICONTROL Agrupaciones]**, configure el informe para agruparlo por [!UICONTROL Proyecto] > [!UICONTROL Nombre].

   ![Una imagen de la pantalla para crear agrupaciones de informes de notas](assets/note-report-groupings.png)

1. Deje [!UICONTROL Filtros] en blanco.
1. Abra **[!UICONTROL Configuración de informes]** y asigne el nombre “Búsqueda de notas”.
1. En el campo [!UICONTROL Descripción], escriba algo como “Buscar notas del sistema o del usuario según el tipo de auditoría seleccionado y otras instrucciones. Las notas del sistema aparecen en la columna Texto de auditoría y las del usuario aparecen en la columna Texto de nota”.

   ![Una imagen de la pantalla para crear la configuración del informe de notas](assets/note-report-report-options.png)

1. Seleccione la **[!UICONTROL pestaña Detalles]** para que se muestre cuando se cargue el informe.
1. Configure el informe para que muestre 200 elementos cuando se incluya en un tablero.
1. Haga clic en **[!UICONTROL Instrucciones del informe]** y añada lo siguiente:

   ![Una imagen de la pantalla para crear instrucciones del informe de notas](assets/note-report-report-prompts.png)

   * [!UICONTROL Nota] > [!UICONTROL Texto de auditoría]
   * [!UICONTROL Nota] > [!UICONTROL Texto de nota]
   * [!UICONTROL Propietario] > [!UICONTROL Nombre]
   * [!UICONTROL Nota] > [!UICONTROL Fecha de entrada]
   * [!UICONTROL Proyecto] > [!UICONTROL Nombre]
   * [!UICONTROL Nota] > [!UICONTROL Tipo de auditoría]

1. Marque la casilla de verificación **[!UICONTROL Mostrar instrucciones en tableros]**.
1. Guarde y cierre el informe.
