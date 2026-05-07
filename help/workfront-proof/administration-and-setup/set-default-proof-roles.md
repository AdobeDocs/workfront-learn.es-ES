---
title: Establecer roles de prueba predeterminados
description: Obtenga información sobre cómo establecer la función de prueba predeterminada que se asigna cuando se crean usuarios nuevos o las personas abren una prueba.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: '2024-01-24T00:00:00.000Z'
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T20:03:40.797Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 362
ht-degree: 87%

---

# Establecer roles de prueba predeterminados



La primera configuración predeterminada para completar es determinar una función de prueba predeterminada que se asignará cuando se creen nuevos usuarios o cuando las personas abran una prueba.

Las funciones de prueba determinan lo que un usuario puede hacer con una prueba: basta con verla, realizar comentarios, aprobarla, etc. [!DNL Workfront] recomienda que se establezcan los valores predeterminados de la función de prueba para todos los usuarios, a fin de que la adición de destinatarios a las pruebas y la configuración de los flujos de trabajo sean más rápidas y sencillas.

![Se pueden seleccionar funciones de prueba al cargar una prueba](assets/proof-system-setups-proof-role-example.png)

Sin embargo, esta función de prueba predeterminada se puede cambiar a medida que se cargan pruebas individuales, lo que garantiza que todos puedan cumplir la función que les corresponde en el proceso de revisión y aprobación.


## Establecer roles de prueba predeterminados

1. Seleccione **Configuración** del [!UICONTROL Menú principal].
1. Seleccione **Revisar y aprobar** en el menú de la izquierda.
1. Haga clic en el botón situado junto a la función de prueba predeterminada para los usuarios de [!DNL Workfront] nuevos y usuarios de prueba invitados para “destinatarios designados”: cualquier persona que se añada al flujo de trabajo de prueba, ya sea de forma manual o a través de una plantilla de flujo de trabajo.
1. Haga clic en el botón situado junto a la función de prueba predeterminada para usuarios de [!DNL Workfront] nuevos y usuarios de prueba invitados para usuarios “que no son destinatarios”. Estos son generalmente usuarios de [!DNL Workfront] que tienen acceso a una prueba, pero que no son una de las personas asignadas al flujo de trabajo.
1. Guarde los cambios.

![Configuración de revisión y aprobación en Workfront](assets/proof-system-setups-workfront-defaults.png)

Tenga en cuenta lo que se espera que haga la mayoría de los usuarios e invitados cuando se añadan a un flujo de trabajo de revisiones. Este debería ser su valor predeterminado.

## Prácticas recomendadas

| Práctica recomendada | He aquí por qué |
|---|---|
| Utilice únicamente Solo lectura o Revisor para los ajustes “Funciones para usuarios que no sean destinatarios que abran una prueba de documento” en Workfront. | Las demás opciones para esta configuración requieren que se tome una decisión de la revisión, lo que puede entorpecer el flujo de trabajo de la revisión. Por lo general, las personas que no están añadidas al flujo de trabajo de la revisión solo tienen que ver la prueba o comentar, no aprobar, por lo que las opciones Solo lectura o Revisor son la mejor elección.<br> <br>Nota: Este ajuste se encuentra en el menú principal de Workfront > Configuración > Revisión y aprobación. |
