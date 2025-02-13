---
title: Crear actividades de tablero
description: Practique la creación de paneles, con instrucciones paso a paso.
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335157.png
jira: KT-8862
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 49%

---

# Crear actividades de tablero

Practique la creación de paneles, con instrucciones paso a paso.

## Actividad 1: Crear un tablero

Crear un [!UICONTROL tablero] con un solo informe:&quot;Buscar notas en este proyecto&quot;. Esto es útil para encontrar rápidamente cualquier actualización realizada en un proyecto, incluso si hay miles de actualizaciones para buscar. Esto buscará en los subprocesos de actualización para extraer rápidamente cualquier actualización que cumpla los criterios especificados en los mensajes.

Cree este informe haciendo una copia del informe &quot;Notas de búsqueda&quot; que creó en la actividad &quot;Crear un informe de notas&quot; (o use otro informe si no realizó esa actividad).

* Elimine el mensaje Nombre del proyecto de la copia y cambie el nombre del informe a &quot;Notas de búsqueda en este proyecto&quot;.
* Asigne un nombre al [!UICONTROL panel] &quot;Notas de búsqueda&quot;.
* Vaya a cualquier página de aterrizaje del proyecto y cree una sección personalizada para un [!UICONTROL panel].
* Tenga en cuenta que cuando busque notas en la sección personalizada, solo mostrará las notas contenidas en el proyecto en el que se encuentra actualmente.

## Respuesta 1

1. Ejecute el informe que ha creado en la actividad Crear un informe de notas.
1. Haga clic en **[!UICONTROL Acciones de informe]** y seleccione **[!UICONTROL Copiar]**. [!DNL Workfront] crea un nuevo informe denominado &quot;Búsqueda de notas (copia)&quot;.
1. Vaya a **[!UICONTROL Acciones de informe]** y seleccione **[!UICONTROL Editar]**. Haga clic en **[!UICONTROL Configuración de informes]** y cambie el nombre a &quot;Buscar notas en este proyecto&quot;.
1. Haga clic en [!UICONTROL Mensajes del informe] y elimine el mensaje [!UICONTROL Proyecto] > [!UICONTROL Nombre] de la lista.

   ![Una imagen de la pantalla para crear un panel nuevo](assets/edit-report-prompts.png)

1. Marque la casilla **[!UICONTROL Mostrar solicitudes en el panel]**.
1. Haga clic en **[!UICONTROL Listo]**, luego **[!UICONTROL Guardar + Cerrar]**. Ahora está viendo la pantalla [!UICONTROL Mensajes] del informe.

   A continuación, utilizará un acceso directo para crear un nuevo tablero y agregarle este informe.

1. Haga clic en **[!UICONTROL Acciones de informe]** y seleccione **[!UICONTROL Agregar al panel]** > **[!UICONTROL Nuevo panel]**.
1. Arrastre el informe &quot;Notas de búsqueda en este proyecto&quot; al panel **[!UICONTROL Diseño]**.
1. Observe que el nombre del informe se convierte en el nombre del panel. Edite el nombre para que aparezca &quot;Notas de búsqueda&quot;.

   ![Una imagen de la pantalla para crear un panel nuevo](assets/create-dashboard.png)

1. Haga clic en **[!UICONTROL Guardar + Cerrar]**.

   Ahora, agregue el panel a una página de proyecto.

   ![Una imagen de la pantalla para crear un panel nuevo](assets/add-custom-section.png)

1. Vaya a cualquier proyecto. En el menú del panel izquierdo, haga clic en el icono **[!UICONTROL Agregar sección personalizada]**.
1. En el campo **[!UICONTROL Agregar un panel]**, escriba &quot;Notas de búsqueda&quot; y seleccione el [!UICONTROL panel] de la lista.
1. En el campo **[!UICONTROL Título de sección personalizada]**, escriba &quot;Notas de búsqueda&quot;.
1. Haga clic en **[!UICONTROL Añadir nueva sección]**.
1. En el menú del panel izquierdo, busque Notas de búsqueda. Haga clic en los puntos a la izquierda del nombre de la sección y arrástrelo justo debajo de Actualizaciones.
