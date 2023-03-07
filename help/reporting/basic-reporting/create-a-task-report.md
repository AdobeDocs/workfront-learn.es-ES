---
title: Crear un informe de tareas
description: 'Aprenda a crear un informe de tareas con un filtro complejo y a encontrar los informes que crea en Workfront. Actividad: crear un informe de notas con instrucciones.'
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335154.png
kt: 8859
exl-id: 90bad2e8-9cd2-4ae7-973b-eeab9d615bef
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 11%

---

# Crear un informe de tareas

En este vídeo, aprenderá lo siguiente:

* Creación de un informe de tareas con un filtro complejo
* Cómo encontrar los informes que crea

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12)

## Actividad: Crear un informe de notas con indicadores

Cree un informe de notas que pueda utilizar para buscar notas de usuarios (es decir, comentarios o actualizaciones) o notas del sistema basadas en el contenido de la nota, el autor, la fecha de entrada, el nombre del proyecto o el tipo de auditoría. Asigne un nombre al informe &quot;Búsqueda de notas&quot;.

Cuando se utiliza el símbolo del sistema Texto de la nota, este informe buscará dentro de los subprocesos de actualización para extraer rápidamente los que cumplan los criterios especificados en los mensajes. Al ejecutar el informe, no es necesario que rellene todos los mensajes, solo los que le interesen. Los espacios en blanco se ignoran automáticamente.

La vista debe incluir columnas para:

* Texto de la nota
* Auditar texto
* Fecha de entrada
* Propietario: nombre
* Tipo de auditoría
* Nombre de la tarea
* Nombre de problema

Deje la pestaña de filtro en blanco.

Agrupar por nombre de proyecto.

Incluya peticiones de datos para lo siguiente:

* Auditar texto
* Texto de la nota
* Nombre del propietario
* Fecha de entrada
* Nombre del proyecto
* Tipo de auditoría

## Respuesta

1. Seleccionar **[!UICONTROL Informes]** desde el **[!UICONTROL Menú principal]**.
1. Haga clic en **[!UICONTROL Nuevo informe]** y seleccione **[!UICONTROL Nota]**.
1. Entrada **[!UICONTROL Columnas (vista)]** configure las columnas para que incluyan:

   ![Imagen de la pantalla para crear columnas de informe de notas](assets/note-report-columns.png)

   * [!UICONTROL Nota] > [!UICONTROL Texto de nota]
   * [!UICONTROL Nota] > [!UICONTROL Auditar texto]
   * [!UICONTROL Nota] > [!UICONTROL Fecha de entrada]
   * [!UICONTROL Propietario] > [!UICONTROL Nombre]
   * [!UICONTROL Nota] > [!UICONTROL Tipo de auditoría]
   * [!UICONTROL Tarea] > [!UICONTROL Nombre]
   * [!UICONTROL Problema] > [!UICONTROL Nombre]

1. Seleccione el **[!UICONTROL Fecha de entrada]** y cambie la **[!UICONTROL Ordenar a descendente]**.
1. En el **[!UICONTROL Agrupaciones]** pestaña, configure el informe para que se agrupe por [!UICONTROL Proyecto] > [!UICONTROL Nombre].

   ![Imagen de la pantalla para crear agrupaciones de informes de notas](assets/note-report-groupings.png)

1. Salir [!UICONTROL Filtros] en blanco.
1. Abrir **[!UICONTROL Configuración de informes]** y asigne al informe el nombre &quot;Búsqueda de notas&quot;.
1. En el [!UICONTROL Descripción] , ponga algo como, &quot;Buscar notas del sistema o del usuario basadas en el tipo de auditoría seleccionado y otras indicaciones. Las notas del sistema aparecen en la columna Texto de auditoría y las notas del usuario en la columna Texto de nota.&quot;

   ![Imagen de la pantalla para crear la configuración del informe de notas](assets/note-report-report-options.png)

1. Seleccionar **[!UICONTROL Pestaña Detalles]** para que se muestre cuando se cargue el informe.
1. Configure el informe para que muestre 200 elementos cuando el informe se incluya en un tablero.
1. Clic **[!UICONTROL Indicadores de informe]** y añada:

   ![Imagen de la pantalla para crear solicitudes de informe de notas](assets/note-report-report-prompts.png)

   * [!UICONTROL Nota] > [!UICONTROL Auditar texto]
   * [!UICONTROL Nota] > [!UICONTROL Texto de nota]
   * [!UICONTROL Propietario] > [!UICONTROL Nombre]
   * [!UICONTROL Nota] > [!UICONTROL Fecha de entrada]
   * [!UICONTROL Proyecto] > [!UICONTROL Nombre]
   * [!UICONTROL Nota] > [!UICONTROL Tipo de auditoría]

1. Marque la casilla para **[!UICONTROL Mostrar indicadores en los paneles]**.
1. Guarde y cierre el informe.
