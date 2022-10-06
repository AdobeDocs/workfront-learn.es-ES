---
title: Editar una plantilla de flujo de trabajo automatizada
description: Aprenda a realizar cambios en una plantilla de flujo de trabajo de pruebas automatizadas existente en [!DNL  Workfront].
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
kt: 8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Edición de una plantilla de flujo de trabajo automatizada

A medida que se refinan los procesos de revisión y aprobación de la prueba o que se realizan cambios organizativos, las plantillas de flujo de trabajo automatizadas deben actualizarse para reflejar las operaciones actuales de sus equipos con Workfront.

Mantener las plantillas actualizadas garantiza la coherencia en los procesos de revisión y aprobación, además de ahorra tiempo para las pruebas de carga, ya que no tienen que modificar constantemente un flujo de trabajo.

1. Select **[!UICONTROL Prueba]** de la variable **[!UICONTROL Menú principal]** en [!DNL Workfront].
1. Desde allí, seleccione **[!UICONTROL Flujos de trabajo]** en el menú del panel izquierdo.
1. Haga clic en el menú de 3 puntos situado en el extremo derecho del nombre de la plantilla y seleccione **[!UICONTROL Ver detalles de una plantilla]**.

Las opciones para compartir, copiar y eliminar la plantilla se encuentran en la parte superior de la ventana de detalles de cada plantilla. La eliminación de una plantilla no afecta a las pruebas en curso que tengan esa plantilla aplicada, pero significa que ya no está disponible para su uso.

![Ventana de detalles de plantilla](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

Haga clic en la flecha para expandir el [!UICONTROL Detalles] para cambiar cosas como el nombre de la plantilla o la zona horaria de la plantilla.

## Realizar cambios en las etapas y los destinatarios

Es posible que se necesiten cambios en la variable [!UICONTROL Flujo de trabajo] área en la que un proceso optimizado significa una fecha límite anterior o cuando alguien se una al equipo y revisará las pruebas.

Cada etapa de un flujo de trabajo automatizado tiene su propia sección, que permite que los plazos, la privacidad, los destinatarios de prueba y otra información se modifiquen de forma independiente.

Este vídeo muestra brevemente algunos de los cambios que puede realizar en la [!UICONTROL Flujo de trabajo] . Consulte la lista con viñetas de este vídeo, que revisa esta configuración. No hay audio en este vídeo.

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12)

Como revisión, estos son los cambios de plantilla de prueba que puede realizar en la variable [!UICONTROL Flujo de trabajo] sección:

* Haga clic en [!UICONTROL nombre de escenario] o [!UICONTROL límite] para actualizar esa información.
* Seleccione la flecha junto a la [!UICONTROL límite] para bloquear el escenario, determine cuándo se activa el escenario o requiera una sola decisión.
* En la lista de destinatarios, haga clic en [!UICONTROL Función] o [!UICONTROL Alertas de correo electrónico] para seleccionar otra opción.
* Vaya al menú de 3 puntos situado a la derecha del nombre de un destinatario para eliminarlo de la lista, convertirlo en el principal responsable de decisiones para esa fase del flujo de trabajo o editar la función de prueba y la información de alerta por correo electrónico.
* Tiene dos opciones para agregar destinatarios a la lista. Una vez que haya abierto el [!UICONTROL Agregar personas al escenario] , haga clic en la etapa a la que desee agregarlas. A continuación, introduzca su nombre o dirección de correo electrónico en la lista de destinatarios y asigne una función de prueba y una alerta de correo electrónico. Haga clic en el [!UICONTROL Agregar personas] cuando haya terminado.
   1. En la esquina superior derecha de cada sección de escenario, vaya a la [!UICONTROL Más] y seleccione [!UICONTROL Agregar personas al escenario].
   1. En la parte superior del [!UICONTROL Flujo de trabajo] área, seleccione [!UICONTROL Agregar personas al escenario].

## Uso compartido de plantillas

La variable [!UICONTROL Compartido Con] muestra los usuarios de prueba que pueden utilizar la plantilla. Elimine las personas que ya no necesiten utilizar la plantilla haciendo clic en el menú de 3 puntos situado a la derecha de su nombre y seleccionando [!UICONTROL Eliminar].

![[!UICONTROL Compartido Con] list](assets/proof-system-setups-edit-template-shared-with.png)

Sin embargo, no puede agregar personas a la lista de uso compartido desde esta sección. Para ello, vuelva a la parte superior de la ventana de detalles de la plantilla y haga clic en el botón [!UICONTROL Compartir plantilla] botón.

## Sección Actividad

[!DNL Workfront] mantiene un historial de auditoría de cuándo se realizaron cambios en la plantilla. Puede ver la fecha, quién realizó el cambio y alguna información breve sobre los cambios realizados.

Esta sección no registra información sobre cuándo se utilizó la plantilla en pruebas.

![Lista de actividades de prueba](assets/proof-system-setups-edit-template-activity.png)
