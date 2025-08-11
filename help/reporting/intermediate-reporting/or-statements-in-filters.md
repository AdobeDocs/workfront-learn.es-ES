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
last-substantial-update: 2025-08-11T00:00:00Z
doc-type: video
source-git-commit: b3cff8f86ceeb6e79e2b88ab335b2671aa25600a
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 31%

---

# Crear instrucciones OR en filtros

En el vídeo se explica cómo crear y utilizar filtros con varias reglas en Workfront. palo de golf De forma predeterminada, Workfront utiliza &quot;Y&quot; entre reglas de filtro, lo que significa que todas las condiciones deben ser verdaderas para que un elemento aparezca en la lista.
También puede cambiar la lógica del filtro a &quot;O&quot;, que muestra los elementos que cumplen cualquiera de las condiciones.
El vídeo también muestra la creación de filtros para tareas utilizando grupos de filtros. palo de golf Por ejemplo, puede crear dos grupos: uno para las tareas incompletas asignadas al equipo creativo que están atrasadas y otro para las tareas incompletas asignadas al equipo creativo que no están asignadas. palo de golf Dentro de cada grupo se aplica la lógica &quot;Y&quot;, lo que significa que deben cumplirse todas las condiciones del grupo. palo de golf La lógica &quot;OR&quot; entre grupos garantiza que se muestren las tareas que cumplen las condiciones de cualquiera de los grupos.

>[!VIDEO](https://video.tv.adobe.com/v/3470696/?quality=12&learn=on&captions=spa)

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
