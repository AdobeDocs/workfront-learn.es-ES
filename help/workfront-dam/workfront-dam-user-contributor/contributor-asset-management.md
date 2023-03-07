---
title: Obtenga información sobre cómo administrar recursos en [!UICONTROL WORKFRONT DAM]
description: Obtenga información sobre cómo administrar recursos en [!UICONTROL WORKFRONT DAM] para mejorar el flujo de trabajo.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Colaborador: administración de recursos

En este vídeo, aprenderá a hacer lo siguiente:

* Usar el menú Edición en un recurso
* Establecer una fecha de caducidad
* Ver notificaciones
* Establecer la configuración de notificaciones individuales
* Cargar una versión del recurso
* Crear una carpeta nueva
* Aplicar una plantilla de metadatos a una carpeta
* Establecer permisos de carpeta

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12)

## Funcionamiento de las versiones de recursos

Parte del flujo de trabajo puede incluir la administración de varias versiones (o rondas, pruebas, iteraciones, como las llame) de un recurso. Puede administrar todas las versiones a través de [!UICONTROL WORKFRONT DAM].

El sistema permite controlar automáticamente las versiones de los recursos cuando se carga un archivo con el mismo nombre que uno existente en la misma carpeta. Consulte con el administrador del sistema si esta funcionalidad está activada.

Si el control de versiones automático está activado, la versión de un recurso solo se eliminará si se ha cargado en la carpeta que contiene el recurso original. Ambos recursos deben tener el mismo nombre de archivo. Si el recurso se carga en una carpeta diferente, entra como un archivo nuevo.
Si el control de versiones no está activado, se carga un archivo con el mismo nombre que un archivo existente como un archivo nuevo, independientemente de la carpeta en la que se coloque. Esto podría dar como resultado dos recursos con el mismo nombre en la misma carpeta.

También puede cargar manualmente versiones de un recurso específico. Haga clic en el icono de edición en el recurso y seleccione **[!UICONTROL Cargar nueva versión]**.

Si publica un recurso con versiones en Brand Connect, el usuario de Brand Connect solo verá la versión más reciente del recurso.

## Estado y caducidad de la carpeta y el recurso

Los estados son otra forma de administrar el acceso a carpetas y recursos en [!UICONTROL WORKFRONT DAM]. Los estados se pueden usar para ocultar ciertos recursos o carpetas de [!UICONTROL Brand Connect] o para que caduque un recurso o una carpeta de modo que nadie, excepto el administrador del sistema, pueda acceder a ellos.

* **[!UICONTROL Activo]**: se utiliza para recursos y carpetas. Recursos y carpetas con [!UICONTROL Activo] Los estados son visibles para todos los usuarios con permisos y se pueden publicar en [!UICONTROL Brand Connect]. [!UICONTROL Activo] se indica con un punto verde en un recurso o carpeta.
* **[!UICONTROL Inactivo]**: se utiliza para recursos y carpetas. Recursos y carpetas con [!UICONTROL Inactivo] estados visibles para [!UICONTROL WORKFRONT DAM] usuarios, pero no son visibles en el [!UICONTROL Brand Connect]. [!UICONTROL Inactivo] se indica con un punto rojo en un recurso o carpeta.
* **[!UICONTROL Sin Caducar]**: se utiliza solo para recursos. Este es el estado predeterminado de todos los recursos. Recursos no caducados que también son [!UICONTROL Activo] son visibles en la [!UICONTROL Brand Connect].
* **[!UICONTROL Caducado]**: se utiliza solo para recursos. Recursos con el [!UICONTROL Caducado] ningún usuario puede descargar el estado, excepto el administrador del sistema. Los recursos caducados son visibles o no son visibles en la [!UICONTROL Brand Connect], según las configuraciones del sistema.
