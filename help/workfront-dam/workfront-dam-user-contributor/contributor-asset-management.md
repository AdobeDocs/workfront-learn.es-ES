---
title: Obtenga información sobre cómo administrar recursos en [!UICONTROL DAM de Workfront]
description: Obtenga información sobre cómo administrar recursos en [!UICONTROL DAM de Workfront] para mejorar el flujo de trabajo.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Colaborador: administración de recursos

En este vídeo, aprenderá a:

* Uso del menú Edición de un recurso
* Establecer una fecha de caducidad
* Ver notificaciones
* Establecer la configuración de notificaciones individuales
* Cargar una versión de un recurso
* Crear una carpeta nueva
* Aplicación de una plantilla de metadatos a una carpeta
* Establecer permisos de carpeta

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12)

## Funcionamiento de las versiones de los recursos

Una parte del flujo de trabajo puede incluir la administración de varias versiones (o rondas, pruebas, iteraciones, como se las llame) de un recurso. Puede administrar todas las versiones mediante [!UICONTROL DAM de Workfront].

El sistema permite el control automático de la versión de los recursos cuando se carga en la misma carpeta un archivo con el mismo nombre que un archivo existente. Consulte con el administrador del sistema para ver si esta funcionalidad se ha activado.

Si el control de versiones automático está activado, un recurso solo se convertirá en una versión si se carga en la carpeta que alberga el recurso original. Ambos recursos deben tener el mismo nombre de archivo. Si el recurso se carga en una carpeta diferente, se introduce como un archivo nuevo.
Si el control de versiones no está activado, un archivo con el mismo nombre que un archivo existente se carga como un archivo nuevo, independientemente de la carpeta en la que se coloque. Esto podría conllevar tener dos recursos con el mismo nombre en la misma carpeta.

También puede cargar manualmente versiones de un recurso específico. Haga clic en el icono de edición del recurso y, a continuación, seleccione **[!UICONTROL Cargar nueva versión]**.

Si publica un recurso con versiones para Brand Connect, el usuario de Brand Connect solo verá la última versión del recurso.

## Estado de carpeta y recurso y caducidad

Los estados son otra forma de administrar el acceso a carpetas y recursos en [!UICONTROL DAM de Workfront]. Los estados se pueden usar para ocultar ciertos recursos o carpetas de [!UICONTROL Brand Connect] o para que caduque un recurso o una carpeta, de modo que nadie, excepto el administrador del sistema, pueda acceder a él.

* **[!UICONTROL Activo]**: se utiliza para recursos y carpetas. Recursos y carpetas con la variable [!UICONTROL Activo] El estado es visible para todos los usuarios con permisos y se puede publicar en [!UICONTROL Brand Connect]. [!UICONTROL Activo] se indica con un punto verde en un recurso o carpeta.
* **[!UICONTROL Inactivo]**: se utiliza para recursos y carpetas. Recursos y carpetas con la variable [!UICONTROL Inactivo] el estado es visible para [!UICONTROL DAM de Workfront] pero no están visibles en el [!UICONTROL Brand Connect]. [!UICONTROL Inactivo] se indica con un punto rojo en un recurso o carpeta.
* **[!UICONTROL Sin caducar]**: se utiliza solo para recursos. Este es el estado predeterminado de todos los recursos. Recursos no caducados que también [!UICONTROL Activo] están visibles en la variable [!UICONTROL Brand Connect].
* **[!UICONTROL Caducado]**: se utiliza solo para recursos. Recursos con la variable [!UICONTROL Caducado] ningún usuario puede descargar el estado excepto el administrador del sistema. Los recursos caducados son visibles o no están visibles en el [!UICONTROL Brand Connect], según las configuraciones del sistema.
