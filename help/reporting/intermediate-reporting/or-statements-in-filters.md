---
title: Crear instrucciones OR en filtros
description: La lógica de filtro flexible de Workfront permite a los usuarios refinar las vistas de creación de informes utilizando reglas predeterminadas "Y", condiciones opcionales "O" y grupos de filtros organizados para criterios complejos.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: '2025-08-11T00:00:00.000Z'
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: c6dd2ac5-f5bd-4e59-9101-25b156918623
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-06T02:11:54.379Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 318
ht-degree: 31%

---

# Crear instrucciones OR en filtros

En el vídeo se explica cómo crear y utilizar filtros con varias reglas en Workfront. De forma predeterminada, Workfront utiliza &quot;Y&quot; entre las reglas de filtro, lo que significa que todas las condiciones deben ser verdaderas para que un elemento aparezca en la lista.
También puede cambiar la lógica del filtro a &quot;O&quot;, que muestra los elementos que cumplen cualquiera de las condiciones.
El vídeo también muestra la creación de filtros para tareas utilizando grupos de filtros. Por ejemplo, puede crear dos grupos: uno para tareas incompletas asignadas al equipo creativo que están atrasadas y otro para tareas incompletas asignadas al equipo creativo que no están asignadas. Dentro de cada grupo, se aplica la lógica &quot;AND&quot;, lo que significa que se deben cumplir todas las condiciones del grupo. La lógica &quot;OR&quot; entre grupos garantiza que se muestren las tareas que cumplen las condiciones de cualquiera de los grupos.

>[!VIDEO](https://video.tv.adobe.com/v/3470692/?quality=12&learn=on&enablevpops=0)

## Actividad de filtro O

Desea encontrar tareas incompletas que están asignadas a usted o que no están asignadas a nadie. Configure un filtro de modo que se asemeje al que se muestra a continuación. ¿Le dará este filtro los resultados que desea? ¿Por qué sí o por qué no?

![Una imagen de una instrucción O creada incorrectamente en [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Respuestas

No, este filtro no proporcionará los resultados esperados (tareas que no han finalizado y que no se le han asignado a usted o que no se le han asignado a nadie) porque la regla de filtrado para la integridad de la tarea solo está a un lado del operador OR.

En su lugar, este filtro genera una lista que muestra:

* Tareas asignadas que no se han completado.
* **MÁS (O)**
* Todas las tareas no asignadas, independientemente del estado.

El filtro debe ser similar al que se muestra a continuación. Observe que este filtro tiene la regla de filtro para la integridad de las tareas en ambos lados del operador OR.

![Una imagen de una instrucción O creada correctamente en [!DNL Workfront]](assets/or-statement-your-turn-2.png)
