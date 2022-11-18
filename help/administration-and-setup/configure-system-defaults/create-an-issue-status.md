---
title: Crear un estado de problema
description: Obtenga información sobre cómo crear un estado de problema para satisfacer las necesidades de los flujos de trabajo de su organización.
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10019
exl-id: 1689080d-1d3c-4fad-a353-64fb3b0d5851
source-git-commit: 5fe0cbb9797ceaac0c402d912be6ed6665ac48ae
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Crear un estado de problema

[!DNL Workfront] recomienda modificar los estados de problemas existentes en el sistema antes de empezar a crear nuevos estados. Esto ayuda a limitar el número de estados que deben mantenerse.

1. Haga clic en **[!UICONTROL Configuración]** en el **[!UICONTROL Menú principal]**.
1. Expanda el **[!UICONTROL Preferencias de proyecto]** en el panel de menú de la izquierda.
1. Select **[!UICONTROL Estados]**.
1. Seleccione el **[!UICONTROL Problemas]** pestaña .
1. Asegúrese de que el campo de la esquina superior derecha está establecido en [!UICONTROL Estados del sistema]. Esto garantiza que el nuevo estado esté disponible globalmente en su [!DNL Workfront] instancia.
1. Select **[!UICONTROL Lista maestra]** para ver todos los estados del problema. Aquí es donde se crea o modifica un estado.
1. Haga clic en **[!UICONTROL Agregar un nuevo estado]**.
1. Complete los campos según sea necesario para su organización: nombre, descripción, color, coincide con, clave, etc.
1. Marque las casillas para el tipo de problema con el que se puede utilizar este estado.
1. Haga clic en **[!UICONTROL Guardar]**.

![Nueva ventana de estado activada [!UICONTROL Estados] página](assets/admin-fund-create-issue-status.png)

## Estados de problemas y administradores de grupos

Los administradores de grupos pueden crear y personalizar estados de problemas para los grupos que administran. Esto proporciona cierta autonomía a su grupo, proporcionándoles los estados que necesitan para seguir trabajando. También elimina la necesidad de una larga lista de estados de todo el sistema.

Los administradores de grupos pueden editar los estados existentes si el administrador del sistema los ha configurado para permitir la personalización.

Los administradores del sistema pueden administrar los estados de los grupos seleccionando el nombre del grupo en la esquina superior derecha de [!UICONTROL Estados] ventana.

![Menú de lista de grupos en [!UICONTROL Estados] página](assets/admin-fund-change-group-master-list.png)

Los administradores de grupos pueden hacer clic en [!UICONTROL Grupos] en la sección [!UICONTROL Configuración] , abra su grupo haciendo clic en el nombre y, a continuación, seleccionando [!UICONTROL Estados] en el menú del panel izquierdo. Asegúrese de seleccionar la pestaña Problemas .

![[!UICONTROL Estados] sección de [!UICONTROL Grupo] página](assets/admin-fund-group-issue-statuses.png)

<!---
For detailed information on how managing statuses can be done by group administrators, see these articles:
Create and customize group statuses
Group administrators
--->

<!---
learn more URLs
Issue statuses
Create and customize system-wide statuses
--->
