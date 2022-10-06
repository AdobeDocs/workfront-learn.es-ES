---
title: Grupos y usuarios en [!UICONTROL DAM de Workfront]
description: Obtenga información sobre cómo crear carpetas, grupos y usuarios en [!UICONTROL DAM de Workfront]. Comprenda los tipos de funciones de usuario y conceda permisos a las carpetas.
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Configuración del sistema: grupos y usuarios

En este vídeo, aprenderá a:

* Comprender cómo afectan las configuraciones de grupo al acceso a los recursos
* Crear carpetas, grupos y usuarios en un orden específico
* Comprender los tipos de funciones de usuario
* Conceder permisos a carpetas
* Crear y editar grupos
* Agregar y editar usuarios

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12)

## Revisión de grupos y usuarios

A medida que configura el [!UICONTROL DAM de Workfront] , es importante tener en cuenta las funciones que los usuarios y grupos desempeñan en el panorama general.

Los grupos controlan el acceso a las carpetas de recursos en [!UICONTROL DAM de Workfront]. La configuración de grupo también controla lo que los usuarios pueden hacer con los recursos (ver, descargar, editar, etc.) tienen permiso de acceso.

Al crear grupos, es vital tener en cuenta a qué carpetas de recursos necesitarán acceder los miembros de ese grupo en [!UICONTROL DAM de Workfront].

Los usuarios son las personas que tienen acceso a [!UICONTROL DAM de Workfront]. Un usuario no puede acceder a nada en [!UICONTROL DAM de Workfront] a menos que se asignen a un grupo. Los usuarios pueden pertenecer a más de un grupo, según sus necesidades.

## Grupos predeterminados

Hay dos grupos predeterminados que se incluyen con [!UICONTROL DAM de Workfront]. Todos los usuarios pertenecen a estos grupos automáticamente, en función de si tienen [!UICONTROL DAM de Workfront] credenciales de inicio de sesión. No puede agregar ni quitar usuarios de estos grupos:

* **Grupo de invitados**: se utiliza para controlar el acceso de un usuario anónimo. Podría ser alguien sin credenciales de inicio de sesión o un usuario que actualmente no ha iniciado sesión.
* **Registrado**-En grupo: todos los usuarios que han iniciado sesión pertenecen a este grupo.

El grupo Administración y su configuración también existen de forma predeterminada. Puede agregar usuarios a este grupo, pero no puede ajustar la configuración.

## Tipos de funciones

A medida que se crean los grupos, se les asigna un tipo de función. El tipo de función determina qué parte de la variable [!UICONTROL DAM de Workfront] los usuarios del sistema obtienen cuando inician sesión — [!UICONTROL DAM de Workfront] o [!UICONTROL Brand Connect].

Hay tres tipos de funciones disponibles con [!UICONTROL DAM de Workfront] licencias:

* **[!UICONTROL Brand Portal]**—Estos usuarios solo tienen acceso a [!UICONTROL Brand Connect], que es donde pueden ver y descargar los recursos aprobados.
* **[!UICONTROL Colaborador]**: estos usuarios pueden acceder a [!UICONTROL DAM de Workfront] y [!UICONTROL Brand Connect]. Tienen derechos de acceso completos a los recursos y las carpetas: ver, descargar, cargar, editar, mover y eliminar.
* **[!UICONTROL Administrador]**: los administradores de sistemas tienen acceso a todo lo incluido en [!UICONTROL Brand Connect] y [!UICONTROL DAM de Workfront], además de la capacidad de establecer la configuración global del sistema para cada uno. También pueden acceder a los recursos que han caducado o que se han establecido como inactivos.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
