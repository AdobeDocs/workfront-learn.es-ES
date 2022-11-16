---
title: Crear filtros con comodines basados en datos
description: Aprenda cómo y cuándo utilizar los comodines basados en datos y cómo crear un filtro basado en la fecha actual.
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Crear filtros con comodines basados en datos

En este vídeo, aprenderá a:

* Saber cuándo usar comodines basados en datos
* Comprender la diferencia entre los dos comodines basados en datos de Workfront
* Añadir un comodín basado en datos a un filtro
* Crear una fecha personalizada utilizando caracteres comodín, atributos, operadores y modificadores
* Crear un intervalo de fechas personalizado con caracteres comodín

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12)

## Preguntas sobre actividades

1. ¿Cómo crearía la regla de filtro si quisiera problemas que tengan una fecha de vencimiento de ayer o de hoy?
1. ¿Cómo crearía la regla de filtro para encontrar proyectos que vencen la semana pasada?
1. Las siguientes reglas de filtro son parte de un informe de tareas que utiliza con regularidad. ¿Qué tipo de resultados obtendría de este informe?

![Una imagen de la pantalla para crear un filtro de tareas con un comodín basado en datos](assets/date-wildcard-answer-1.png)

## Respuestas

1. Filtre la fecha de finalización planeada del problema entre [!UICONTROL $$TODAY-1d] y [!UICONTROL $$HOY].
1. Filtre la fecha de finalización planeada para el proyecto entre [!UICONTROL $$HOYb-1w] y [!UICONTROL $$TODAYe-1w].
1. Este informe encuentra tareas asignadas que aún no han finalizado (es decir, que tienen un porcentaje completado inferior a 100) y que deberían haberse realizado o que vencen hoy. La regla de filtro para la fecha de finalización prevista de las tareas indica que se deben observar las tareas que tienen una fecha de vencimiento igual o anterior a la fecha actual.
