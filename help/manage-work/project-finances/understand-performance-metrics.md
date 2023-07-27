---
title: Comprender las métricas de rendimiento
description: 'Aprenda a utilizar las métricas de rendimiento: el [!UICONTROL Método de índice de rendimiento] ([!UICONTROL PIM]) y la [!UICONTROL Estimación al finalizar] ([!UICONTROL EAC]).'
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '433'
ht-degree: 100%

---

# Comprender las métricas de rendimiento

Entre las dos métricas de rendimiento que utilizan los administradores del proyecto se incluye el [!UICONTROL Método de índice de rendimiento] ([!UICONTROL PIM]) y la [!UICONTROL Estimación al finalizar] ([!UICONTROL EAC]). Los valores predeterminados de todo el sistema se pueden configurar en [!DNL Workfront] y se aplican a proyectos de nueva creación. El [!UICONTROL PIM] se puede modificar en proyectos individuales.

**[!UICONTROL GIP]**

La configuración del [!UICONTROL PIM] controla cómo [!DNL Workfront] calcula otras métricas de rendimiento del proyecto, como el [!UICONTROL Índice de rendimiento de costes] ([!UICONTROL CPI]), el [!UICONTROL Índice de rendimiento de la programación de costes] ([!UICONTROL CSI]), el [!UICONTROL Índice de rendimiento de la programación] ([!UICONTROL SPI]) y la [!UICONTROL Estimación al finalizar] ([!UICONTROL EAC]).

Las opciones para el [!UICONTROL PIM] están basadas en horas y en costes.

* **Basado en horas:** Workfront utiliza las horas planificadas para calcular el CPI y el EAC del proyecto. El EAC del proyecto se muestra como un número, en horas.
* **Basado en los costes:** Workfront utiliza el coste planificado de mano de obra para calcular el CPI y el EAC del proyecto. El EAC aparece como un valor de moneda. Al utilizar esta opción, asegúrese de que los destinatarios de las tareas (usuarios y funciones) estén asociados con las tasas de coste.

**[!UICONTROL EAC]**

El [!UICONTROL EAC] representa el coste total proyectado de la tarea o proyecto cuando se completa. Las opciones se calculan en el nivel de proyecto y se resumen desde tareas/subtareas.

* **Calcular en el nivel de proyecto:** el [!UICONTROL EAC] para la tarea principal y el proyecto se determinan utilizando las horas/costes laborales reales en las fórmulas del [!UICONTROL EAC]. El cálculo incluye las horas/costes reales y los gastos añadidos directamente a la tarea o proyecto principal.
* R **esumen de tareas/subtareas:** el [!UICONTROL EAC] para la tarea principal y el proyecto se determinan añadiendo el [!UICONTROL EAC] para cada tarea secundaria. Este cálculo excluye las horas/costes reales añadidos directamente a una tarea principal o proyecto.

Los cálculos [!UICONTROL EAC] se enumeran en [Calcular estimación al finalizar (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=es).

**Métricas de rendimiento: Configuración**

Para configurar los valores predeterminados del sistema [!UICONTROL PIM] y [!UICONTROL EAC], haga lo siguiente:

1. Seleccione **[!UICONTROL Configuración]** del menú principal.
1. Haga clic en **[!UICONTROL Preferencias de proyecto]** en el menú del panel izquierdo, y luego en **[!UICONTROL Proyectos]**
1. En la sección [!UICONTROL Estado del proyecto], busque [!UICONTROL Método de índice de rendimiento]. Seleccione Basado en horas o en costes.
1. Para [!UICONTROL Estimación al finalizar], seleccione Calcular en el nivel de proyecto o Resumen de tareas/subtareas.
1. Haga clic en **[!UICONTROL Guardar]** en la parte inferior de la ventana.

![Una imagen de la pantalla [!UICONTROL Preferencias del proyecto] ](assets/setting-up-finances-1.png)

**Establezca [!UICONTROL PIM] en proyectos individuales**

1. Vaya a la página de aterrizaje de un proyecto.
1. Haga clic en **[!UICONTROL Detalles del proyecto]** en el panel izquierdo.
1. Abra la sección **[!UICONTROL Finanzas]** para obtener más información.
1. Haga doble clic en el texto siguiente **[!UICONTROL Método de índice de rendimiento]** para editarlo.
1. Seleccione Basado en horas o en costes.
1. Haga clic en **[!UICONTROL Guardar]** Cambios para finalizar.

![Una imagen de la pantalla [!UICONTROL Detalles del proyecto] ](assets/setting-up-finances-2.png)

El [!UICONTROL PIM] se puede configurar en una plantilla de proyecto, en la sección [!UICONTROL Finanzas] de los detalles de la plantilla.
