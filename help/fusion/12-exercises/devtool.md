---
title: Herramienta Desarrollo
description: Mejore sus capacidades para solucionar problemas de un escenario y facilitar configuraciones complejas mediante DevTool.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11057
thumbnail: KT11057.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---


# Herramienta Desarrollo

Mejore sus capacidades para solucionar problemas de un escenario y facilitar las configuraciones complejas mediante la herramienta de desarrollo.

## Información general del ejercicio

Instale y utilice las diferentes áreas de la herramienta Workfront Dev para profundizar en las solicitudes/respuestas realizadas y en los trucos avanzados de diseño de escenarios.

>[!NOTE]
>
>La herramienta de desarrollo de Workfront Fusion solo está disponible en el explorador Chrome cuando se usa la [Herramienta para desarrolladores Chrome](https://developer.chrome.com/docs/devtools/).

![Imagen de Devtool 1](../12-exercises/assets/devtool-walkthrough-1.png)

## Pasos a seguir

**Instale la herramienta Dev.**

1. Descargue el documento &quot;workfront-fusión-devtool.zip&quot; que se encuentra en la carpeta Fusion Exercise Files de la unidad de prueba.
1. Extraiga los archivos zip a una carpeta.
1. Abra una pestaña en Chrome e introduzca . **chrome://extensions**.
1. Alterne en el modo Desarrollador con el conmutador en la parte superior derecha y, a continuación, haga clic en el botón Cargar desempaquetado que aparece en la parte superior izquierda. Seleccione la carpeta que contiene la herramienta Dev (aquí es donde la descomprimió).

   ![Imagen de Devtool 2](../12-exercises/assets/devtool-walkthrough-2.png)

1. Una vez desempaquetada, la herramienta de desarrollo aparece entre las demás extensiones.

   ![Imagen de Devtool 3](../12-exercises/assets/devtool-walkthrough-3.png)

   **Utilice el flujo en directo.**

1. Comience abriendo el escenario &quot;Uso de Data Stores para sincronizar datos&quot;.
1. Abra la herramienta Dev escribiendo F12 o la función F12. O puede hacer clic en el menú de tres puntos de la barra de direcciones de Chrome y navegar a las herramientas para desarrolladores.

   ![Imagen de Devtool 4](../12-exercises/assets/navigate-to-devtools.png)

1. Haga clic en la ficha Workfront Fusion y, a continuación, seleccione Transmisión en directo en la lista de la izquierda.
1. Haga clic en Ejecutar una vez para ver los eventos a medida que se producen.
1. Haga clic en un evento para ver las pestañas a la derecha de Encabezados de solicitud, Cuerpo de solicitud, Encabezados de respuesta y Cuerpo de respuesta.

   ![Imagen de Devtool 4](../12-exercises/assets/devtool-walkthrough-4.png)

   **Uso de Scenario Debugger**

1. Seleccione Scenario Debugger y haga clic en un módulo para ver información sobre las operaciones de dicho módulo.

   ![Imagen de Devtool 5](../12-exercises/assets/devtool-walkthrough-5.png)

1. Vaya a la pestaña Historial . Haga clic en Detalles de una ejecución para examinar los detalles de operación del módulo para una ejecución específica.

   ![Imagen de Devtool 6](../12-exercises/assets/devtool-walkthrough-6.png)

   **Uso de las herramientas**

1. Vuelva al diseñador de escenarios y seleccione Herramientas en la herramienta Desarrollo. Muestra las herramientas disponibles.

   ![Imagen de Devtool 7](../12-exercises/assets/devtool-walkthrough-7.png)

+ Enfoque en un módulo : busque y abra un módulo rápidamente mediante el uso del ID de módulo.
+ Buscar módulos por asignación : busque un escenario con una palabra clave para encontrar valores asignados o claves en módulos.
+ Obtener metadatos de la aplicación : consulte un escenario los metadatos de la aplicación seleccionada.
+ Copiar asignación: copia la asignación de un módulo a otro. También puede clonar el módulo en el diseñador.
+ Copiar filtro : copia un filtro. El filtro siempre se asigna al módulo en el que está correctamente.
+ Conexión de intercambio : la herramienta toma la conexión del módulo seleccionado y establece la misma conexión con todos los módulos de la misma aplicación en el escenario. Esto resulta útil si tiene que cambiar la conexión en un escenario completado. Evite perder toda la asignación y ahorre tiempo con esta herramienta.
+ Variable de intercambio : busca todas las ocurrencias de la variable dada en todo el escenario, o en un módulo, y las reemplaza por la nueva. No se admiten caracteres comodín. Si ha asignado accidentalmente un valor a lo largo de todo el escenario, esto puede ayudarle a intercambiar fácilmente por el valor correcto.
+ Intercambiar aplicación: intercambia la aplicación dada por otra.
+ Base 64: codifique los datos introducidos en Base64 o descodifique Base64. Resulta útil cuando desea buscar datos concretos en la solicitud codificada.
+ Copiar nombre de módulo : copia el nombre de módulo seleccionado en el portapapeles.
+ Origen de reasignación : cambie el origen de la asignación de un módulo a otro. Primero debe añadir el módulo para utilizarlo como módulo de origen a la ruta en un escenario.
+ Migración del sistema operativo: se realiza específicamente para actualizar los módulos de hojas de Google (heredadas) a la última versión de hojas de Google. Añade una nueva versión del módulo justo después de la versión heredada del módulo en la ruta del escenario.
