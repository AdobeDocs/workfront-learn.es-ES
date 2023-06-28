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
ht-degree: 5%

---

# Crear y compartir un formulario personalizado

En este vídeo, aprenderá a hacer lo siguiente:

* Determinar qué objetos utilizar para el formulario
* Añadir campos únicos en una variedad de formatos
* Organizar campos mediante secciones y lógica
* Compartir formularios con otros usuarios

>[!VIDEO](https://video.tv.adobe.com/v/335172/?quality=12&learn=on)

## Los formularios personalizados funcionan con varios tipos de objetos

Al hacer clic en [!UICONTROL Nuevo formulario personalizado] botón, puede seleccionar tantos objetos como desee utilizar con un solo formulario personalizado. Todos los campos que agregue a este formulario estarán disponibles para cualquiera de los objetos seleccionados cuando el formulario personalizado esté adjunto a ellos.

![Ventana de formulario personalizado que muestra [!UICONTROL Nuevo formulario personalizado] opciones de objeto](assets/create-custom-form.png)

Al editar un formulario personalizado, puede ver todos los tipos de objetos seleccionados. Puede agregar o eliminar tipos de objetos de esta lista.

![Ventana de formulario personalizada que muestra los tipos de objeto seleccionados durante la edición del formulario](assets/edit-custom-form.png)

Es posible que desee crear una forma personalizada de tipo proyecto y problema. Cuando se adjunta a un problema, puede rellenar cualquiera de los campos relacionados con el problema. Posteriormente, si decide convertir el problema en un proyecto, el formulario personalizado se cargará automáticamente en el proyecto y los datos introducidos en los campos del formulario personalizado del problema estarán disponibles para su visualización o edición en el formulario personalizado del proyecto.

## Opciones de campo personalizado

**[!UICONTROL Etiqueta] y [!UICONTROL Nombre] campos**

El [!UICONTROL Etiqueta] y [!UICONTROL Nombre] los campos de un campo personalizado tienen diferentes propósitos. [!UICONTROL Etiqueta] es el nombre de campo que verán los usuarios en [!DNL Workfront]. [!UICONTROL Nombre] es lo que se puede utilizar con integraciones de, como API.

![Ventana de formulario personalizado que muestra [!UICONTROL Etiqueta] y [!UICONTROL Nombre] campos](assets/custom-forms-field-label-and-name.png)

Esto proporciona la flexibilidad para cambiar la etiqueta orientada al usuario de modo que coincida con los cambios en la organización, sin afectar a las integraciones u otras conexiones que dependen de un nombre de campo específico.

**[!UICONTROL Campo de texto con formato]**

El [!UICONTROL Campo de texto con formato]contiene herramientas básicas de marcado de texto que permiten a los usuarios agregar negrita, cursiva o subrayado en el texto mientras rellenan el campo de un formulario personalizado.

![Ventana de formulario personalizado que muestra [!UICONTROL Campo de texto con formato] opción](assets/custom-forms-text-field-with-formatting.png)

El campo también tiene un límite de 15 000 caracteres, lo que permite disponer de mucho espacio para proporcionar información esencial y utilizar el formato para facilitar la lectura a los demás.

**[!UICONTROL Escritura anticipada] campo**

El [!UICONTROL Escritura anticipada] permite al sistema rellenar automáticamente una lista de opciones basadas en el objeto seleccionado para el campo.

![Ventana de formulario personalizado que muestra [!UICONTROL Escritura anticipada] opción de campo](assets/custom-forms-typeahead-1.png)

Por ejemplo, si crea un [!UICONTROL Escritura anticipada] Campo denominado &quot;Nombre de aprobación del responsable de marketing&quot; y seleccione [!UICONTROL Usuario] como tipo de objeto referenciado, aparece una lista de nombres de usuario cuando un usuario rellena ese campo en un formulario personalizado. El [!UICONTROL Escritura anticipada] El objetivo del campo es conectar los datos personalizados con la información capturada en el sistema y eliminar la necesidad de mantener manualmente muchas opciones en los campos desplegables.

![Ventana de formulario personalizado que muestra [!UICONTROL Escritura anticipada] menú desplegable](assets/custom-forms-typeahead-2.png)
