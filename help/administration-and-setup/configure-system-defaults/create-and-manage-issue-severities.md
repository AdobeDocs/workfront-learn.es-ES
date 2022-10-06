---
title: Crear y administrar grupos de problemas
description: Obtenga información sobre cómo configurar y administrar las gravedad del problema.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: 5d385de5cdcee0d433304c09507ba6bb5b0a10e6
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 3%

---

# Crear y administrar grupos de problemas

## Introducción a la gravedad de los problemas

Se puede utilizar una gravedad para indicar la gravedad de un problema o cómo podría afectar al trabajo realizado.

![[!UICONTROL Gravedad] en el [!UICONTROL Detalles del problema] window](assets/admin-fund-severity-issue-details.png)

La variable [!UICONTROL Gravedad] se puede acceder al campo en la [!UICONTROL Detalles del problema]. También se puede incluir en las vistas de columnas de las listas y en los informes personalizados.

[!DNL Workfront] tiene cinco gravedad predeterminadas:

* [!UICONTROL Cosmético]
* [!UICONTROL Causa confusión]
* [!UICONTROL Error con solución]
* [!UICONTROL Error sin solución]
* [!UICONTROL Error fatal]

Los administradores del sistema pueden cambiar el nombre de estas gravedad predeterminadas o crear otras nuevas, si es necesario.

Las gravedad solo están disponibles para los problemas de [!DNL Workfront].

## Crear y administrar grupos de problemas

Como administrador del sistema, puede crear nuevas gravedad, si es necesario, para completar el flujo de trabajo del problema.

![[!UICONTROL Versiones] en [!UICONTROL Configuración]](assets/admin-fund-severity-section.png)

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expanda el **[!UICONTROL Preferencias de proyecto]** en el panel de menú de la izquierda.
1. Select **[!UICONTROL Versiones]**.
1. Haga clic en **[!UICONTROL Agregar una nueva gravedad]**.
1. Asigne un nombre a la gravedad que coincida con el uso deseado.
1. La variable **[!UICONTROL Importancia]** coincide con la gravedad del problema. El número más alto corresponde a la gravedad más alta. La variable [!UICONTROL Importancia] debe ser único.
1. Seleccione un color para la prioridad. Se utiliza en los informes de gráficos y en otros lugares de [!DNL Workfront].
1. Designe una de las opciones de gravedad como **[!UICONTROL Gravedad predeterminada]**. Esto se aplica automáticamente a todos los problemas nuevos en Workfront.
1. Incluya una descripción de la gravedad, como cómo se utilizará.
1. Haga clic fuera de los campos para guardar.

![[!UICONTROL Versiones] list](assets/admin-fund-severity-new.png)

### Modificación de gravámenes

Si una gravedad ya no es relevante para los flujos de trabajo del problema, se puede cambiar su nombre, ocultarla o eliminarla.

Si ya no se necesita una gravedad, [!DNL Workfront] recomienda ocultar la gravedad (haga clic en la [!UICONTROL Ocultar] junto a ella en el área de configuración). Esto elimina la opción de gravedad del menú desplegable del problema, pero conserva la gravedad de los datos históricos, por lo que aún está disponible para la generación de informes.

![[!UICONTROL Ocultar] columna resaltada en [!UICONTROL Versiones] en [!UICONTROL Configuración]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] recomienda que **no** elimine una gravedad que se haya utilizado en problemas anteriores. Cuando elimina una gravedad, se le pide que la sustituya por otra. Esto puede cambiar los datos históricos y afectar a los informes.

![Eliminar ventana de gravedad](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
