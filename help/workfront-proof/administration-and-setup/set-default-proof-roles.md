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
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 52%

---

# Establecer roles de prueba predeterminados



La primera configuración predeterminada para completar es determinar una función de prueba predeterminada que se asignará cuando se creen nuevos usuarios o cuando las personas abran una prueba.

Las funciones de prueba determinan lo que un usuario puede hacer con una prueba: basta con verla, realizar comentarios, aprobarla, etc. [!DNL Workfront] recomienda establecer los valores predeterminados de la función de prueba para todos los usuarios, para añadir destinatarios a pruebas y configurar flujos de trabajo de forma más rápida y sencilla.

![Se pueden seleccionar funciones de prueba al cargar una prueba](assets/proof-system-setups-proof-role-example.png)

Sin embargo, esta función de prueba predeterminada se puede cambiar a medida que se cargan pruebas individuales, lo que garantiza que todos puedan cumplir la función que les corresponde en el proceso de revisión y aprobación.


## Establecer roles de prueba predeterminados

1. Seleccione **Configuración** del [!UICONTROL Menú principal].
1. Seleccione **Revisar y aprobar** en el menú de la izquierda.
1. Haga clic en el botón situado junto a la función de prueba predeterminada que desee para las dos funciones nuevas [!DNL Workfront] usuarios y usuarios de prueba invitados para &quot;destinatarios designados&quot;: cualquier persona que se añada al flujo de trabajo de prueba, ya sea de forma manual o a través de una plantilla de flujo de trabajo.
1. Haga clic en el botón situado junto a la función de prueba predeterminada que desee para las dos funciones nuevas [!DNL Workfront] usuarios y usuarios de prueba invitados para usuarios &quot;no destinatarios&quot;. Generalmente, son [!DNL Workfront] usuarios que tienen acceso a una prueba pero que no son una de las personas asignadas al flujo de trabajo.
1. Guarde los cambios.

![Configuración de revisión y aprobación en Workfront](assets/proof-system-setups-workfront-defaults.png)

Tenga en cuenta lo que se espera que haga la mayoría de los usuarios e invitados cuando se añadan a un flujo de trabajo de pruebas. Este debería ser su valor predeterminado.

## Prácticas recomendadas

| Práctica recomendada | He aquí por qué |
|---|---|
| Utilice solo lectura o Revisor para la configuración &quot;Funciones para usuarios que no son destinatarios y que abren una revisión de documento&quot; en Workfront. | El resto de opciones de esta configuración requieren que se tome una decisión sobre la prueba, lo que puede descarrilar el flujo de trabajo de prueba. Por lo general, las personas que no se agregan al flujo de trabajo de prueba solo necesitan ver la prueba o hacer comentarios, no aprobar realmente la prueba, por lo que las opciones Solo lectura o Revisor son las mejores. <br> <br>Nota: Esta configuración se encuentra en el menú principal de Workfront > Configuración > Revisión y aprobación. |
