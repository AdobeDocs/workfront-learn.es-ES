---
title: Añadir formato condicional básico
description: Aprenda a utilizar las reglas de columna para cambiar el color del texto, el formato y los colores de fondo en un informe o vista, en función de los criterios que establezca.
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: 0ee80dceb8208bd0360fd8c9ab68fb8a73677a9d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Agregar formato condicional básico a una vista

El formato condicional se realiza creando reglas de columna. Las reglas de columna permiten dar formato a una columna de una manera específica según los criterios que establezca.

En este vídeo, aprenderá lo siguiente:

* Qué es el formato condicional en una vista
* Creación y modificación del formato condicional

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)

## Resumen

Para crear un formato condicional:

1. Elija la columna donde desea que aparezca el formato
1. Decida qué condiciones desea que cambie el formato
1. Decida qué tipo de cambio de formato funcionará mejor

   * color de fondo
   * color del texto
   * texto de reemplazo
   * mostrar un icono

## Actividad: añadir formato condicional a una vista

Cree una vista de tareas denominada &quot;Estándar + Progreso&quot; utilizando la vista Estándar existente y agregando este formato condicional a la vista [!UICONTROL Nombre] columna.

1. Agregue una regla de columna que pondrá el fondo del campo en rojo cuando el estado del progreso de la tarea sea Late.
1. Agregue una regla de columna que pondrá de color amarillo el fondo del campo cuando el estado del progreso sea Retrasado o En riesgo.

Esto le ayudará a identificar tareas con problemas sin incluir la columna para el estado de progreso como parte de la vista.

## Respuesta

![Imagen de la pantalla para crear una regla de columna nueva](assets/conditional-formatting-exercise.png)

1. En un informe de lista de tareas, vaya a **[!UICONTROL Ver]** menú desplegable y seleccione **[!UICONTROL Nueva vista]**.
1. Asigne a la vista el nombre &quot;Estándar + Progreso&quot;.
1. Utilice las columnas predeterminadas proporcionadas.
1. Seleccione el [!UICONTROL Nombre de tarea] columna. Esta es la columna a la que desea aplicar el formato condicional, por lo que aparece en rojo o amarillo si el estado de progreso de la tarea no es A tiempo.
1. Clic **[!UICONTROL Opciones avanzadas]** en la esquina superior derecha de la ventana de report builder.
1. Clic **[!UICONTROL Agregar una regla para esta columna]**.
1. Inicie la regla de columna cambiando [!UICONTROL Tarea] > [!UICONTROL Nombre] en la parte superior de la ventana para [!UICONTROL Tarea] > [!UICONTROL Estado de progreso]. Simplemente haga clic en **[!UICONTROL X]** junto a [!UICONTROL Tarea] > [!UICONTROL Nombre] para eliminarlo del campo.
1. Escriba &quot;progress&quot; en el campo y seleccione [!UICONTROL Estado de progreso] en el [!UICONTROL Tarea] origen del campo.
1. Seleccionar **[!UICONTROL Retrasado]** en el campo a la derecha de [!UICONTROL Igual] calificador.
1. Elija un fondo rojo en la [!UICONTROL Color del texto] fila.
1. Clic **[!UICONTROL Agregar regla]** para guardar la regla de columna.
1. Ahora haga clic en **[!UICONTROL Agregar regla de columna]** para agregar otra regla.
1. Igual que antes, elimine [!UICONTROL Tarea] > [!UICONTROL Nombre] en el campo criterios. Sustitúyala por [!UICONTROL Estado de progreso] en el [!UICONTROL Tarea] origen del campo.
1. Seleccionar ambos [!UICONTROL En riesgo] y [!UICONTROL Rezagado] en el campo a la derecha del calificador Igual.
1. Elija un fondo de color amarillo en la [!UICONTROL Color del texto] fila.
1. Clic **[!UICONTROL Agregar regla]** para guardar la regla de columna.
1. Clic **[!UICONTROL Guardar vista]** para guardar la vista.
