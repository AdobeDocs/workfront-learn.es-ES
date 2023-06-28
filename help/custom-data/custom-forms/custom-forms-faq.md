---
title: Respuestas a preguntas sobre Custom Forms
description: Obtenga respuestas a preguntas comunes sobre formularios personalizados.
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
jira: KT-10058
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 1%

---

# Preguntas comunes sobre los formularios personalizados

**¿Puedo cambiar el tipo de visualización de un campo después de crearlo? Por ejemplo, ¿puedo cambiar de un menú desplegable a casillas de verificación?**

Sí. El tipo de visualización se puede cambiar a otro tipo de visualización similar: texto a párrafo, menú desplegable a casillas de verificación o botones de opción, etc. Para obtener más información sobre cómo cambiar el tipo de visualización, consulte el artículo Crear un formulario personalizado.


**¿Puedo utilizar el mismo formulario personalizado para varios objetos? Por ejemplo, ¿un formulario que he creado para una tarea a un proyecto?**

No. Los formularios personalizados tienen una relación uno a uno con un objeto. Sin embargo, puede copiar el formulario personalizado y cambiar el objeto por el que necesite.


**¿Se puede adjuntar un formulario personalizado a una plantilla de proyecto?**

Sí. De este modo, cualquier proyecto creado a partir de esa plantilla ya tendrá adjunto el formulario personalizado.


**¿Hay un límite en el número de campos que puedo tener en un formulario personalizado?**

Puede agregar hasta 500 campos en un solo formulario personalizado. Sin embargo, puede producirse una degradación del rendimiento cuando existen más de 100 campos en un formulario, según la complejidad del formulario personalizado. Algunos ejemplos de formularios complejos son los formularios con parámetros en cascada, los campos de datos personalizados calculados y las opciones de varios valores de un campo determinado.


**¿Hay un límite en el número de formularios personalizados que puedo adjuntar a un proyecto?**

Sí. Puede adjuntar hasta 10 formularios personalizados a un objeto. Para obtener más información, consulte este artículo, Aplicar Forms personalizado a objetos.


**¿Puedo desactivar un formulario personalizado?**

Sí. En la pestaña Configuración de formulario del formulario personalizado, desactive la casilla Está activo. Esto quita el formulario personalizado de cualquier menú desplegable en Workfront. Sin embargo, si el formulario personalizado ya está adjunto a un proyecto, permanecerá y conservará los datos ya introducidos.