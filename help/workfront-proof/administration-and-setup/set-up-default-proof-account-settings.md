---
title: Ajustar la configuración predeterminada de la cuenta de prueba
description: Obtenga información sobre la configuración de la cuenta predeterminada que se aplica globalmente a todos los usuarios de pruebas y revisión.
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-up-proof-actual-default-settings.png
jira: KT-10236
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 6eda8bcd-ab0f-4e02-9080-64b6051b327f
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 100%

---

# Ajustar la configuración predeterminada de la cuenta de prueba

Establezca la configuración de la cuenta predeterminada que se aplica globalmente a todos los usuarios de pruebas y revisión: país, idioma y zona horaria. Si tiene usuarios en varios países o zonas horarias, puede ajustar esta configuración en el perfil de usuario de cada individuo, si es necesario.

![Ventana Configuración de la cuenta para la revisión](assets/proof-system-setups-default-account-settings.png)

1. Seleccione **[!UICONTROL Revisión]** del [!UICONTROL Menú principal] de [!DNL Workfront's].
1. Seleccione **[!UICONTROL Configuración de la cuenta]** en la barra de navegación superior.
1. Seleccione la pestaña **[!UICONTROL Detalles]**.
1. Vaya al campo [!UICONTROL País] y seleccione **[!UICONTROL Editar]**. Elija el país en el que se encuentran la mayoría de los usuarios de la revisión de forma predeterminada.
1. Seleccione **[!UICONTROL Guardar]** para esa configuración.
1. Vaya al campo [!UICONTROL Idioma predeterminado] y seleccione **[!UICONTROL Editar]**. Elija el idioma que la mayoría de los usuarios de revisión utilizarán como predeterminado.
1. Seleccione **[!UICONTROL Guardar]** para esa configuración.
1. Vaya al campo [!UICONTROL Zona horaria predeterminada] y seleccione **[!UICONTROL Editar]**. Elija la zona horaria en la que estará la mayoría de los usuarios de la revisión como opción predeterminada. Esta será la zona horaria reconocida por los flujos de trabajo de prueba que se configuran manualmente. También se aplicará a las plantillas de flujo de trabajo de prueba, pero cada plantilla puede tener una zona horaria establecida.
1. Seleccione **[!UICONTROL Guardar]** para esa configuración.

## Prácticas recomendadas


| Práctica recomendada | He aquí por qué |
|---|---|
| Ajuste la configuración del back-end de prueba para que los usuarios vean las fechas límite en formato de reloj de 12 horas. | Seleccione la opción F j, Y, gi:a en la configuración de prueba para los usuarios que deseen ver fechas y horas límite de prueba en formato a. m./p. m. Para las zonas que utilizan un reloj de 12 horas, esto ayuda a aclarar los plazos.<br> <br>Nota: Para encontrar esta configuración, vaya al menú principal de Workfront > Revisión > Configuración de la cuenta > Usuarios > y edite el campo Formato de fecha para cada uno de ellos. |
| Establezca una fecha límite de la revisión predeterminada como parte de la configuración del sistema. | Cuando se establece la fecha límite de la revisión predeterminada (la fecha de carga + el número de días laborables), si el creador de la prueba olvida añadir una fecha límite, Workfront aplica automáticamente esta fecha límite a cada prueba cargada.<br> <br>Nota: Para encontrar esta configuración, vaya al menú principal de Workfront > Revisión > Configuración de la cuenta > Configuración > Valores predeterminados de la prueba > campo Fecha límite (+ días laborables). |
| Ocultar la opción de decisión de la revisión no relevante. | Esta opción de decisión suele causar confusión entre los aprobadores, ya que las organizaciones a menudo no definen cuándo se debe utilizar la opción No relevante. La opción No relevante generalmente indica que la prueba no es relevante para el destinatario de la prueba y que no necesita tomar una decisión de aprobado o rechazado. Al seleccionar No relevante, esto permite que continúe el flujo de trabajo de prueba.<br> <br>La opción No relevante no es necesaria en la mayoría de los flujos de trabajo de prueba.<br> <br>Nota: Para encontrar esta configuración, vaya al menú principal de Workfront > Revisión > Configuración de la cuenta > Decisiones. |
| No reordene las opciones de decisión de la revisión en la configuración de la prueba. | Cada configuración de la decisión de la revisión contiene un valor/peso específico que, si se reordena, puede generar confusión en las configuraciones de prueba. El orden de decisión y el valor/peso se utilizan como activadores de la fase de prueba y en la creación de informes.<br> <br>Para encontrar esta configuración, vaya al menú principal > Revisión > Configuración de la cuenta > Decisiones. |
| Establezca los valores predeterminados de usuario para las funciones de prueba y las alertas de correo electrónico. | Estos ajustes se rellenan automáticamente al asignar un flujo de trabajo de prueba, lo que acelera el proceso y contribuye a la coherencia entre los flujos de trabajo de prueba.<br> <br>Nota: La configuración predeterminada del usuario se encuentra en el menú principal de Workfront > Revisión > Configuración de la cuenta > Usuarios > y al seleccionar el usuario para el cual se establecen los valores predeterminados. |
