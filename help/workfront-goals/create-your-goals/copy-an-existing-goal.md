---
title: Copiar una meta existente
description: Obtenga información sobre cómo copiar un objetivo existente en [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
    internal-label: Workfront Goals
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 98%
---
# Copiar una meta existente

Digamos que es el final de un trimestre y queremos recrear una meta existente para el próximo período. O tal vez no haya completado la meta y necesita ampliarla hasta el siguiente período de tiempo. ¿Cuál es la mejor opción para crearlo? Desea copiar y modificar una meta existente.

Copiar una meta existente también es útil si varios integrantes del equipo tienen objetivos similares y necesita crear una meta para cada uno de ellos.

<!--
Pro-tips graphic
-->

Estas son algunas cosas que hay que tener en cuenta antes de copiar las metas:

* Se copia toda la información de la meta original, con la excepción del período (porque es en el pasado).
* Puede copiar los resultados de una meta existente y se transferirán a la nueva.
* Los resultados copiados se asignan al mismo propietario de forma predeterminada.
* No se puede copiar el progreso de una meta existente en una nueva.
* No se pueden copiar las actividades de una meta al copiarla.

## Cómo copiar una meta

1. Haga clic en un nombre de una meta para abrir el panel **[!UICONTROL Detalles de la meta]**.
1. Haga clic en el icono de tres puntos y, a continuación, seleccione **[!UICONTROL Copiar]**.
1. Actualice cualquiera de la siguiente información para la meta copiada:
   * **Nuevo meta**: este es el nombre de la meta nueva. El valor predeterminado es el nombre de la meta original.
   * **Período**: el período de tiempo durante el cual desea alcanzar la meta. Seleccione un período de tiempo en el menú desplegable o haga clic en Definir fechas personalizadas para indicar un período de tiempo personalizado. El período predeterminado siempre es el trimestre actual.
   * **Propietario**: el propietario de la meta. Puede ser un usuario, equipo, grupo o empresa. El valor predeterminado es el propietario de la meta original.
   * **Descripción**: información adicional sobre la meta.

1. Marque la casilla **[!UICONTROL Copiar resultados]** si la meta original tenía resultados añadidos y desea copiarlos a la nueva meta. Los resultados de la meta copiada tienen el mismo propietario, nombres y valores medidos que los resultados de la meta original.

1. Haga clic en **[!UICONTROL Guardar]**. La meta copiada se guarda con el estado Borrador.

   ![Una imagen del panel [!UICONTROL Detalles de la meta] en [!DNL Workfront Goals] con la opción [!UICONTROL Copiar] &#x200B;](assets/03-workfront-goals-copy-a-goal.png)

1. Haga clic en **[!UICONTROL Activar]**, que actualiza el estado de la meta a Activo. La meta debe tener una actividad asociada o un resultado para “activar”.

1. Haga clic en la **X** en la parte superior derecha del panel [!UICONTROL Detalles de la meta] para cerrarlo.

Si ha copiado una meta que no se ha completado en un período de tiempo anterior y desea continuar trabajando en él en el siguiente período de tiempo, haga lo siguiente:

1. Vaya a la meta original en la **[!UICONTROL Lista de metas]**, sección **[!UICONTROL Registro]** o **[!UICONTROL Pulse]**.
1. Comente la meta para indicar que se copió y se creó una más actual.
1. Cierre la meta original para preservar el progreso realizado durante su período de tiempo original. Haga clic en el icono de tres puntos del panel **[!UICONTROL Detalles de la meta]** y seleccione **[!UICONTROL Cerrar]** en el menú.
1. Actualice el valor [!UICONTROL Inicial] del nuevo resultado para que coincida con el valor **[!UICONTROL Destinatario]** del resultado anterior, por lo que el nuevo progreso de la meta comienza a calcularse a partir del punto alcanzado en el período anterior.
