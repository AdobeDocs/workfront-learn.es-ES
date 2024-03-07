---
title: Explicación de la navegación y revisión de proyectos
description: Obtenga información sobre cómo leer el gráfico del plan de grupo en [!UICONTROL Análisis mejorado].
activity: use
feature: Reports and Dashboards
thumbnail: 335047.png
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8729
recommendations: noDisplay,noCatalog
exl-id: 1409a1af-3bdb-40f7-af01-f9de2357b602
doc-type: video
source-git-commit: d29054f0551a9add8460e4c9fd265cee2dfb72ca
workflow-type: ht
source-wordcount: '459'
ht-degree: 100%

---

# Explicación de la navegación y revisión de proyectos

Este vídeo contiene información sobre:

* Cómo leer el gráfico del plan de grupo

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12&learn=on)

## Gráfico del plan de grupo

![Imagen de un gráfico del plan de grupo con números que coinciden con las viñetas siguientes](assets/section-2-1.png)

En el gráfico, verá lo siguiente:

1. Los nombres de los proyectos están a la izquierda.
1. Las fechas se muestran en la parte inferior.
1. La línea vertical azul muestra la fecha específica en la que se pasa el ratón sobre ella.
1. Las líneas azules horizontales muestran las fechas de inicio y finalización planificadas del proyecto.
1. Las líneas verdes indican que el proyecto está en el destino.
1. Las líneas naranja indican que el proyecto está en riesgo.
1. Las líneas rojas indican que el proyecto tiene problemas.

Al visualizar esta información sobre sus proyectos, podrá determinar lo siguiente:

* Los eventos que desencadenan que un proyecto se extienda más allá de la fecha planificada de finalización.
* Cuándo un proyecto empieza a tener problemas.
* Cuántos proyectos están abiertos durante el mismo período de tiempo.
* Cuántos proyectos están activos.
* Qué proyectos necesitan atención o apoyo extra.

## La condición se basa en el estado de progreso

La condición del proyecto es una representación visual del progreso del proyecto. Workfront determina la condición en función del estado de progreso de las tareas dentro del proyecto.

![Una imagen de los posibles estados de progreso](assets/section-2-2.png)

La condición de un proyecto se puede establecer de la siguiente manera:

* **Manualmente**, por parte de los usuarios con acceso para administrar el proyecto, cuando el tipo de condición del proyecto se establece en manual. Esto permite establecer la condición del proyecto de forma independiente de la ruta crítica.
* **Automáticamente**, por parte de Workfront, cuando el tipo de condición del proyecto se establece en Estado de progreso.

Workfront recomienda establecer el tipo de condición en Estado de progreso para que tenga una indicación clara del progreso real del proyecto, en función del progreso de las tareas.

![Imagen de los posibles estados de progreso](assets/section-2-3.png)

Cuando se establece en Estado de progreso, la condición del proyecto puede ser:

* **En el destino**: cuando el estado del progreso de la última tarea de la ruta crítica es el de A tiempo, la condición del proyecto estará En el destino. El proyecto está en vías de finalizar según lo programado.
* **En riesgo**: cuando el estado de progreso de la última tarea en la ruta crítica está Detrás o En riesgo, la condición del proyecto está En riesgo. El proyecto está en vías de finalizar tarde, pero aún no es tarde.
* **Con problemas**: cuando el estado de progreso de la última tarea de la ruta crítica es Tarde, la condición del proyecto es Con problemas. La fecha de entrega ya ha pasado y el proyecto lleva retraso.

>[!NOTE]
>
>Las condiciones se pueden personalizar para su entorno, por lo que puede encontrar más de tres opciones o los nombres pueden ser diferentes a los anteriores. Para obtener información sobre las condiciones de personalización, consulte el artículo [Crear o editar una condición personalizada](https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-conditions/create-edit-custom-conditions.html?lang=es).
