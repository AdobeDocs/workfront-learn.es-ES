---
title: Crear y compartir un formulario personalizado
description: Obtenga información sobre cómo crear un formulario personalizado, agregar campos únicos al formulario, organizar campos mediante secciones y lógica y compartir formularios con los usuarios.
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
thumbnail: 335172.png
jira: KT-8909
exl-id: b37334c7-67d0-4359-9537-dc26843582d1
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 100%

---

# Crear y compartir un formulario personalizado

Este vídeo contiene información sobre:

* Determinar qué objetos utilizar para el formulario
* Añadir campos únicos en una gran variedad de formatos
* Organizar campos mediante secciones y lógica
* Compartir formularios con otros usuarios

>[!VIDEO](https://video.tv.adobe.com/v/335172/?quality=12&learn=on)

## Los formularios personalizados funcionan con varios tipos de objetos

Al hacer clic en el botón [!UICONTROL Nuevo formulario personalizado], puede seleccionar tantos objetos como desee utilizar con un único formulario personalizado. Todos los campos que agregue a este formulario estarán disponibles para cualquiera de los objetos seleccionados cuando el formulario personalizado esté adjunto a ellos.

![La ventana de formulario personalizado muestra las opciones del objeto [!UICONTROL Nuevo formulario personalizado] ](assets/create-custom-form.png)

Al editar un formulario personalizado, puede ver todos los tipos de objeto seleccionados. Puede agregar o eliminar los tipos de objetos de esta lista.

![Ventana de formulario personalizado que muestra los tipos de objeto seleccionados durante la edición del formulario](assets/edit-custom-form.png)

Es posible que desee crear una forma personalizada de tipo de proyecto y problema. Cuando se adjunta a un problema, puede rellenar cualquiera de los campos relacionados con el problema. Posteriormente, si decide convertir el problema en un proyecto, el formulario personalizado se cargará automáticamente en el proyecto y los datos que introduzca en los campos del formulario personalizado del problema estarán disponibles para su visualización o edición en el formulario personalizado del proyecto.

## Opciones de campos personalizados

Campos **[!UICONTROL Etiqueta] y [!UICONTROL Nombre]**

Los campos [!UICONTROL Etiqueta] y [!UICONTROL Nombre] de un campo personalizado tienen diferentes propósitos. [!UICONTROL Etiqueta] es el nombre del campo que verán los usuarios en [!DNL Workfront]. [!UICONTROL Nombre] es lo que se puede usar con integraciones como API.

![La ventana del formulario personalizado muestra los campos [!UICONTROL Etiqueta] y [!UICONTROL Nombre] ](assets/custom-forms-field-label-and-name.png)

Esto proporciona la flexibilidad para cambiar la etiqueta de cara al usuario para que coincida con los cambios en su organización, sin afectar a las integraciones u otras conexiones que dependen de un nombre de campo específico.

**[!UICONTROL Campo de texto con formato]**

La variable [!UICONTROL Campo de texto con formato ]contiene herramientas básicas de marcado de texto que permiten a los usuarios agregar negrita, cursiva o subrayado al texto mientras rellenan el campo en un formulario personalizado.

![La ventana de formulario personalizado muestra la opción [!UICONTROL Campo de texto con formato] ](assets/custom-forms-text-field-with-formatting.png)

El campo también tiene un límite de 15.000 caracteres, lo que permite disponer de mucho espacio para proporcionar información vital y utilizar formato para facilitar la lectura por parte de los demás.

Campo **[!UICONTROL TypeAhead]**

El campo [!UICONTROL TypeAhead] permite que el sistema rellene automáticamente una lista de opciones en función del objeto seleccionado para el campo.

![La ventana de formulario personalizado muestra la opción de campo [!UICONTROL TypeAhead] ](assets/custom-forms-typeahead-1.png)

Por ejemplo, si crea un campo denominado [!UICONTROL TypeAhead] “Nombre de aprobación del administrador de marketing” y selecciona [!UICONTROL Usuario] como tipo de objeto al que se hace referencia, aparece una lista de nombres de usuario cuando un usuario rellena ese campo en un formulario personalizado. El campo [!UICONTROL TypeAhead] está diseñado para conectar los datos personalizados con información capturada en el sistema. Elimina la necesidad de mantener manualmente muchas opciones en los campos desplegables.

![La ventana de formulario personalizado muestra el menú desplegable [!UICONTROL TypeAhead] ](assets/custom-forms-typeahead-2.png)
