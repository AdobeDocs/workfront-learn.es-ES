---
title: Explicación de los grupos y usuarios en [!UICONTROL DAM de Workfront]
description: Obtenga información sobre cómo crear carpetas, grupos y usuarios en [!UICONTROL DAM de Workfront]. Comprenda los tipos de funciones de usuario y conceda permisos a las carpetas.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 100%

---

# Configuración del sistema: grupos y usuarios

Este vídeo contiene información sobre:

* Comprender cómo afectan las configuraciones de grupo al acceso a los recursos
* Crear carpetas, grupos y usuarios en un orden específico
* Comprender los tipos de funciones de usuario
* Conceder permisos a carpetas
* Crear y editar grupos
* Agregar y editar usuarios

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## Revisión de grupos y usuarios

A medida que configura el sistema de [!UICONTROL DAM de Workfront], es importante tener en cuenta las funciones que los usuarios y grupos desempeñan en el panorama general.

Los grupos controlan el acceso a las carpetas de recursos en [!UICONTROL DAM de Workfront]. La configuración de grupo también controla lo que los usuarios pueden hacer con los recursos (ver, descargar, editar, etc.) a los que tienen permiso de acceso.

Al crear grupos, es vital tener en cuenta a qué carpetas de recursos necesitarán acceder los miembros de ese grupo en [!UICONTROL DAM de Workfront].

Los usuarios son las personas que tienen acceso a [!UICONTROL DAM de Workfront]. Un usuario no puede acceder o utilizar el [!UICONTROL DAM de Workfront] a menos que se le asigne un grupo. Los usuarios pueden pertenecer a más de un grupo, según sus necesidades.

## Grupos predeterminados

Hay dos grupos predeterminados que se incluyen en [!UICONTROL DAM de Workfront]. Todos los usuarios pertenecen a estos grupos automáticamente, en función de si tienen credenciales de inicio de sesión de [!UICONTROL DAM de Workfront]. No puede agregar ni quitar usuarios de los siguientes grupos.

* **Grupo de invitados**: se utiliza para controlar el acceso de un usuario anónimo. Puede tratarse de alguien sin credenciales de acceso o de un usuario que no haya iniciado sesión.
* Grupo **conectado**: todos los usuarios que han iniciado sesión pertenecen a este grupo.

El grupo Administración y su configuración también existen de forma predeterminada. Puede agregar usuarios a este grupo, pero no puede ajustar la configuración.

## Tipos de funciones

A medida que se crean los grupos, se les asigna un tipo de función. El tipo de función determina qué parte del sistema de [!UICONTROL DAM de Workfront] obtienen los usuarios cuando inician sesión: [!UICONTROL DAM de Workfront] o [!UICONTROL Brand Connect].

Hay tres tipos de funciones disponibles con las licencias de [!UICONTROL DAM de Workfront]:

* **[!UICONTROL Brand Portal]**: estos usuarios solo tienen acceso a [!UICONTROL Brand Connect], que es donde pueden ver y descargar los recursos aprobados.
* **[!UICONTROL Colaborador]**: estos usuarios pueden acceder a [!UICONTROL DAM de Workfront] y [!UICONTROL Brand Connect]. Tienen derechos de acceso completo a los recursos y las carpetas: ver, descargar, cargar, editar, mover y eliminar.
* **[!UICONTROL Administrador]**: los administradores del sistema tienen acceso a todo lo incluido en [!UICONTROL Brand Connect] y [!UICONTROL DAM de Workfront], además de la capacidad de establecer la configuración global del sistema para cada uno. También pueden acceder a los recursos que han caducado o que se han establecido como inactivos.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
