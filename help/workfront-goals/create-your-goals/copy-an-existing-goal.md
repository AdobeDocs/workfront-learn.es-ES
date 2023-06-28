---
title: Copiar una meta existente
description: Obtenga información sobre cómo copiar una meta existente en [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
jira: KT-10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Copiar una meta existente

Supongamos que es el final de un trimestre y que desea volver a crear un objetivo existente para el siguiente período. O tal vez no completó el objetivo y necesita ampliarlo al siguiente período de tiempo. ¿Cuál es la mejor opción para crear esa meta? Desea copiar y modificar un objetivo existente.

Copiar una meta existente también es útil si varios integrantes del equipo tienen metas similares y necesita crear una meta para cada una de ellas.

<!--
Pro-tips graphic
-->

Estas son algunas cosas que hay que tener en cuenta antes de copiar los objetivos:

* Toda la información de la meta original se copiará, con la excepción del periodo de la meta (porque está en el pasado).
* Puede copiar los resultados de una meta existente y se transferirán a la nueva meta.
* Los resultados copiados se asignan al mismo propietario de forma predeterminada.
* No se puede copiar el progreso de la meta existente en una nueva.
* No puede copiar las actividades de una meta cuando copia una meta.

## Cómo copiar una meta

1. Haga clic en un nombre de meta para abrir **[!UICONTROL Detalles de meta]** panel.
1. Haga clic en el icono de 3 puntos y seleccione **[!UICONTROL Copiar]**.
1. Actualice cualquiera de la siguiente información para el objetivo copiado:
   * **Nueva meta**: es el nombre de la nueva meta. El valor predeterminado es el nombre del objetivo original.
   * **Periodo**: el período de tiempo durante el cual se desea alcanzar el objetivo. Seleccione un periodo de tiempo en el menú desplegable o haga clic en Definir fechas personalizadas para indicar un periodo de tiempo personalizado. El período predeterminado es siempre el trimestre actual.
   * **Propietario**: el propietario del objetivo. Puede ser un usuario, un equipo, un grupo o una empresa. El valor predeterminado es el propietario del objetivo original.
   * **Descripción**: información adicional sobre la meta.

1. Compruebe la **[!UICONTROL Copiar resultados]** cuadro si la meta original tenía resultados agregados y desea copiarlos en la nueva meta. Los resultados de la meta copiada tienen el mismo propietario, nombres y valores medidos que los resultados de la meta original.

1. Haga clic en **[!UICONTROL Guardar]**. La meta copiada se guardará con el estado Borrador.

   ![Una imagen de la [!UICONTROL Detalles de meta] panel en [!DNL Workfront Goals] con el [!UICONTROL Copiar] opción](assets/03-workfront-goals-copy-a-goal.png)

1. Clic **[!UICONTROL Activar]**, que actualiza el estado de la meta a Activo. El objetivo debe tener una actividad o resultado asociado para poder &quot;activarse&quot;.

1. Haga clic en **X** en la parte superior derecha de la etiqueta [!UICONTROL Detalles de meta] panel para cerrarlo.

Si ha copiado una meta que no se completó en un período de tiempo anterior y desea continuar trabajando en ella en el siguiente período de tiempo, haga lo siguiente:

1. Ir a la meta original en **[!UICONTROL Lista de metas]**, **[!UICONTROL Check-in]** sección, o **[!UICONTROL Pulse]** sección.
1. Comentario sobre la meta para indicar que se ha copiado y que se ha creado una meta más actual.
1. Cierre el objetivo original para conservar el progreso realizado durante su periodo de tiempo original. Haga clic en el icono de 3 puntos de la **[!UICONTROL Detalles de meta]** panel y seleccione **[!UICONTROL Cerrar]** en el menú.
1. Actualice el [!UICONTROL Inicial] valor del nuevo resultado que debe coincidir con el **[!UICONTROL Target]** valor del resultado anterior, de modo que el nuevo progreso de la meta comienza a calcular desde el punto alcanzado en el periodo anterior.
