---
title: Edición de una plantilla de flujo de trabajo automatizado
description: Aprenda a realizar cambios en una plantilla de flujo de trabajo de revisión automatizada existente en [!DNL  Workfront].
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
kt: 8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Edición de una plantilla de flujo de trabajo automatizado

A medida que se refinan los procesos de revisión y aprobación de pruebas o se realizan cambios en la organización, las plantillas de flujo de trabajo automatizadas deben actualizarse para reflejar las operaciones actuales de los equipos que utilizan Workfront.

Mantener las plantillas actualizadas garantiza la coherencia en los procesos de revisión y aprobación, además de ahorrar tiempo a los usuarios que cargan pruebas, ya que no tienen que modificar constantemente un flujo de trabajo.

1. Seleccionar **[!UICONTROL Revisión]** desde el **[!UICONTROL Menú principal]** in [!DNL Workfront].
1. Desde allí, seleccione **[!UICONTROL Flujos de trabajo]** en el menú del panel izquierdo.
1. Haga clic en el menú de 3 puntos situado en el extremo derecho del nombre de la plantilla y seleccione **[!UICONTROL Ver detalles de la plantilla]**.

Las opciones para compartir, copiar y eliminar la plantilla se encuentran en la parte superior de la ventana de detalles de la plantilla para cada plantilla. La eliminación de una plantilla no afecta a las pruebas en curso que tengan esa plantilla aplicada, pero significa que la plantilla ya no está disponible para su uso.

![Ventana de detalles de plantilla](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

Haga clic en la flecha para expandir [!UICONTROL Detalles] para cambiar cosas como el nombre de la plantilla o la zona horaria de la plantilla.

## Realizar cambios en las fases y los destinatarios

Es posible que sea necesario realizar cambios en la [!UICONTROL Flujo de trabajo] área en la que un proceso optimizado implica una fecha límite anterior o en la que alguien se une al equipo y revisará las pruebas.

Cada fase de un flujo de trabajo automatizado tiene su propia sección, que permite modificar de forma independiente los plazos, la privacidad, los destinatarios de prueba y otra información.

Este vídeo muestra brevemente algunos de los cambios que puede realizar en la [!UICONTROL Flujo de trabajo] área. Consulte la lista con viñetas debajo de este vídeo, que revisa esta configuración. No hay audio en este vídeo.

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12)

Como revisión, estos son los cambios de plantilla de prueba que puede realizar en la [!UICONTROL Flujo de trabajo] sección:

* Haga clic en [!UICONTROL nombre del escenario] o el campo [!UICONTROL deadline] para actualizar esa información.
* Seleccione la flecha situada junto a la variable [!UICONTROL deadline] para bloquear la fase, determine cuándo se activa o requiera una sola decisión.
* En la lista de destinatarios, haga clic en [!UICONTROL Rol] o [!UICONTROL Alertas de correo electrónico] para seleccionar otra opción.
* Vaya al menú de 3 puntos situado a la derecha del nombre de un destinatario para eliminarlo de la lista, convertirlo en el responsable principal de la toma de decisiones para esa fase del flujo de trabajo o editar la información de la función de prueba y la alerta por correo electrónico.
* Tiene dos opciones para agregar destinatarios a la lista. Una vez que haya abierto el [!UICONTROL Agregar personas al escenario] , haga clic en el escenario al que desee agregarlas. A continuación, introduzca su nombre o dirección de correo electrónico en la lista de destinatarios y asigne una función de prueba y una alerta de correo electrónico. Haga clic en [!UICONTROL Agregar personas] cuando haya terminado.
   1. En la esquina superior derecha de cada sección de fase, vaya a la [!UICONTROL Más] y seleccione [!UICONTROL Agregar personas al escenario].
   1. En la parte superior del [!UICONTROL Flujo de trabajo] , seleccione [!UICONTROL Agregar personas al escenario].

## Uso compartido de plantillas

El [!UICONTROL Compartido con] muestra los usuarios de prueba que pueden utilizar la plantilla. Elimine las personas que ya no necesiten utilizar la plantilla haciendo clic en el menú de 3 puntos situado a la derecha de su nombre y seleccionando [!UICONTROL Eliminar].

![[!UICONTROL Compartido con] lista](assets/proof-system-setups-edit-template-shared-with.png)

Sin embargo, no puede agregar personas a la lista de uso compartido desde esta sección. Para ello, vuelva a la parte superior de la ventana de detalles de la plantilla y haga clic en [!UICONTROL Compartir plantilla] botón.

## Sección Actividad

[!DNL Workfront] mantiene un historial de auditoría de cuándo se realizaron cambios en la plantilla. Puede ver la fecha, quién realizó el cambio y alguna información breve sobre los cambios realizados.

Esta sección no registra información sobre cuándo se ha utilizado la plantilla en las pruebas.

![Lista de actividades de revisión](assets/proof-system-setups-edit-template-activity.png)
