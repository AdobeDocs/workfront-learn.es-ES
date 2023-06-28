---
title: Crear y administrar gravedades de problemas
description: Obtenga información sobre cómo configurar y administrar gravedades de problemas.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 3%

---

# Crear y administrar gravedades de problemas

## Introducción a las gravedades de los problemas

Una gravedad se puede utilizar para indicar la gravedad de un problema o cómo podría afectar al trabajo realizado.

![[!UICONTROL Gravedad] en el menú [!UICONTROL Detalles del problema] ventana](assets/admin-fund-severity-issue-details.png)

El [!UICONTROL Gravedad] se puede acceder a este campo en la [!UICONTROL Detalles del problema]. También se puede incluir en las vistas de columnas de las listas y en los informes personalizados.

[!DNL Workfront] tiene cinco gravedades predeterminadas:

* [!UICONTROL Cosmético]
* [!UICONTROL Causa confusión]
* [!UICONTROL Error con solución]
* [!UICONTROL Error sin solución]
* [!UICONTROL Error fatal]

Los administradores del sistema pueden cambiar el nombre de estas gravedades predeterminadas o crear otras nuevas, si es necesario.

Las gravedades solo están disponibles para los problemas de [!DNL Workfront].

## Crear y administrar gravedades de problemas

Como administrador del sistema, puede crear nuevas gravedades, si es necesario, para completar el flujo de trabajo del problema.

![[!UICONTROL Gravedades] página en [!UICONTROL Configurar]](assets/admin-fund-severity-section.png)

1. Clic **[!UICONTROL Configurar]** en el **[!UICONTROL Menú principal]**.
1. Expanda el **[!UICONTROL Preferencias de proyecto]** en el panel de menú izquierdo.
1. Seleccionar **[!UICONTROL Gravedades]**.
1. Clic **[!UICONTROL Añadir una gravedad nueva]**.
1. Asigne a la gravedad un nombre que coincida con su uso previsto.
1. El **[!UICONTROL Importancia]** El número coincide con la gravedad del problema. El número más alto corresponde a la gravedad más alta. El [!UICONTROL Importancia] el número debe ser único.
1. Seleccione un color para su prioridad. Se utiliza en informes de gráficos y otros lugares de [!DNL Workfront].
1. Designe una de las opciones de gravedad como **[!UICONTROL Gravedad predeterminada]**. Esto se aplica automáticamente a todos los problemas nuevos de Workfront.
1. Incluya una descripción de la gravedad, como su uso.
1. Haga clic fuera de los campos para guardar.

![[!UICONTROL Gravedades] lista](assets/admin-fund-severity-new.png)

### Modificación de gravedades

Si una gravedad ya no es relevante para los flujos de trabajo de problemas, se puede cambiar el nombre, ocultarla o eliminarla.

Si ya no se necesita una gravedad, [!DNL Workfront] recomienda ocultar la gravedad (haga clic en el botón [!UICONTROL Hide] situado junto a él en el área de configuración). Esto elimina la opción gravedad del menú desplegable del problema, pero mantiene la gravedad en los datos históricos, por lo que aún está disponible para la creación de informes.

![[!UICONTROL Hide] columna resaltada en [!UICONTROL Gravedades] página en [!UICONTROL Configurar]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] recomienda que **no** elimine una gravedad que se haya utilizado en problemas anteriores. Cuando elimina una gravedad, le pide que sustituya otra gravedad. Esto puede cambiar los datos históricos y afectar a la creación de informes.

![Ventana Eliminar gravedad](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
