---
title: Comprender el registro de auditoría del sistema
description: Aprenda a utilizar el registro de auditoría del sistema para revisar cuándo se realizaron cambios y cuándo a los elementos.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
TQID: https://experienceleague.adobe.com/xMxWQ53TUXVjS-H8EuK3nf7jt8v4vUgKoZVsmApc-JM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 100%

---

# Comprender el registro de auditoría del sistema

El registro de auditoría del sistema es la mejor manera de que el administrador del sistema esté atento a lo que sucede en [!DNL Workfront]. Piense en el registro como su fuente de verdad para quién hizo qué cambios y cuándo.

Acceda al registro de auditoría desde la sección [!UICONTROL Preferencias] en área [!UICONTROL Configuración]. De forma predeterminada, se ven los datos de los últimos siete días. Cambie los criterios de filtro para ver los datos de diferentes intervalos de fechas.

Cuando un usuario realiza determinadas acciones, [!UICONTROL Workfront] las registra en la sección [!UICONTROL Registros de auditoría] del área [!UICONTROL Configuración].

Menú desplegable ![[!UICONTROL Tipo de registro] en la página [!UICONTROL Registros de auditoría] en [!UICONTROL Configuración]](assets/admin-fund-audit-log-1.png)

Cada acción registrada muestra lo siguiente:

* La fecha y hora del cambio
* El tipo de registro
* El nombre del usuario que completó la acción
* El objeto
* Cualquier detalle asociado con la acción
* La dirección IP

Lista del ![[!UICONTROL Registro de auditoría]](assets/admin-fund-audit-log-2.JPG)

## Exportar el registro de auditoría

La exportación de los datos del registro de auditoría permite a los administradores del sistema compartir la información con auditores internos/externos o especialistas en seguridad. Algunas organizaciones necesitan que se mantengan ciertos registros para cumplir con las regulaciones de seguridad cibernética. Otros necesitan la información importada en un sistema de seguridad para su análisis.

Los registros de auditoría se pueden exportar en un archivo CSV (valor separado por comas), que se puede abrir en una aplicación de hoja de cálculo o en un editor de texto sin formato. La exportación está limitada a 50 000 filas al mismo tiempo, por lo que debe utilizar los filtros para reducir la lista si el total supera los 50 000.

Botón ![[!UICONTROL Exportar] en la página [!UICONTROL Registros de auditoría]](assets/admin-fund-audit-log-3.png)

<!--
learn more URLs
Audit logs
Managing audit logs
-->
