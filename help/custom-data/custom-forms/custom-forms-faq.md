---
title: Respuestas a preguntas sobre los Formularios personalizados
description: Obtener respuestas a preguntas comunes sobre formularios personalizados.
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
jira: KT-10058
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 88%
---
# Preguntas frecuentes sobre formularios personalizados

**¿Puedo cambiar el tipo de visualización de un campo después de haberlo creado? Por ejemplo, ¿puedo cambiar de un menú desplegable a casillas de verificación?**

Sí. El tipo de visualización se puede cambiar a otro tipo de visualización similar: texto a párrafo, menú desplegable a casillas de verificación o botones de opción, etc. Para obtener más información sobre cómo cambiar el tipo de visualización, consulte el artículo Crear un formulario personalizado.


**¿Puedo utilizar el mismo formulario personalizado para varios objetos? Por ejemplo, ¿un formulario que he creado para una tarea en un proyecto?**

No. Los formularios personalizados tienen una relación personalizada con un objeto. Sin embargo, puede copiar el formulario personalizado y cambiar el objeto por el que sea necesario.


**¿Se puede adjuntar un formulario personalizado a una plantilla de proyecto?**

Sí. De este modo, cualquier proyecto creado a partir de esa plantilla tendrá ya adjunto el formulario personalizado.


**¿Hay un límite en el número de campos que puedo tener en un formulario personalizado?**

Puede agregar hasta 500 campos en un único formulario personalizado. Sin embargo, puede producirse una degradación del rendimiento cuando existan más de 100 campos en un formulario, según la complejidad del formulario personalizado. Algunos ejemplos de formularios complejos son los formularios con parámetros en cascada, campos de datos personalizados calculados y varias opciones de valor en un campo determinado.


**¿Hay un límite en el número de formularios personalizados que pueda adjuntar a un proyecto?**

Sí. Puede adjuntar hasta 10 formularios personalizados en un objeto. Para obtener más información, consulte el artículo de Aplicar Formularios personalizados a objetos.


**¿Se puede desactivar un formulario personalizado?**

Sí. En la pestaña Configuración del formulario en el formulario personalizado, desactive la casilla Está activo. De este modo, se quita el formulario personalizado de cualquier menú desplegable de Workfront. Sin embargo, si el formulario personalizado ya está adjunto a un proyecto, el formulario se queda y conserva los datos ya introducidos.