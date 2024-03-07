---
title: Comprender la administración de recursos como colaborador
description: Obtenga información sobre cómo administrar recursos en [!UICONTROL DAM de Workfront] para mejorar el flujo de trabajo.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: 2cb3cc67f4f1fcd1345f178bf525d7b00f6271cf
workflow-type: ht
source-wordcount: '460'
ht-degree: 100%

---

# Comprender la administración de recursos como colaborador

Este vídeo contiene información sobre:

* Uso del menú Edición de un recurso
* Establecer una fecha de caducidad
* Ver notificaciones
* Establecer la configuración de notificaciones individuales
* Cargar una versión de un recurso
* Crear una nueva carpeta
* Aplicación de una plantilla de metadatos a una carpeta
* Establecer permisos de carpeta

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on)

## Funcionamiento de las versiones de los recursos

Una parte del flujo de trabajo puede incluir la administración de varias versiones (o rondas, pruebas, iteraciones, como se las llame) de un recurso. Puede administrar todas las versiones mediante [!UICONTROL DAM de Workfront].

El sistema permite el control automático de la versión de los recursos cuando se carga en la misma carpeta un archivo con el mismo nombre que un archivo existente. Consulte con el administrador del sistema para ver si esta funcionalidad se ha activado.

Si el control de versiones automático está activado, un recurso solo se convertirá en una versión si se carga en la carpeta que alberga el recurso original. Ambos recursos deben tener el mismo nombre de archivo. Si el recurso se carga en una carpeta diferente, el recurso se introduce como un archivo nuevo.
Si el control de versiones no está activado, un archivo con el mismo nombre que un archivo existente se carga como un archivo nuevo, independientemente de la carpeta en la que se coloque. Esto podría conllevar tener dos recursos con el mismo nombre en la misma carpeta.

También puede cargar manualmente versiones de un recurso específico. Haga clic en el icono de edición del recurso y, a continuación, seleccione **[!UICONTROL Cargar nueva versión]**.

Si publica un recurso con versiones para Brand Connect, el usuario de Brand Connect solo verá la última versión del recurso.

## Estado de la carpeta y del recurso y caducidad

Los estados son otra forma de administrar el acceso a carpetas y recursos en [!UICONTROL DAM de Workfront]. Los estados se pueden usar para ocultar ciertos recursos o carpetas de [!UICONTROL Brand Connect] o para que caduque un recurso o una carpeta, de modo que nadie, excepto el administrador del sistema, pueda acceder a él.

* **[!UICONTROL Activo]**: se utiliza para recursos y carpetas. Recursos y carpetas con el estado [!UICONTROL Activo] son visibles para todos los usuarios con permisos y se pueden publicar en [!UICONTROL Brand Connect]. [!UICONTROL Activo] se indica con un punto verde en un recurso o carpeta.
* **[!UICONTROL Inactivo]**: se utiliza para recursos y carpetas. Los recursos y carpetas con el estado [!UICONTROL Inactivo] son visibles para los usuarios de [!UICONTROL DAM de Workfront], pero no están visibles en [!UICONTROL Brand Connect]. [!UICONTROL Inactivo] se indica con un punto rojo en un recurso o carpeta.
* **[!UICONTROL Sin caducar]**: se utiliza solo para recursos. Este es el estado predeterminado de todos los recursos. Recursos no caducados que también están [!UICONTROL Activos] están visibles en [!UICONTROL Brand Connect].
* **[!UICONTROL Caducado]**: se utiliza solo para recursos. Los recursos con el estado [!UICONTROL Caducado] no pueden ser descargados por ningún usuario, excepto por el administrador del sistema. Los recursos caducados son visibles o no están visibles en [!UICONTROL Brand Connect], según las configuraciones del sistema.
