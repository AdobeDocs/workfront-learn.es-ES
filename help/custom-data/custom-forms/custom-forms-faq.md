---
title: Respuestas a preguntas sobre Forms personalizado
description: Obtenga respuestas a preguntas comunes sobre formularios personalizados.
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
kt: 10058
source-git-commit: 7cdce710ecc6fbcdccfe147a40623dc96f07ed2c
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 1%

---

# Preguntas frecuentes sobre formularios personalizados

**¿Puedo cambiar el tipo de visualización de un campo después de haberlo creado? Por ejemplo, ¿puedo cambiar de un menú desplegable a casillas de verificación?**

Sí. El tipo de visualización puede cambiarse a otro tipo de visualización similar: texto a párrafo, menú desplegable a casillas de verificación o botones de opción, etc. Para obtener más información sobre cómo cambiar el tipo de visualización, consulte el artículo Crear un formulario personalizado .


**¿Puedo utilizar el mismo formulario personalizado para varios objetos? Por ejemplo, ¿un formulario que he creado para una tarea en un proyecto?**

No. Los formularios personalizados tienen una relación &quot;uno a uno&quot; con un objeto. Sin embargo, puede copiar el formulario personalizado y cambiar el objeto por el que sea necesario.


**¿Se puede adjuntar un formulario personalizado a una plantilla de proyecto?**

Sí. De este modo, cualquier proyecto creado a partir de esa plantilla tendrá ya adjunto el formulario personalizado.


**¿Hay un límite en el número de campos que puedo tener en un formulario personalizado?**

Puede agregar hasta 500 campos en un único formulario personalizado. Sin embargo, puede producirse una degradación del rendimiento cuando existen más de 100 campos en un formulario, según la complejidad del formulario personalizado. Algunos ejemplos de formularios complejos son los formularios con parámetros en cascada, campos de datos personalizados calculados y varias opciones de valor en un campo determinado.


**¿Hay un límite en el número de formularios personalizados que puedo adjuntar a un proyecto?**

Sí. Puede adjuntar hasta 10 formularios personalizados en un objeto. Para obtener más información, consulte este artículo Aplicación de Forms personalizado a objetos .


**¿Se puede desactivar un formulario personalizado?**

Sí. En la ficha Configuración del formulario del formulario personalizado, desactive la casilla Es activo . De este modo, se quita el formulario personalizado de cualquier menú desplegable de Workfront. Sin embargo, si el formulario personalizado ya está adjunto a un proyecto, el formulario permanece y conserva los datos ya introducidos.