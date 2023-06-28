---
title: Comprender el registro de auditoría del sistema
description: Aprenda a utilizar el registro de auditoría del sistema para revisar cuándo se realizaron cambios y cuándo se agregaron elementos.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Comprender el registro de auditoría del sistema

El registro de auditoría del sistema es la mejor manera por parte del administrador del sistema de estar al tanto de lo que sucede en [!DNL Workfront]. Piense en el registro como su fuente de verdad para saber quién hizo qué cambios y cuándo.

Para acceder al registro de auditoría, vaya a [!UICONTROL Preferencias] de la sección [!UICONTROL Configurar] área. De forma predeterminada, se ven los datos de los últimos siete días. Cambie los criterios de filtro para ver datos de diferentes intervalos de fechas.

Cuando un usuario realiza determinadas acciones, [!UICONTROL Workfront] los registra en el [!UICONTROL Registros de auditoría] de la sección [!UICONTROL Configurar] área.

![[!UICONTROL Tipo de registro] menú desplegable de la pestaña [!UICONTROL Registros de auditoría] página en [!UICONTROL Configurar]](assets/admin-fund-audit-log-1.png)

Cada acción registrada o registrada muestra:

* La fecha y la hora del cambio
* El tipo de registro
* El nombre del usuario que completó la acción
* El objeto
* Cualquier detalle asociado con la acción
* La dirección IP

![[!UICONTROL Registro de auditoría] lista](assets/admin-fund-audit-log-2.JPG)

## Exportar el registro de auditoría

La exportación de los datos del registro de auditoría permite a los administradores del sistema compartir la información con auditores internos/externos o especialistas en seguridad. Algunas organizaciones requieren que se conserven ciertos registros para cumplir con las regulaciones de ciberseguridad. Otros necesitan la información importada en un sistema de seguridad para su análisis.

Los registros de auditoría se pueden exportar en un archivo CSV (valor separado por comas), que se puede abrir en una aplicación de hoja de cálculo o en un editor de texto sin formato. La exportación está limitada a 50 000 filas a la vez, por lo que debe utilizar los filtros para reducir la lista si el total supera las 50 000.

![[!UICONTROL Exportar] botón activado [!UICONTROL Registros de auditoría] página](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
