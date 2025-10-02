---
title: Crear filtros con caracteres comodín basados en datos
description: Aprenda cómo y cuándo utilizar los caracteres comodín basados en datos y cómo crear un filtro basado en la fecha actual.
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-06-27T00:00:00Z
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
source-git-commit: 1fafcafb173ceb4115612e1c33ca36564c7a6c3d
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 70%

---

# Crear filtros con caracteres comodín basados en datos

Este vídeo contiene información sobre:

* Saber cuándo usar los caracteres comodín basados en datos
* Comprender la diferencia entre los dos comodines basados en fechas de Workfront
* Añadir un carácter comodín basado en datos a un filtro
* Crear una fecha personalizada utilizando caracteres comodín, atributos, operadores y modificadores
* Crear un intervalo de fechas personalizado con caracteres comodín

>[!VIDEO](https://video.tv.adobe.com/v/3412659/?quality=12&learn=on&captions=spa)


## Actividades &quot;Crear filtros con comodines basados en fecha&quot;


### Preguntas sobre actividades

1. ¿Cómo crearía la regla de filtro si quisiera los problemas cuya fecha de vencimiento fuera ayer u hoy?
1. ¿Cómo crearía la regla de filtro para encontrar proyectos que vencieron la semana pasada?
1. Las siguientes reglas de filtro son parte de un informe de tareas que utiliza con regularidad. ¿Qué tipo de resultados obtendría de este informe?

![Una imagen de la pantalla para crear un filtro de tareas con un carácter comodín basado en datos](assets/date-wildcard-answer-1.png)

### Respuestas

1. Filtre la fecha planificada de finalización del problema entre [!UICONTROL $$TODAY-1d] y [!UICONTROL $$TODAY].
1. Filtre la fecha planificada de finalización para el proyecto entre [!UICONTROL $$TODAYb-1w] y [!UICONTROL $$TODAYe-1w].
1. Este informe encuentra las tareas que se le han asignado y que aún no han finalizado (es decir, tienen un porcentaje completado inferior a 100) y que han vencido o que vencen en el día de hoy. La regla de filtro para la fecha planificada de finalización de las tareas indica que se deben ver las tareas que tienen una fecha de vencimiento igual o anterior a la fecha actual.
