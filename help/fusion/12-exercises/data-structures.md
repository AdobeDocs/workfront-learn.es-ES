---
title: Estructuras de datos
description: Transformar datos de un archivo de origen a un archivo de destino. (Debe tener entre 60 y 160 caracteres, pero tiene 58)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11054
thumbnail: KT11054.png
exl-id: 06a39a87-23f3-4d4a-995e-d32fb9c5f50d
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# Estructuras de datos

Transformar datos de un archivo de origen a un archivo de destino.

## Resumen del ejercicio

Abra un archivo CSV que contenga una lista de entradas de tiempo. Estas entradas de tiempo son para minutos registrados a lo largo de ciertos días por varios usuarios. El objetivo es tomar esta información y generar un nuevo CSV que muestre el tiempo total, en horas, registrado por cada usuario, cada día.

![Estructuras de datos Imagen 1](../12-exercises/assets/data-structures-walkthrough-1.png)

![Estructuras de datos Imagen 2](../12-exercises/assets/data-structures-walkthrough-2.png)


En esta situación, abrirá un archivo que contiene una lista de entradas de tiempo para los minutos trabajados, incluida la fecha y la hora, la cantidad de minutos introducidos y la dirección de correo electrónico de quién realizó la entrada. Hay 100 entradas de tiempo, algunas hechas por los mismos individuos y algunas de ellas se hicieron el mismo día que otras.

Para generar un archivo que muestre el tiempo total, en horas, trabajado cada día por cada individuo, siga estos pasos:

1. En el módulo déclencheur, obtenga un archivo de la carpeta Workfront. Descargue el archivo.
1. En el primer módulo CSV, analice los datos de entrada de tiempo para generar un paquete para cada entrada de tiempo. Esto es un iterador.
1. El primer módulo Herramientas es un agregador numérico. Esto SUMARÁ todos los minutos y agrupará las filas por dirección de correo electrónico y luego por fecha. El resultado es el total de minutos trabajados cada día por dirección de correo electrónico.
1. El segundo módulo Herramientas es un módulo Establecer variable. Utilice esto para dar formato a los minutos para dividir por 60 y redondear a 2 decimales.
1. En el segundo módulo CSV, configure el archivo de salida.
1. En el módulo final, cargue el archivo CSV en Workfront.

## Pasos a seguir

**Descargue el archivo desde Workfront.**

1. En la carpeta &quot;Fusion Exercise Files&quot; de Workfront, seleccione &quot;_Fusion1.0JanTime.csv&quot; y haga clic en Detalles del documento.
1. Copie el primer número de ID de la dirección URL.
1. Cree un nuevo escenario. Asígnele el nombre &quot;Creación y uso de estructuras de datos&quot;.
1. Comience con el módulo Descargar documento desde la aplicación de Workfront.
1. Configure la conexión de Workfront e incluya el ID de documento que copió de la URL de Workfront.

   ![Estructuras de datos Imagen 3](../12-exercises/assets/data-structures-walkthrough-3.png)

   **Analice los datos de entrada de tiempo.**

1. Añada otro módulo, seleccionando Analizar CSV.
1. Configure Analizar CSV para 7 columnas. Marque la casilla CSV contiene encabezados. Elija Comma delimiterType y coloque Data en el campo CSV.

   ![Estructuras de datos Imagen 4](../12-exercises/assets/data-structures-walkthrough-4.png)

1. Haga clic en Ejecutar una vez para ver el resultado.
1. Abra el inspector de ejecución para ver las entradas y salidas del módulo Analizar CSV. Hay un paquete (un archivo CSV) como entrada y varios paquetes como salida (un paquete para cada fila en el archivo CSV). Debería tener un aspecto similar al siguiente:

   ![Estructuras de datos Imagen 5](../12-exercises/assets/data-structures-walkthrough-5.png)

   **A continuación, transforme los datos en el formulario de salida deseado, con los totales de tiempo agregados expresados en horas en lugar de minutos.**

1. Agregue un módulo de la herramienta Agregador numérico.
1. Seleccione el módulo de origen, que es el módulo Analizar CSV.
1. Seleccione SUM para la función de acumulado.
1. El campo Value es la columna 7 del archivo CSV. Son los minutos que registra cada usuario.
1. Para sumar los campos por grupo, haga clic en Advanced Settings y establezca Group by en email (columna 4), date (columna 5).

   + Esto suma todas las combinaciones del correo electrónico y la fecha. Asegúrese de colocar una coma entre la columna 4 y la columna 5. Se utilizará como delimitador más adelante.

   **El panel de asignación debería tener un aspecto similar al siguiente:**

   ![Estructuras de datos Imagen 6](../12-exercises/assets/data-structures-walkthrough-6.png)

