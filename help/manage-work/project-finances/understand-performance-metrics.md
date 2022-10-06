---
title: Comprender las métricas de rendimiento
description: Las métricas de rendimiento son las [!UICONTROL Método de índice de rendimiento] ([!UICONTROL PIM]) y [!UICONTROL Estimación al finalizar] ([!UICONTROL EAC]).
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Comprender las métricas de rendimiento

Entre las dos métricas de rendimiento que utilizan los administradores de proyectos se incluye la variable [!UICONTROL Método de índice de rendimiento] ([!UICONTROL PIM]) y [!UICONTROL Estimación al finalizar] ([!UICONTROL EAC]). Los valores predeterminados de todo el sistema se pueden configurar en [!DNL Workfront] y se aplican a proyectos de nueva creación. [!UICONTROL PIM] se puede modificar en proyectos individuales.

**[!UICONTROL MIR]**

La configuración de la variable [!UICONTROL PIM] controlar cómo [!DNL Workfront] calcula otras métricas de rendimiento del proyecto, como la variable [!UICONTROL Índice de rendimiento de costes] ([!UICONTROL CPI]), [!UICONTROL Índice de rendimiento del programa de costo] ([!UICONTROL CSI]), [!UICONTROL Programar índice de rendimiento] ([!UICONTROL SPI]) y [!UICONTROL Estimación al finalizar] ([!UICONTROL EAC]).

Opciones para la variable [!UICONTROL PIM] están basados en horas y en costes.

* **Basado en horas** — Workfront utiliza las horas planificadas para calcular el CPI y la CAO del proyecto. La CAO del proyecto se muestra como un número, en horas.
* **Basado en los costes** — Workfront utiliza el coste laboral planificado para calcular el IPC y la CAO del proyecto. EAC aparece como un valor de moneda. Al utilizar esta opción, asegúrese de que los asignadores de tareas (usuarios o funciones de trabajo) estén asociados con las tasas de coste.

**[!UICONTROL CAE]**

[!UICONTROL EAC] representa el coste total previsto de la tarea o proyecto cuando se completa. Las opciones se calculan en el nivel de proyecto y se resumen desde tareas/subtareas.

* **Calcular en el nivel de proyecto** — [!UICONTROL EAC] para la tarea principal y el proyecto se determinan utilizando las horas/costes laborales reales en [!UICONTROL EAC] fórmulas. El cálculo incluye las horas/costes reales y los gastos añadidos directamente a la tarea o proyecto principal.
* R **configuración de tareas/subtareas** — [!UICONTROL EAC] para la tarea principal y el proyecto se determinan añadiendo la variable [!UICONTROL EAC] para cada tarea secundaria. Este cálculo excluye las horas/costes reales añadidos directamente a una tarea o proyecto principal.

La variable [!UICONTROL EAC] los cálculos se enumeran en &quot;Calcular estimación al finalizar (EAC)&quot; <!-- link to article -->artículo sobre [!UICONTROL [!DNL Workfront] One].

**Métricas de rendimiento: Configuración**

Para configurar [!UICONTROL PIM] y [!UICONTROL EAC] valores predeterminados del sistema:

1. Select **[!UICONTROL Configuración]** del menú principal.
1. Haga clic en **[!UICONTROL Preferencias de proyecto]** en el menú del panel izquierdo, haga clic en **[!UICONTROL Proyectos]**
1. En el [!UICONTROL Estado del proyecto] sección, buscar [!UICONTROL Método de índice de rendimiento]. Seleccione Basado en horas o en costes.
1. Para [!UICONTROL Estimación al finalizar], seleccione Calcular en el nivel de proyecto o Resumen de tareas/subtareas.
1. Haga clic en **[!UICONTROL Guardar]** en la parte inferior de la ventana.

![Una imagen del [!UICONTROL Preferencias de proyecto] pantalla](assets/setting-up-finances-1.png)

**Establezca [!UICONTROL PIM] sobre proyectos individuales**

1. Vaya a la página de aterrizaje de un proyecto.
1. Haga clic en **[!UICONTROL Detalles del proyecto]** del panel izquierdo.
1. Abra el **[!UICONTROL Finanzas]** para obtener más información.
1. Haga doble clic en el texto siguiente **[!UICONTROL Método de índice de rendimiento]** para editarlo.
1. Seleccione Basado en horas o en costes.
1. Haga clic en **[!UICONTROL Guardar]** Cambios para finalizar.

![Una imagen del [!UICONTROL Detalles del proyecto] pantalla](assets/setting-up-finances-2.png)

[!UICONTROL PIM] se puede configurar en una plantilla de proyecto, en la variable [!UICONTROL Finanzas] de los detalles de la plantilla.
