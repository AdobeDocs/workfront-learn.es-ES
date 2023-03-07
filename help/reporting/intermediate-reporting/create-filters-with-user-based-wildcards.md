---
title: Creación de filtros con comodines basados en usuarios
description: Obtenga información sobre cómo utilizar caracteres comodín basados en usuarios y cómo crear un filtro basado en el usuario que ha iniciado sesión.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Creación de filtros con comodines basados en usuarios

En este vídeo, aprenderá a hacer lo siguiente:

* Comprender por qué utilizar caracteres comodín
* Creación de un filtro con un comodín basado en usuario

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12)

>[!TIP]
>
>Utilice el origen y el nombre del campo Usuarios de asignación >> Id. al crear filtros que vean la información de asignación de tareas o problemas.  Esta opción busca todos los usuarios asignados a la tarea o al problema, no solo el &quot;propietario&quot; o el usuario asignado principal.

>[!TIP]
>
>Utilice $$USER.ID (en lugar de su nombre) incluso cuando genere filtros para usted mismo. De este modo, si alguien ve un filtro que está ejecutando y dice &quot;compártalo conmigo&quot;, el filtro ya está configurado para que cada persona que lo utilice vea su propia información.

>[!TIP]
>
>Siempre debe utilizar el calificador de filtro Igual cuando utilice comodines basados en usuarios.

## Actividad

Tiene un poco de tiempo adicional esta semana, por lo que desea ver si hay alguien en su equipo que pueda utilizar alguna ayuda con sus asignaciones. Cree un filtro de tareas para buscar tareas que vencen esta semana y que no se hayan completado.

## Respuesta

¡Eres increíble por ayudar a tus compañeros de equipo! Con el filtro configurado como la imagen siguiente, encontrará tareas:

* Que no se han completado (lo que significa que no tienen un [!UICONTROL Completar] estado o estado que equivale a [!UICONTROL Completar]);
* Que están en proyectos con un [!UICONTROL Actual] estado (después de todo, no desea encontrar tareas para proyectos que aún no se hayan iniciado);
* Que se asignan a alguien de su equipo de inicio, según la configuración del equipo de Workfront;
* Y que tienen una fecha de finalización en algún momento de esta semana (esta regla utilizó el filtro de fecha generado previamente para definir &quot;esta semana&quot;).

![Imagen de la pantalla para crear un filtro de tareas con un comodín basado en el usuario](assets/user-wildcard-exercise-answer.png)

Es posible que tenga que añadir algunos filtros adicionales si necesita limitar la lista un poco más. Por ejemplo, es posible que desee agregar una regla de filtro que examine un programa o portafolio específico del que su equipo trabaje.
