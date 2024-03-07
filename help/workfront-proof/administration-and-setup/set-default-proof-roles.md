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
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: ht
source-wordcount: '359'
ht-degree: 100%

---

# Establecer roles de prueba predeterminados



La primera configuración predeterminada para completar es determinar una función de prueba predeterminada que se asignará cuando se creen nuevos usuarios o cuando las personas abran una prueba.

Las funciones de prueba determinan lo que un usuario puede hacer con una prueba: basta con verla, realizar comentarios, aprobarla, etc. [!DNL Workfront] recomienda establecer los valores predeterminados de la función de prueba para todos los usuarios, para añadir destinatarios a pruebas y configurar flujos de trabajo de forma más rápida y sencilla.

![Se pueden seleccionar funciones de prueba al cargar una prueba](assets/proof-system-setups-proof-role-example.png)

Sin embargo, esta función de prueba predeterminada se puede cambiar a medida que se cargan pruebas individuales, lo que garantiza que todos puedan cumplir la función que les corresponde en el proceso de revisión y aprobación.


## Establecer roles de prueba predeterminados

1. Seleccione **Configuración** del [!UICONTROL Menú principal].
1. Seleccione **Revisar y aprobar** en el menú de la izquierda.
1. Haga clic en el botón situado junto a la función de prueba predeterminada para los usuarios de [!DNL Workfront] nuevos y usuarios de prueba invitados para “destinatarios designados”: cualquier persona que se añada al flujo de trabajo de prueba, ya sea de forma manual o a través de una plantilla de flujo de trabajo.
1. Haga clic en el botón situado junto a la función de prueba predeterminada para usuarios de [!DNL Workfront] nuevos y usuarios de prueba invitados para usuarios “que no son destinatarios”. Estos son generalmente usuarios de [!DNL Workfront] que tienen acceso a una prueba, pero que no son una de las personas asignadas al flujo de trabajo.
1. Guarde los cambios.

![Configuración de revisión y aprobación en Workfront](assets/proof-system-setups-workfront-defaults.png)

Tenga en cuenta lo que se espera que haga la mayoría de los usuarios e invitados cuando se añadan a un flujo de trabajo de pruebas. Este debería ser su valor predeterminado.

## Prácticas recomendadas

| Práctica recomendada | He aquí por qué |
|---|---|
| Utilice únicamente Solo lectura o Revisor para los ajustes “Funciones para usuarios que no sean destinatarios que abran una prueba de documento” en Workfront. | Las demás opciones para esta configuración requieren que se tome una decisión de la revisión, lo que puede entorpecer el flujo de trabajo de la revisión. Por lo general, las personas que no están añadidas al flujo de trabajo de la revisión solo tienen que ver la prueba o comentar, no aprobar, por lo que las opciones Solo lectura o Revisor son la mejor elección.<br> <br>Nota: Este ajuste se encuentra en el menú principal de Workfront > Configuración > Revisión y aprobación. |
