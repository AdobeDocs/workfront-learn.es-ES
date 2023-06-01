---
title: Comprender las métricas de rendimiento
description: 'Aprenda a utilizar las métricas de rendimiento: [!UICONTROL Método de índice de rendimiento] ([!UICONTROL PIM]) y el [!UICONTROL Estimar al finalizar] ([!UICONTROL EAC]).'
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: 65bd26fefb280d12ec44a4923f6d96ac8d88d6fb
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Comprender las métricas de rendimiento

Dos métricas de rendimiento utilizadas por los jefes de proyecto son [!UICONTROL Método de índice de rendimiento] ([!UICONTROL PIM]) y el [!UICONTROL Estimar al finalizar] ([!UICONTROL EAC]). Los valores predeterminados de todo el sistema se pueden establecer en [!DNL Workfront] y se aplican a los proyectos recién creados. [!UICONTROL PIM] se pueden modificar en proyectos individuales.

**[!UICONTROL MIR]**

La configuración del [!UICONTROL PIM] controlar cómo [!DNL Workfront] calcula otras métricas de rendimiento del proyecto, como la variable [!UICONTROL Índice de rendimiento de costes] ([!UICONTROL IRC]), [!UICONTROL Índice de rendimiento del horario de costes] ([!UICONTROL CSI]), [!UICONTROL Índice de rendimiento del horario] ([!UICONTROL SPI]), y [!UICONTROL Estimar al finalizar] ([!UICONTROL EAC]).

Opciones de la [!UICONTROL PIM] se basan en horas y en costes.

* **Basado en horas** — Workfront utiliza las horas planificadas para calcular el IPC y el EAC del proyecto. El EAC del proyecto se muestra como un número, en horas.
* **Basado en costes** — Workfront utiliza el coste laboral previsto para calcular el IPC y el EAC del proyecto. EAC aparece como un valor de moneda. Al utilizar esta opción, asegúrese de que las personas asignadas a la tarea (usuarios o funciones del puesto) estén asociadas a las tasas de coste.

**[!UICONTROL CAE]**

[!UICONTROL EAC] representa el costo total proyectado de la tarea o proyecto cuando finaliza. Las opciones se calculan en el nivel de proyecto y se resumen a partir de tareas/subtareas.

* **Calcular a nivel de proyecto** — [!UICONTROL EAC] para la tarea y el proyecto principales se determinan utilizando las horas reales/los costes laborales reales en [!UICONTROL EAC] fórmulas. El cálculo incluye las horas/costos reales y los gastos agregados directamente a la tarea o proyecto principal.
* R **resumir a partir de tareas/subtareas** — [!UICONTROL EAC] para la tarea y el proyecto principales se determinan añadiendo el [!UICONTROL EAC] para cada tarea secundaria. Este cálculo excluye las horas/costos reales agregados directamente a una tarea o proyecto principal.

El [!UICONTROL EAC] cálculos se enumeran en [Calcular estimación al finalizar (EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**Métricas de rendimiento: Configuración**

Para establecer [!UICONTROL PIM] y [!UICONTROL EAC] valores predeterminados del sistema:

1. Seleccionar **[!UICONTROL Configurar]** en el menú principal.
1. Clic **[!UICONTROL Preferencias de proyecto]** en el menú del panel izquierdo, haga clic en **[!UICONTROL Proyectos]**
1. En el [!UICONTROL Estado del proyecto] sección, buscar [!UICONTROL Método de índice de rendimiento]. Seleccione Basado en horas o Basado en costos.
1. Para [!UICONTROL Estimar al finalizar], seleccione Calcular a nivel de proyecto o Resumir a partir de tareas/subtareas.
1. Clic **[!UICONTROL Guardar]** en la parte inferior de la ventana.

![Una imagen de la [!UICONTROL Preferencias de proyecto] pantalla](assets/setting-up-finances-1.png)

**Establecer [!UICONTROL PIM] en proyectos individuales**

1. Vaya a la página de aterrizaje de un proyecto.
1. Clic **[!UICONTROL Detalles del proyecto]** en el panel izquierdo.
1. Abra el **[!UICONTROL Finanzas]** sección.
1. Haga doble clic en el texto siguiente **[!UICONTROL Método de índice de rendimiento]** para editarlo.
1. Seleccione Basado en horas o Basado en costos.
1. Clic **[!UICONTROL Guardar]** Cambios para finalizar.

![Una imagen de la [!UICONTROL Detalles del proyecto] pantalla](assets/setting-up-finances-2.png)

[!UICONTROL PIM] se puede configurar en una plantilla de proyecto, en el [!UICONTROL Finanzas] de los detalles de la plantilla.