1. Haga clic en Ejecutar una vez para comprobar el resultado de la agregación.

   **Los paquetes de salida deben tener este aspecto:**

   ![Estructuras de datos Imagen 7](../12-exercises/assets/data-structures-walkthrough-7.png)

   **Ahora, convierta los minutos acumulados en horas.**

1. Añada otro módulo de herramientas seleccionando Establecer variable.
1. Asigne a la variable el nombre &quot;Horas&quot;.
1. Establezca el valor de la variable en formatNumber(result/60;2;.;,)

   **El panel de asignación debería tener un aspecto similar al siguiente:**

   ![Estructuras de datos Imagen 8](../12-exercises/assets/data-structures-walkthrough-8.png)

   **A continuación, obtenga los valores configurados para el archivo de salida. Desea el userID y el valor de fecha utilizados para las agrupaciones. También desea las horas que se han calculado.**

1. Añada otro módulo-módulo CSV con el agregador Crear CSV (avanzado).
1. El módulo de origen es Herramientas - Agregador numérico.
1. Haga clic en Agregar junto al campo Estructura de datos y asigne a la estructura de datos el nombre &quot;Suma diaria registrada&quot;.
1. Haga clic en Agregar elemento para crear el primer elemento.
1. Asigne al elemento el nombre &quot;UserID&quot; y establezca el tipo en Text. Haga clic en Agregar.
1. Haga clic en Agregar elemento de nuevo para crear el segundo elemento.
1. Asigne al elemento el nombre &quot;Fecha&quot;, establezca el tipo en Fecha y haga clic en Agregar.
1. Haga clic en Agregar elemento una vez más.
1. Asigne al elemento el nombre &quot;Horas&quot;, establezca el tipo en Número y haga clic en Agregar.

   **La estructura de datos debería tener un aspecto similar al siguiente:**

   ![Estructuras de datos Imagen 9](../12-exercises/assets/data-structures-walkthrough-9.png)

1. Haga clic en Guardar para finalizar la estructura de datos Suma diaria registrada.

   **Ahora proporciona los valores de los tres campos que acaba de crear. Debería ver esos tres campos en el panel de asignación CSV.**

1. Haga clic en el campo UserID y seleccione GET en la pestaña de funciones generales. En el primer parámetro, coloque SPLIT desde la pestaña text and binary functions. El primer parámetro de la función SPLIT es el campo Key. Añada una coma como delimitador y 1 como índice. Esto indica que desea que la GET recupere el primer campo de la matriz de claves.
1. Copie esta expresión en el campo Date. GET Cambie el índice de 1 a 2 para obtener el segundo valor de la matriz.
1. Para el campo Horas, añada el campo Horas desde la herramienta Establecer variable.

   **El panel de asignación de CSV debe tener este aspecto:**

   ![Imagen 10 de estructuras de datos](../12-exercises/assets/data-structures-walkthrough-10.png)

   **Si ejecuta el escenario ahora, debería ver este resultado:**

   ![Imagen 11 de estructuras de datos](../12-exercises/assets/data-structures-walkthrough-11.png)

   **Ahora, agregue un módulo para tomar este resultado y cárguelo como un documento en un proyecto existente en Workfront.**

1. Abra el proyecto en Workfront y copie el ID de proyecto de la dirección URL.
1. Vuelva al escenario en Fusion y añada otro módulo: el módulo Cargar documento desde la aplicación de Workfront.
1. Pegue el ID del proyecto en el campo ID de registro relacionado.
1. Elija Proyecto para el tipo de registro relacionado.
1. Elija la opción Mapa para el archivo de origen.
1. Para el nombre del documento, utilice el nombre de archivo que descargó y agregue &quot;Actualizado&quot; delante de él.
1. Para el contenido del archivo, utilice el resultado Texto del módulo Crear CSV.

   **El panel de asignación debería tener un aspecto similar al siguiente:**

   ![Imagen 12 de estructuras de datos](../12-exercises/assets/data-structures-walkthrough-12.png)

1. Haga clic en Aceptar y guarde el escenario.
1. Haga clic en Ejecutar una vez para ejecutar el escenario.

   **Compruebe el inspector de ejecución en el módulo Cargar documento para confirmar que el documento se ha cargado.**

   ![Imagen 13 de estructuras de datos](../12-exercises/assets/data-structures-walkthrough-13.png)
