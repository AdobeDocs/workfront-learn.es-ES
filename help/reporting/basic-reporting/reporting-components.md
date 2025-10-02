---
title: Información sobre los componentes del sistema de informes
description: Los componentes de informes de Workfront refinan la visualización de datos con filtros basados en objetos, vistas dinámicas, agrupaciones estructuradas y la funcionalidad de comodín para obtener perspectivas adaptadas.
activity: use
feature: Reports and Dashboards
thumbnail: 335146.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8850
last-substantial-update: 2025-04-28T00:00:00Z
exl-id: e9f9ba24-540f-49e1-ac52-740df489317b
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 42%

---

# Información sobre los componentes del sistema de informes

En el vídeo se explica el concepto de los componentes de creación de informes en Workfront, que son esenciales para crear filtros, vistas y agrupaciones. Los componentes clave incluyen:

* **Tipo de objeto:** Especifica el objeto de Workfront que se está tratando, como un proyecto, una tarea o una entrada de hora. palo de golf Los filtros, las vistas y las agrupaciones son específicos del tipo de objeto. palo de golf
* **Source de campo y Nombre de campo:** El origen de campo es el elemento de Workfront donde se adjunta información y el nombre de campo es la información específica (por ejemplo, &quot;descripción&quot; de un proyecto). palo de golf
* **Campo de valor:** Representa el contenido de un campo, como &quot;bajo&quot;, &quot;normal&quot;, &quot;alto&quot; o &quot;urgente&quot; para el campo de prioridad. palo de golf
* **Calificador de filtro:** Define qué valores incluir o excluir en un informe, como mostrar tareas con una prioridad &quot;alta&quot;.


>[!VIDEO](https://video.tv.adobe.com/v/335146/?quality=12&amp;learn=on&amp;enablevpops=0

## Puntos clave

* **Componentes de informes:** Los componentes de informes de Workfront incluyen el tipo de objeto, el origen del campo, el nombre del campo, los calificadores de filtro y el campo de valor, que son esenciales para crear filtros, vistas y agrupaciones. palo de golf
* **Especificidad del tipo de objeto:** Los filtros, las vistas y las agrupaciones están vinculados a tipos de objetos específicos, como proyectos, tareas o entradas de horas, lo que garantiza que los informes se adapten a los datos relevantes. palo de golf
* **Reglas de filtro:** Los filtros utilizan el origen del campo, el nombre del campo, los calificadores y los valores para definir los criterios. palo de golf Por ejemplo, el filtro &quot;Mis proyectos&quot; muestra solo los proyectos actuales en los que el usuario que ha iniciado sesión forma parte del equipo del proyecto. palo de golf
* **Vistas y agrupaciones:** Las vistas muestran combinaciones de origen de campo y nombre de campo en columnas (por ejemplo, &quot;nombre de propietario&quot;), mientras que las agrupaciones organizan los datos según criterios específicos (por ejemplo, &quot;nombre de empresa&quot;).
* **Uso de caracteres comodín:** Los caracteres comodín de los filtros permiten la coincidencia dinámica, como la identificación de usuarios que iniciaron sesión en un equipo de proyecto y la mejora de la personalización en los informes. palo de golf

## Referencia rápida de los componentes de informes

![Una imagen de la pantalla para crear un filtro](assets/reporting-components-1.png)

**A - Origen del campo**

Las opciones de origen del campo dependen del tipo de objeto seleccionado. A menudo, el origen del campo es el elemento de Workfront al que pertenece un fragmento de información específico (también conocido como nombre de campo). A veces, el origen del campo es el mismo que el tipo de objeto.
El origen del campo determina qué nombres de campo están disponibles.

Ejemplos: [!UICONTROL Proyecto], [!UICONTROL Tarea], [!UICONTROL Problema], [!UICONTROL Asignado a]

**B - Nombre del campo**

Los nombres de campo son fragmentos de información disponible sobre lo que ha seleccionado como origen de campo.

Pueden ser campos de Workfront que haya rellenado, campos de un formulario personalizado o información que Workfront capture automáticamente.

Los nombres de campo dirigen las opciones de campo de valor.

Ejemplos: [!UICONTROL Estado de progreso], [!UICONTROL Descripción], [!UICONTROL Fecha planificada de finalización], Campos de formulario personalizados

**C - Calificadores de filtro**

Los calificadores de filtro ayudan a reducir los posibles resultados visibles en el origen del campo y el nombre del campo seleccionado.

Especifican cómo se relacionan el origen del campo y el nombre del campo con el campo de valor.

Ejemplos: Igual, Contiene, Nulo, Menor que

**D - Valor**

El valor es la parte de información introducida en el campo especificado por el nombre del campo.

Las opciones de valor están determinadas por el origen del campo y el nombre del campo.

En el valor se pueden utilizar caracteres comodín para usuarios y fechas, así como texto de forma libre.

Ejemplos: Nuevo, Actual, $$TODAYbw, Descripción

>[!TIP]
>
>Para obtener ayuda sobre los nombres de campo específicos en Workfront, consulte en el [Glosario de terminología de Adobe Workfront](https://experienceleague.adobe.com/docs/workfront/using/basics/workfront-terminology-glossary.html?lang=es).

