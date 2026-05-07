---
title: Ejercicio de Exploración de ejecuciones, ciclos y paquetes
description: Comprenda cómo se comportan las ejecuciones, los ciclos y los paquetes mediante el historial de ejecución de un escenario.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:39.670Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 344
ht-degree: 100%

---

# Ejercicio de Exploración de ejecuciones, ciclos y paquetes

Comprenda cómo se comportan las ejecuciones, los ciclos y los paquetes mediante el historial de ejecución de un escenario.

## Información general del ejercicio

Práctica con diferentes configuraciones de escenario para explorar mediante ejecuciones y ciclos.

![Imagen 1 de Exploración de ciclos de ejecución y paquetes](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## Pasos a seguir

1. Clonar el escenario llamado “Uso compartido de variables entre rutas de enrutamiento”. Asigne un nombre al nuevo escenario “Variables de uso compartido entre rutas de enrutamiento: prueba de ciclos”.
1. Elimine el módulo Enviar un correo electrónico, ya que no es necesario para esta prueba.

   **Configure el escenario para procesar tres ciclos por ejecución. Procese cinco proyectos en cada ciclo.**

1. Haga clic en el módulo activador y cambie el campo Máximo a 5, por lo que solo se procesan cinco proyectos en cada ciclo.
1. En los criterios de búsqueda, elimine el segundo filtro que restringe la búsqueda a un solo proyecto.
1. Haga clic en Aceptar.

1. En la barra de herramientas de Fusion, abra Configuración del escenario y cambie el campo Número máximo de ciclos de 1 a 3.
1. Haga clic en Aceptar.

   ![Imagen 1 de Exploración de ciclos de ejecución y paquetes](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **Programar el escenario para que se ejecute a cada minuto.**

1. Haga clic en el icono del reloj situado junto al módulo activador y cambie el campo Minutos a 1 minuto.

   ![Imagen 2 de Exploración de ciclos de ejecución y paquetes](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. A continuación, cambie la opción de Programación debajo del botón Ejecutar una vez a Activado. Guarde el escenario.

   ![Imagen 3 Exploración de ciclos de ejecución y paquetes](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. Vaya al historial de ejecución del escenario y observe cómo aparece un nuevo registro de historial en el minuto siguiente. Es posible que deba actualizar la página.

   ![Imagen 1 de Exploración de ciclos de ejecución y paquetes](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. Haga clic en el botón Detalles de una ejecución. Haga clic en el registro Simple del panel derecho, similar a lo que hizo en la parte del historial de ejecución de la formación de Workfront Fusion.
1. Los registros de operaciones procesadas se dividen en ciclos.

   ![Imagen 5 de Exploración de ciclos de ejecución y paquetes](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. Un menú desplegable en la parte superior derecha de la ventana le permite seleccionar cualquiera de los 3 ciclos que ha configurado para que se ejecuten cada vez.

   ![Imagen 6 Exploración de ciclos de ejecución y paquetes](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
