---
title: Copiar un objetivo existente
description: Obtenga información sobre cómo copiar un objetivo existente en [!DNL Workfront Goals].
activity: use
team: Technical Marketing
feature: Workfront Goals
type: Tutorial
role: User
level: Beginner
kt: 10121
exl-id: bf9ac10a-8419-458b-b4e8-bedb0ad3b98f
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Copiar un objetivo existente

Digamos que es el final de un trimestre y queremos recrear un objetivo existente para el próximo período. O tal vez no completaste el objetivo y necesitabas extender hasta el siguiente período de tiempo. ¿Cuál es la mejor opción para crear ese objetivo? Desea copiar y modificar un objetivo existente.

Copiar un objetivo existente también es útil si varios integrantes del equipo tienen objetivos similares y necesita crear un objetivo para cada uno de ellos.

<!--
Pro-tips graphic
-->

Estas son algunas cosas que hay que tener en cuenta antes de copiar los objetivos:

* Toda la información del objetivo original se copiará, con la excepción del periodo de objetivo (porque es en el pasado).
* Puede copiar los resultados de un objetivo existente y se transferirán al nuevo objetivo.
* Los resultados copiados se asignan al mismo propietario de forma predeterminada.
* No se puede copiar el progreso del objetivo existente en un nuevo objetivo.
* No se pueden copiar las actividades de un objetivo al copiar un objetivo.

## Cómo copiar un objetivo

1. Haga clic en un nombre de objetivo para abrir **[!UICONTROL Detalles del objetivo]** panel.
1. Haga clic en el icono de 3 puntos y, a continuación, seleccione **[!UICONTROL Copiar]**.
1. Actualice cualquiera de la siguiente información para el objetivo copiado:
   * **Nuevo objetivo**—Este es el nombre del nuevo objetivo. El valor predeterminado es el nombre del objetivo original.
   * **Periodo**: el período de tiempo durante el cual desea alcanzar el objetivo. Seleccione un período de tiempo en el menú desplegable o haga clic en Definir fechas personalizadas para indicar un período de tiempo personalizado. El periodo predeterminado siempre es el trimestre actual.
   * **Propietario**: el propietario del objetivo. Puede ser un usuario, equipo, grupo o empresa. El valor predeterminado es el propietario del objetivo original.
   * **Descripción**: información adicional sobre el objetivo.

1. Marque la **[!UICONTROL Copiar resultados]** si el objetivo original tenía resultados agregados y desea copiarlos en el nuevo objetivo. Los resultados del objetivo copiado tienen el mismo propietario, nombres y valores medidos que los resultados del objetivo original.

1. Haga clic en **[!UICONTROL Guardar]**. El objetivo copiado se guarda con el estado Borrador.

   ![Una imagen del [!UICONTROL Detalles del objetivo] panel en [!DNL Workfront Goals] con la variable [!UICONTROL Copiar] option](assets/03-workfront-goals-copy-a-goal.png)

1. Haga clic en **[!UICONTROL Activar]**, que actualiza el estado del objetivo a Activo. El objetivo debe tener una actividad asociada o un resultado para &quot;activar&quot;.

1. Haga clic en el **X** en la parte superior derecha del [!UICONTROL Detalles del objetivo] para cerrarlo.

Si ha copiado un objetivo que no se completó en un período de tiempo anterior y desea continuar trabajando en él en el siguiente período de tiempo, haga lo siguiente:

1. Vaya al objetivo original en la **[!UICONTROL Lista de objetivos]**, **[!UICONTROL Registro]** o **[!UICONTROL Pulse]** para obtener más información.
1. Comente el objetivo para indicar que se copió y se creó un objetivo más actual.
1. Cierre el objetivo original para preservar el progreso realizado durante su período de tiempo original. Haga clic en el icono de 3 puntos de la sección **[!UICONTROL Detalles del objetivo]** panel y seleccione **[!UICONTROL Cerrar]** del menú .
1. Actualice el [!UICONTROL Inicial] del nuevo resultado para que coincida con la variable **[!UICONTROL Target]** del resultado anterior, por lo que el nuevo progreso del objetivo comienza a calcularse a partir del punto alcanzado en el periodo anterior.
