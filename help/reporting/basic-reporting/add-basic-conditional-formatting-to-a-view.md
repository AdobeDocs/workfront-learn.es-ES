---
title: Añadir un formato condicional básico a una vista
description: Aprenda a utilizar reglas de columna para cambiar el color del texto, el formato y los colores de fondo en un informe o una vista, según los criterios que haya establecido.
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: 2c9e57b8f85c74061bd3e52ef4eaea60bc4ec5bb
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 95%

---

# Añadir un formato condicional básico a una vista

El formato condicional se realiza creando reglas de columna. Las reglas de columna permiten dar un formato específico a la columna basándose en el criterio que usted elija.

Este vídeo contiene información sobre:

* ¿Qué formato condicional hay en una vista?
* Cómo crear y modificar el formato condicional

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)


## Resumen de formato condicional

Para crear un formato condicional:

1. Elija la columna donde desea que aparezca el formato
1. Decida en qué condiciones desea cambiar el formato
1. Decida qué tipo de cambio de formato funcionará mejor

   * Color de fondo
   * Color de texto
   * texto de reemplazo
   * mostrar un icono

## Actividades &quot;Añadir formato condicional básico a una vista&quot;

### Actividad 1: Agregar formato condicional a una vista

Cree una vista de tarea denominada “Estándar + Progreso” utilizando la vista Estándar existente y añadiendo este formato condicional en la columna [!UICONTROL Nombre].

1. Añada una regla de columna que ponga el campo en segundo plano en rojo cuando el estado de progreso de la tarea sea Tarde.
1. Agregue una regla de columna que haga que el fondo del campo aparezca de color amarillo cuando el estado de progreso sea Detrás o En riesgo.

Esto le ayudará a identificar las tareas con problemas sin incluir la columna para el estado de progreso como parte de la vista.

### Respuesta 1

![Imagen de la pantalla para crear una nueva regla de columna](assets/conditional-formatting-exercise.png)

1. En un informe de lista de tareas, vaya al menú desplegable **[!UICONTROL Ver]** y seleccione **[!UICONTROL Nueva vista]**.
1. Asigne un nombre a la vista “Estándar + Progreso”.
1. Utilice las columnas predeterminadas proporcionadas.
1. Seleccione la columna [!UICONTROL Nombre de la tarea]. Esta es la columna a la que desea aplicar el formato condicional, por lo que aparece en rojo o amarillo si el estado de progreso de la tarea no es Tiempo activo.
1. Haga clic en **[!UICONTROL Opciones avanzadas]** en la esquina superior derecha de la ventana del Creador de informes.
1. Haga clic en **[!UICONTROL Añadir una regla para esta columna]**.
1. Inicie la regla de columna cambiando [!UICONTROL Tarea] > [!UICONTROL Nombre] en la parte superior de la ventana para [!UICONTROL Tarea] > [!UICONTROL Estado de progreso]. Haga clic en el icono **[!UICONTROL X]** junto a [!UICONTROL Tarea] > [!UICONTROL Nombre] para eliminarlo del campo.
1. Escriba “progreso” en el campo y, a continuación, seleccione[!UICONTROL  Estado de progreso] en el origen del campo [!UICONTROL Tarea].
1. Seleccione **[!UICONTROL Tarde]** en el campo a la derecha del calificador [!UICONTROL Igual].
1. Elija un fondo de rojo en la fila [!UICONTROL Color del texto].
1. Haga clic en **[!UICONTROL Agregar regla]** para guardar la regla de columna.
1. Ahora haga clic en **[!UICONTROL Agregar regla de columna]** de nuevo para agregar otra regla.
1. Igual que antes, elimine [!UICONTROL Tarea] > [!UICONTROL Nombre] del campo criterios. Sustitúyalo por [!UICONTROL Estado de progreso] en el origen del campo [!UICONTROL Tarea].
1. Seleccione ambos [!UICONTROL En riesgo] y [!UICONTROL Detrás] en el campo a la derecha del calificador Igual.
1. Elija un fondo amarillo en la fila [!UICONTROL Color del texto].
1. Haga clic en **[!UICONTROL Agregar regla]** para guardar la regla de columna.
1. Haga clic en **[!UICONTROL Guardar vista]** para guardar la vista.
