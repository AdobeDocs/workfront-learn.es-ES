---
title: Ruteadores
description: Comprender la importancia de los enrutadores y cómo pueden utilizarse para procesar condicionalmente distintos módulos.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11043
thumbnail: KT11043.png
exl-id: f2a60273-c19b-4423-b354-8cff0dd7bd6b
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Ruteadores

Comprender la importancia de los enrutadores y cómo pueden utilizarse para procesar condicionalmente distintos módulos.

## Información general del ejercicio

Utilice un router para pasar paquetes Pokemon vs. superhéroes por la ruta correcta y luego cree una tarea para cada carácter.

![Routers Image 1](../12-exercises/assets/routers-walkthrough-1.png)

## Pasos a seguir

1. Clona el escenario Usar conectores universales del ejercicio anterior. Denomínela &quot;Creación de diferentes rutas mediante enrutadores&quot;.

   **Cree una nueva ruta para superhéroes clonando módulos y agregando un router.**

   ![Imagen 2 de enrutadores](../12-exercises/assets/routers-walkthrough-2.png)

1. Haga clic con el botón derecho en el módulo Get Pokemon info y seleccione Clone. Una vez clonado, arrástrelo y conéctelo a la línea entre el nuevo módulo HTTP y el módulo CSV Parse.

   >[!NOTE]
   >
   > Observe cómo agrega automáticamente un router con dos rutas.

1. Asigne a este módulo el nombre &quot;Obtener apariencia de superhéroe&quot;.
1. Clone este módulo, mueva el clon a la derecha y llámelo &quot;Get superhero abilities&quot;.
1. Clona el módulo Herramientas y muévalo al final de la segunda ruta.
1. En la barra de herramientas, haga clic en el icono de varita (botón Alinear automáticamente ).

   **El escenario debería tener este aspecto:**

   ![Imagen de enrutadores 3](../12-exercises/assets/routers-walkthrough-3.png)

   **A continuación, cambiará los valores asignados en los nuevos módulos clonados.**

1. Vaya a <https://www.superheroapi.com/> y use su cuenta de Facebook para obtener un token de acceso.

   >[!NOTE]
   >
   >Si tiene problemas para acceder a su propio token de superhéroe, puede utilizar este token compartido: 10110256647253588. Tenga en cuenta cuántas veces llama a la API de superhéroe para que este token compartido siga funcionando para todos.

1. Abra la configuración de Obtener apariencia de superhéroe y cambie la URL a `https://www.superheroapi.com/api/[access- token]/332/appearance`. Asegúrese de incluir el token de acceso en la dirección URL. Haga clic en Aceptar.
1. Abra la configuración de las capacidades de Obtener superhéroe y cambie la dirección URL a `https://www.superheroapi.com/api/[access- token]/332/powerstats`. Asegúrese de incluir el token de acceso en la dirección URL. Haga clic en Aceptar.
1. Haga clic con el botón derecho en cada módulo superhéroe y seleccione Ejecutar este módulo únicamente. Esto generará la estructura de datos que debe ver para la asignación.
1. Después de ejecutar ambos, cambie el número &quot;332&quot; en cada campo URL a la Columna 4 asignada desde el módulo CSV de análisis.

   ![Imagen de enrutadores 4](../12-exercises/assets/routers-walkthrough-4.png)

   **Ahora puede hacer clic en el módulo Set multiple variables en la ruta de superhéroe y actualizar el nombre, la altura, el peso y las capacidades.**

1. Actualice los campos Nombre y Funciones del módulo Get superhero abilities: Módulo 8.

   ![Imagen 5 de enrutadores](../12-exercises/assets/routers-walkthrough-5.png)

1. Actualice los campos Alto y Peso desde el módulo Obtener apariencia de superhéroe: Módulo 6.

   ![Imagen de enrutadores 6](../12-exercises/assets/routers-walkthrough-6.png)

   **Cuando haya terminado, las variables deberían tener este aspecto. Tenga en cuenta que los números de módulo aparecen en los valores de campo.**

   ![Routers Image 7](../12-exercises/assets/routers-walkthrough-7.png)

1. Haga clic en Aceptar y, a continuación, guarde el escenario.

   **Cree otra ruta para crear una tarea por carácter.**

1. En Workfront, cree un proyecto vacío. Asígnele el nombre &quot;Proyecto de manifiesto de envío&quot; y copie el ID del proyecto de la dirección URL.
1. Vuelva a Workfront Fusion y haga clic en el centro del enrutador para crear otra ruta.

   ![Imagen 8 de enrutadores](../12-exercises/assets/routers-walkthrough-8.png)

1. Haga clic en el centro del módulo vacío que aparece y añada un módulo Crear registro desde la aplicación de Workfront.
1. Establezca el Tipo de registro en Tarea y seleccione ID de proyecto en la sección Campos en Asignar .
1. Pegue el ID del proyecto que ha copiado de Workfront en el campo ID del proyecto .
1. Ahora, seleccione el campo Nombre de la sección Campos a asignar .
1. Asigne un nombre a la tarea &quot;[Carácter] from [Franquicia],&quot; tomando el nombre del carácter y el nombre de la franquicia del archivo CSV. La columna 3 es el nombre del carácter y la columna 2 es el nombre de la franquicia.

   ![Imagen de enrutadores 9](../12-exercises/assets/routers-walkthrough-9.png)

1. Haga clic en Aceptar y cambie el nombre de este módulo a &quot;Crear una tarea para cada carácter&quot;.

   **Añada filtros para que el escenario se pueda ejecutar sin errores. Solo quieres que los caracteres Pokemon bajen por el camino superior, solo los caracteres superhéroes bajen por el camino medio, y todos los caracteres vayan por el camino inferior.**

1. Haga clic en la línea de puntos a la izquierda del módulo Get Pokemon info para crear el primer filtro. Denomínela &quot;Carácter Pokemon&quot;.
1. Para la condición, solo permita registros donde la franquicia (Columna 2) sea igual a &quot;Pokemon&quot;. Elija el operador de texto &quot;Equal to&quot;.
1. Haga clic en la línea de puntos a la izquierda del módulo Obtener apariencia de superhéroe para crear el siguiente filtro. Denomínela &quot;Carácter de superhéroe&quot;.
1. Dado que los superhéroes pueden provenir de varias franquicias, utilice el campo ID de superhéroe (columna 4) para determinar si un carácter es o no un superhéroe.

   **Los filtros deberían tener este aspecto:**

   ![Imagen de enrutadores 11](../12-exercises/assets/routers-walkthrough-11.png)

   ![Imagen de enrutadores 10](../12-exercises/assets/routers-walkthrough-10.png)

1. Guarde el escenario y haga clic en Ejecutar una vez. Utilice los inspectores de ejecución para comprobar que todas las operaciones se han realizado correctamente y las tareas que se crearon en el proyecto de Workfront.

   ![Imagen de enrutadores 12](../12-exercises/assets/routers-walkthrough-12.png)
