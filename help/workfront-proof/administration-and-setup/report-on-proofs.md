---
title: Informar sobre revisiones
description: Aprenda a utilizar las funcionalidades de creación de informes para administrar el progreso de la revisión.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '445'
ht-degree: 100%

---

# Informar sobre revisiones

Las funciones de prueba digital de [!DNL Workfront] permiten administrar proyectos y flujos de trabajo de revisión relacionados en un solo lugar, [!DNL Workfront]. Obtenga información valiosa sobre el trabajo de pruebas que se está realizando con tipos de informes, fuentes de campos y nombres de campos que muestran información de revisión y aprobación.

Recomendamos trabajar con su consultor de [!DNL Workfront] para crear informes que cumplan los requisitos de su organización. Algunos de los informes deben estar familiarizados con la creación de informes del modo de texto de [!DNL Workfront].

Comience con estos informes estándar básicos para ayudar a sus equipos a administrar las pruebas que pasan por un proceso de revisión y aprobación en [!DNL Workfront].

## [!UICONTROL Aprobación de revisión]

Este tipo de informe le ayuda a realizar un seguimiento de las aprobaciones de prueba pendientes para asegurarse de que se cumplen los plazos.

![Seleccionar [!UICONTROL Aprobación de prueba] del menú desplegable [!UICONTROL Nuevo informe] ](assets/proof-system-setups-proof-approval-report.png)

Las opciones de visualización y filtrado incluyen la [!UICONTROL fecha de decisión], [!UICONTROL aprobación de la prueba], [!UICONTROL fase de aprobación], [!UICONTROL plantilla de flujo de trabajo] e [!UICONTROL información del solicitante]. Con la creación de informes del modo de texto, puede crear una agrupación que organice la lista por nombre de documento. [Comprensión del modo de texto básico de las agrupaciones](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=es).

Al escribir informes de aprobación de pruebas, asegúrese de que está obteniendo información relacionada con la versión más actual de las pruebas. [!DNL Workfront] recomienda incluir este origen de campo y el nombre de campo en el filtro:

**[!UICONTROL Aprobación de prueba]>>[!UICONTROL Es la versión del documento actual]**

![Pestaña Filtros del Creador de informes](assets/proof-system-setups-proof-approval-report-is-current-version.png)

Esto resulta útil cuando genera informes en pruebas que tienen varias versiones, por lo que el informe solo enumera la versión actual de cada prueba que necesita aprobación. Esto filtra las versiones anteriores en las que ya no necesita trabajar.

## [!UICONTROL Versión del documento]

Este tipo de informe le permite administrar y rastrear versiones en [!DNL Workfront].

![Seleccione la [!UICONTROL Versión del documento] del menú desplegable [!UICONTROL Nuevo informe] ](assets/proof-system-setups-document-version-report.png)

Las opciones de vista incluyen información de la [!UICONTROL versión del documento], [!UICONTROL documento], [!UICONTROL introducido por], [!UICONTROL estado de aprobación de la prueba], [!UICONTROL creador de pruebas] y [!UICONTROL proveedor de documentos].

Los agrupamientos se pueden realizar mediante la [!UICONTROL versión del documento], [!UICONTROL introducido por], [!UICONTROL estado de aprobación de la prueba] o información del propietario de la prueba.

Los filtros incluyen [!UICONTROL versión del documento], [!UICONTROL nivel de acceso], [!UICONTROL documento], [!UICONTROL introducido por], [!UICONTROL estado de aprobación de la prueba], [!UICONTROL creador de pruebas] y la información del proveedor de documentos.

Puede mostrar el nombre de la fase de prueba que está activa actualmente para cada documento del informe con esta columna en una vista:

**[!UICONTROL Versiones de documento] >> [!UICONTROL Etapas de prueba activas]**

![Pestaña Filtros del Creador de informes](assets/proof-system-setups-active-proof-stages.png)

Si no hay ningún escenario activo actualmente, la columna está en blanco.

Este origen de campo >> nombre de campo también está disponible como filtro en un informe.

Utilice el origen del campo [!UICONTROL Creador de pruebas] para informar sobre la información del usuario que creó la prueba. Elija el origen del campo [!UICONTROL Nombre] para mostrar el nombre del creador de pruebas en una vista.

**[!UICONTROL Creador de pruebas] >> [!UICONTROL Nombre]**

Esta combinación de origen del campo >> nombre del campo también está disponible como filtro.

![Pestaña Filtros del Creador de informes](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
