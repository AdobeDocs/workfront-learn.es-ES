---
title: Crear filtros con comodines basados en el usuario
description: Aprenda a utilizar comodines basados en el usuario y a crear un filtro basado en el usuario que ha iniciado sesión.
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Crear filtros con comodines basados en el usuario

En este vídeo, aprenderá a:

* Comprender por qué utilizar caracteres comodín
* Genere un filtro con un comodín basado en el usuario

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12)

>[!TIP]
>
>Utilice el nombre y la fuente del campo de asignación Usuarios >> ID al crear filtros que miren la información de asignación de tareas o problemas.  Esta opción busca todos los usuarios asignados a la tarea o el problema, no solo el &quot;propietario&quot; o el usuario asignado principal.

>[!TIP]
>
>Utilice $$USER.ID (en lugar de su nombre) incluso cuando cree filtros para usted mismo. De esta manera, si alguien ve un filtro que está ejecutando y dice &quot;compartir eso conmigo&quot;, el filtro ya está configurado para que cada persona que lo utiliza vea su propia información.

>[!TIP]
>
>Siempre debe utilizar el calificador de filtro Igual al utilizar caracteres comodín basados en el usuario.

## Actividad

Esta semana tiene un poco de tiempo adicional, por lo que desea ver si hay alguien en su equipo que pueda utilizar algún tipo de asistencia con sus asignaciones. Cree un filtro de tareas para encontrar tareas que vencen esta semana y que no se han completado.

## Respuesta

¡Eres genial por ayudar a tus compañeros de equipo! Con el filtro configurado como la imagen siguiente, encontrará tareas:

* No se han completado (lo que significa que no tienen un [!UICONTROL Completar] estado o estado igual a [!UICONTROL Completar]);
* que están en proyectos con un [!UICONTROL Actual] estado (después de todo, no desea encontrar tareas para proyectos que aún no se han iniciado);
* que se asignan a alguien del equipo de casa, tal como se define en la configuración del equipo de Workfront;
* Y que tienen una fecha de finalización en algún momento de esta semana (esta regla usaba el filtro de fechas precompilado para definir &quot;esta semana&quot;).

![Una imagen de la pantalla para crear un filtro de tareas con un comodín basado en el usuario](assets/user-wildcard-exercise-answer.png)

Es posible que necesite añadir algunos filtros adicionales si necesita limitar la lista un poco más. Por ejemplo, puede que desee agregar una regla de filtro que observe un programa o portafolio específico en el que su equipo trabaja.
