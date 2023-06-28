---
title: Explicación de los grupos y usuarios en [!UICONTROL WORKFRONT DAM]
description: Obtenga información sobre cómo crear carpetas, grupos y usuarios en [!UICONTROL WORKFRONT DAM]. Comprenda los tipos de funciones de usuario y conceda permisos a las carpetas.
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
ht-degree: 0%

---

# Configuración del sistema: grupos y usuarios

En este vídeo, aprenderá a hacer lo siguiente:

* Comprender cómo las configuraciones de grupo afectan al acceso a los recursos
* Crear carpetas, grupos y usuarios en un orden específico
* Explicación de los tipos de funciones de usuario
* Conceder permisos a carpetas
* Creación y edición de grupos
* Adición y edición de usuarios

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## Revisión de grupos y usuarios

Al configurar su [!UICONTROL WORKFRONT DAM] , es importante tener en cuenta las funciones que los usuarios y grupos desempeñan en el panorama general.

Los grupos controlan el acceso a las carpetas de recursos en [!UICONTROL WORKFRONT DAM]. La configuración de grupo también controla lo que los usuarios pueden hacer con los recursos (ver, descargar, editar, etc.) tienen permiso para acceder a.

Al crear grupos, es vital tener en cuenta a qué carpetas de recursos necesitarán acceso los miembros de ese grupo en [!UICONTROL WORKFRONT DAM].

Los usuarios son las personas que tienen inicios de sesión en [!UICONTROL WORKFRONT DAM]. Un usuario no puede acceder a nada en [!UICONTROL WORKFRONT DAM] a menos que estén asignados a un grupo. Los usuarios pueden pertenecer a más de un grupo, según sus necesidades.

## Grupos predeterminados

Hay dos grupos predeterminados que se incluyen con [!UICONTROL WORKFRONT DAM]. Todos los usuarios pertenecen a estos grupos automáticamente, en función de si tienen [!UICONTROL WORKFRONT DAM] credenciales de inicio de sesión. No puede agregar ni eliminar usuarios de estos grupos:

* **Grupo de invitados**: se utiliza para controlar el acceso de un usuario anónimo. Podría tratarse de alguien sin credenciales de inicio de sesión o de un usuario que no haya iniciado sesión en ese momento.
* **Registrados** Grupo de inicio de sesión: todos los usuarios que han iniciado sesión pertenecen a este grupo.

El grupo Administración y su configuración también existen de forma predeterminada. Puede agregar usuarios a este grupo, pero no puede ajustar la configuración.

## Tipos de roles

A medida que se crean los grupos, se les asigna un tipo de función. El tipo de función determina qué parte del [!UICONTROL WORKFRONT DAM] los usuarios del sistema obtienen cuando inician sesión — [!UICONTROL WORKFRONT DAM] o bien [!UICONTROL Brand Connect].

Hay tres tipos de funciones disponibles con [!UICONTROL WORKFRONT DAM] licencias:

* **[!UICONTROL Brand Portal]**: estos usuarios solo tienen acceso a [!UICONTROL Brand Connect], donde pueden ver y descargar los recursos aprobados.
* **[!UICONTROL Colaborador]**: estos usuarios pueden acceder a [!UICONTROL WORKFRONT DAM] y [!UICONTROL Brand Connect]. Tienen derechos de acceso completos a recursos y carpetas: ver, descargar, cargar, editar, mover y eliminar.
* **[!UICONTROL Administrador]**: los administradores del sistema tienen acceso a todo en [!UICONTROL Brand Connect] y [!UICONTROL WORKFRONT DAM], además de la capacidad de establecer la configuración global del sistema para cada uno. También pueden acceder a recursos que han caducado o que se han establecido como inactivos.

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
