---
title: Añadir formato condicional básico a las actividades de una vista
description: Practique agregando formato condicional básico a las vistas, con instrucciones paso a paso.
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8855
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 87%

---

# Añadir formato condicional básico a las actividades de una vista

Practique agregando formato condicional básico a las vistas, con instrucciones paso a paso.

## Resumen

Para crear un formato condicional:

1. Elija la columna donde desea que aparezca el formato
1. Decida en qué condiciones desea cambiar el formato
1. Decida qué tipo de cambio de formato funcionará mejor

   * Color de fondo
   * Color de texto
   * texto de reemplazo
   * mostrar un icono

## Actividad 1: Agregar formato condicional a una vista

Cree una vista de tarea denominada “Estándar + Progreso” utilizando la vista Estándar existente y añadiendo este formato condicional en la columna [!UICONTROL Nombre].

1. Añada una regla de columna que ponga el campo en segundo plano en rojo cuando el estado de progreso de la tarea sea Tarde.
1. Agregue una regla de columna que haga que el fondo del campo aparezca de color amarillo cuando el estado de progreso sea Detrás o En riesgo.

Esto le ayudará a identificar las tareas con problemas sin incluir la columna para el estado de progreso como parte de la vista.

## Respuesta 1

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
