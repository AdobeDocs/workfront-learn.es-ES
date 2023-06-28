---
title: Enrutadores
description: Comprenda la importancia de los enrutadores y cómo se pueden utilizar para procesar de forma condicional distintos módulos.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11043
thumbnail: KT11043.png
exl-id: f2a60273-c19b-4423-b354-8cff0dd7bd6b
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Enrutadores

Comprenda la importancia de los enrutadores y cómo se pueden utilizar para procesar de forma condicional distintos módulos.

## Resumen del ejercicio

Use un enrutador para pasar paquetes de Pokemon vs. superhéroes por la ruta correcta y luego cree una tarea para cada personaje.

![Imagen 1 de enrutadores](../12-exercises/assets/routers-walkthrough-1.png)

## Pasos a seguir

1. Clone el escenario Using universal connectors del ejercicio anterior. Asígnele el nombre &quot;Creación de diferentes rutas mediante enrutadores&quot;.

   **Cree una nueva ruta para los superhéroes clonando módulos y añadiendo un enrutador.**

   ![Imagen 2 de enrutadores](../12-exercises/assets/routers-walkthrough-2.png)

1. Haga clic con el botón derecho en el módulo Obtener información de Pokemon y seleccione Clonar. Una vez clonado, arrástrelo y conéctelo a la línea entre el nuevo módulo HTTP y el módulo Analizar CSV.

   >[!NOTE]
   >
   > Observe cómo agrega automáticamente un enrutador con dos rutas.

1. Asigne un nombre a este módulo &quot;Obtener la apariencia de superhéroe&quot;.
1. Clona este módulo, mueve el clon a la derecha y ponle el nombre &quot;Consigue habilidades de superhéroe&quot;.
1. Clone el módulo Herramientas y muévalo al final de la segunda ruta.
1. Haga clic en el icono de la varita (el botón Alineación automática ) en la barra de herramientas.

   **El escenario debería tener este aspecto:**

   ![Imagen 3 de enrutadores](../12-exercises/assets/routers-walkthrough-3.png)

   **A continuación, va a cambiar los valores asignados en los nuevos módulos clonados.**

1. Ir a <https://www.superheroapi.com/> y use su cuenta de Facebook para obtener un token de acceso.

   >[!NOTE]
   >
   >Si tiene problemas para acceder a su propio token de superhéroe, puede utilizar este token compartido: 10110256647253588. Tenga en cuenta cuántas veces llama a la API de superhéroes para que este token compartido siga funcionando para todos.

1. Abra la configuración de Obtener apariencia de superhéroe y cambie la dirección URL a `https://www.superheroapi.com/api/[access- token]/332/appearance`. Asegúrese de incluir el token de acceso en la dirección URL. Haga clic en Aceptar.
1. Abra la configuración de Obtener capacidades de superhéroes y cambie la dirección URL a `https://www.superheroapi.com/api/[access- token]/332/powerstats`. Asegúrese de incluir el token de acceso en la dirección URL. Haga clic en Aceptar.
1. Haga clic con el botón derecho en cada módulo de superhéroes y seleccione Ejecutar solo este módulo. Esto generará la estructura de datos que necesita ver para la asignación.
1. Después de ejecutar ambos, cambie el número &quot;332&quot; en cada campo URL a la Columna 4 asignada desde el módulo Analizar CSV.

   ![Imagen 4 de enrutadores](../12-exercises/assets/routers-walkthrough-4.png)

   **Ahora puede hacer clic en el módulo Establecer varias variables en la ruta de superhéroes y actualizar el nombre, la altura, el peso y las capacidades.**

1. Actualice los campos Nombre y Habilidades desde el módulo Obtener habilidades de superhéroes: Módulo 8.

   ![Imagen 5 de enrutadores](../12-exercises/assets/routers-walkthrough-5.png)

1. Actualice los campos Altura y Peso desde el módulo Obtener apariencia de superhéroes: Módulo 6.

   ![Imagen 6 de enrutadores](../12-exercises/assets/routers-walkthrough-6.png)

   **Cuando haya terminado, las variables deberían tener este aspecto. Tenga en cuenta que los números de módulo aparecen en los valores de campo.**

   ![Imagen 7 de enrutadores](../12-exercises/assets/routers-walkthrough-7.png)

1. Haga clic en Aceptar y guarde el escenario.

   **Cree otra ruta para crear una tarea por carácter.**

1. En Workfront, cree un proyecto vacío. Asígnele el nombre &quot;Proyecto de manifiesto de envío&quot; y copie el ID de proyecto de la dirección URL.
1. Vuelva a Workfront Fusion y haga clic en el centro del enrutador para crear otra ruta.

   ![Imagen 8 de enrutadores](../12-exercises/assets/routers-walkthrough-8.png)

1. Haga clic en el centro del módulo vacío que aparece y agregue un módulo Crear registro desde la aplicación de Workfront.
1. Establezca el Tipo de registro en Tarea y seleccione ID de proyecto en la sección Campos a asignar.
1. Pegue el ID de proyecto que copió de Workfront en el campo ID de proyecto.
1. A continuación, seleccione el campo Nombre de la sección Campos a asignar.
1. Asigne un nombre a la tarea &quot;[Carácter] de [Franquicia],&quot; tomando el nombre del carácter y el nombre de la franquicia del archivo CSV. Column 3 es el nombre del carácter y column 2 es el nombre de la franquicia.

   ![Imagen 9 de enrutadores](../12-exercises/assets/routers-walkthrough-9.png)

1. Haga clic en Aceptar y cambie el nombre de este módulo a &quot;Crear una tarea para cada carácter&quot;.

   **Añada filtros para que el escenario se pueda ejecutar sin errores. Quieres que solo los personajes de Pokémon vayan por el camino superior, solo los personajes de superhéroes vayan por el camino medio, y todos los personajes vayan por el camino inferior.**

1. Haga clic en la línea de puntos a la izquierda del módulo Obtener información de Pokemon para crear el primer filtro. Asígnele el nombre &quot;Pokemon character&quot;.
1. Para la condición, solo permita registros donde la franquicia (Columna 2) sea igual a &quot;Pokemon&quot;. Elija el operador de texto &quot;Igual a&quot;.
1. Haga clic en la línea de puntos a la izquierda del módulo Obtener apariencia de superhéroe para crear el siguiente filtro. Nómbralo &quot;personaje de superhéroe&quot;.
1. Dado que los superhéroes pueden provenir de varias franquicias, utilice el campo ID de superhéroe (Columna 4) para determinar si un personaje es un superhéroe o no.

   **Los filtros deberían tener un aspecto similar al siguiente:**

   ![Imagen 11 de enrutadores](../12-exercises/assets/routers-walkthrough-11.png)

   ![Imagen 10 de enrutadores](../12-exercises/assets/routers-walkthrough-10.png)

1. Guarde el escenario y haga clic en Ejecutar una vez. Utilice los inspectores de ejecución para comprobar que todas las operaciones se han realizado correctamente y comprobar las tareas creadas en el proyecto de Workfront.

   ![Imagen 12 de enrutadores](../12-exercises/assets/routers-walkthrough-12.png)
