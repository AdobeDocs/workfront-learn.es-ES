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
source-git-commit: 8cd01b3dca3a62c1d8699d7d076dccddf2010907
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 47%

---

# Creación de un informe de tareas

Este vídeo contiene información sobre:

* Cómo crear un informe de tareas con un filtro complejo
* Cómo encontrar los informes que crea

>[!VIDEO](https://video.tv.adobe.com/v/335154/?quality=12&learn=on)

## Actividad 1: Crear un informe de notas con indicadores

Cree un informe de Notas que pueda usar para buscar notas del usuario (es decir, comentarios o actualizaciones) o notas del sistema basadas en el contenido, el autor, la fecha de entrada, el nombre del proyecto o el tipo de auditoría. Asigne un nombre al informe &quot;Búsqueda de notas&quot;.

Cuando se utiliza la instrucción Texto de nota, este informe buscará dentro de los hilos de actualización para extraer rápidamente cualquiera que cumpla los criterios especificados. Al ejecutar el informe, no es necesario que rellene todos los mensajes, solo los que le interesen. Las que están en blanco se ignoran automáticamente.

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

## Respuesta de actividad 1

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
1. Abrir **[!UICONTROL Configuración de informes]** y asigne al informe el nombre &quot;Búsqueda de notas&quot;.
1. En el [!UICONTROL Descripción] , ponga algo como, &quot;Buscar notas del sistema o del usuario basadas en el tipo de auditoría seleccionado y otras indicaciones. Las notas del sistema aparecen en la columna Texto de auditoría y las notas del usuario en la columna Texto de nota.&quot;

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

## Actividad 2: Crear un informe de comentarios del equipo de administración

Este es un informe de problemas que muestra todos los problemas de una cola de solicitudes de comentarios creada para los administradores del sistema. Puede ver cómo crear esta cola de solicitudes en la [Crear una cola de solicitudes de comentarios de administrador del sistema](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-system-admin-feedback-request-queue.html) tutorial.

Este informe también utiliza un formulario personalizado. Para obtener información sobre cómo crear un formulario personalizado, consulte la [Crear y compartir un formulario personalizado](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/custom-data/custom-forms/custom-forms-creating-and-sharing-a-custom-form.html) tutorial.

Este formulario personalizado debe crearse de la siguiente manera:

Nombre: Comentarios del proceso de administración

1. Tipo de proceso (campo desplegable)
   * niveles de acceso
   * proceso de aprobación (solo global)
   * notificaciones por correo electrónico
   * plantilla de diseño
   * ruta de hitos
   * plantilla de proyecto
   * notificaciones de recordatorio
   * cola de solicitudes
1. Nombre del proceso (campo de texto de una sola línea)
1. Grado del proceso (campo desplegable)
   * 1 - totalmente inútil
   * 2 - no es muy útil
   * 3 - bueno, pero podría ser mejor
   * 4 - excelente
1. Problema o buenas noticias (campo de texto de párrafo)

Cree un informe de problemas denominado **Informe de comentarios del equipo de administración**.

La vista debe tener las columnas siguientes:

* Problema: Nombre
* Contacto principal: Nombre
* Problema: Tipo de proceso
* Problema: Nombre del proceso
* Problema: Grado del proceso
* Problema: Problema o buenas noticias
* Problema: Fecha de entrada
* Problema: Edad
* Problema: Asignaciones
* Problema: estado

Agrupar por tipo de proceso.

Filtre por el ID del proyecto de la cola de solicitudes donde residen los problemas de comentarios.


![Captura de pantalla del informe de comentarios del equipo de administración](assets/create-a-system-admin-feedback-request-queue.png)



## Respuesta de actividad 2

1. Seleccione **[!UICONTROL Informes]** desde el **[!UICONTROL Menú principal]**.
1. Haga clic en **[!UICONTROL Nuevo informe]** y seleccione **[!UICONTROL Problema]**.
1. En **[!UICONTROL Columnas (Vista)]**, configure las columnas para incluir lo siguiente:

   ![Imagen de la pantalla para crear columnas de informe de problemas](assets/task-report-activity-2-1.png)

   * [!UICONTROL Problema] > [!UICONTROL Nombre]
   * [!UICONTROL Contacto principal] > [!UICONTROL Nombre]
      * Nota: Aparece con &quot;Propietario:Nombre&quot; como etiqueta de columna. Puede cambiarlo a &quot;Notificado por&quot; haciendo clic en Opciones avanzadas y escribiendo &quot;Notificado por&quot; en **Etiqueta de columna personalizada** field.
   * [!UICONTROL Problema] > [!UICONTROL Tipo de proceso]
   * [!UICONTROL Problema] > [!UICONTROL Nombre del proceso]
   * [!UICONTROL Problema] > [!UICONTROL Grado del proceso]
   * [!UICONTROL Problema] > [!UICONTROL Problema o buenas noticias]
   * [!UICONTROL Problema] > [!UICONTROL Fecha de entrada]
   * [!UICONTROL Problema] > [!UICONTROL Edad]
   * [!UICONTROL Problema] > [!UICONTROL Asignaciones]
   * [!UICONTROL Problema] > [!UICONTROL Estado]

1. Seleccione la columna **[!UICONTROL Fecha de entrada]** y cambie a **[!UICONTROL Orden de bajada]**.
1. En el **[!UICONTROL Agrupaciones]** pestaña, configure el informe para que se agrupe por **[!UICONTROL Problema] > [!UICONTROL Tipo de proceso]**.

   ![Imagen de la pantalla para crear agrupaciones de informes de problemas](assets/task-report-activity-2-2.png)

1. En el **[!UICONTROL Filtros]** pestaña, añada un filtro para **[!UICONTROL Problema] > [!UICONTROL Identificador de proyecto]** para coincidir con el proyecto de la cola de solicitudes donde residen los problemas de comentarios.

   ![Imagen de la pantalla para crear filtros de informe de problemas](assets/task-report-activity-2-3.png)

1. Guarde y cierre el informe.
