---
title: Estructuras de datos
description: Transformar datos de un archivo de origen a un archivo de destino. (Debe tener entre 60 y 160 caracteres, pero tiene 58 caracteres)
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
workflow-type: ht
source-wordcount: '1048'
ht-degree: 100%

---

# Estructuras de datos

Transformar datos de un archivo de origen a un archivo de destino.

## Información general del ejercicio

Abra un archivo CSV que contenga una lista de entradas de tiempo. Estas entradas de tiempo son para los minutos para los que varios usuarios se registran a lo largo de ciertos días. El objetivo es tomar esta información y producir un nuevo CSV que muestre el tiempo total, en horas, en las que cada usuario se ha registrado cada día.

![Imagen 1 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-1.png)

![Imagen 2 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-2.png)


En esta situación, se abrirá un archivo que contenga una lista de entradas de tiempo por minutos de trabajo, incluida la fecha y la hora, cuántos minutos se escribieron y la dirección de correo electrónico de quién realizó la entrada. Hay 100 entradas de tiempo, algunas hechas por las mismas personas y otras el mismo día que otras.

Para producir un archivo que muestre el tiempo total, en horas, trabajado cada día por cada individuo, siga estos pasos:

1. En el módulo activador, obtenga un archivo de la carpeta Workfront. Descargue el archivo.
1. En el primer módulo CSV, analice los datos de entrada de tiempo para generar un paquete para cada entrada de tiempo. Este es un iterador.
1. El primer módulo Herramientas es un agregador numérico. Esto SUMA todos los minutos y agrupa las filas por dirección de correo electrónico y, a continuación, por fecha. El resultado es el total de minutos trabajados cada día por dirección de correo electrónico.
1. El segundo módulo de Herramientas es el módulo de la variable Set. Utilice esto para dar formato a los minutos que se dividirán entre 60 y redondee a 2 decimales.
1. En el segundo módulo CSV, configure el archivo de resultados.
1. En el módulo final, cargue el archivo CSV en Workfront.

## Pasos a seguir

**Descargue el archivo desde Workfront.**

1. En la carpeta “Archivos de ejercicio de Fusion” de Workfront, seleccione “_Fusion1.0JanTime.csv” y haga clic en Detalles del documento.
1. Copie el primer número de ID de la dirección URL.
1. Crear un nuevo escenario. Asígnele el nombre “Creación y uso de estructuras de datos”.
1. Comience con el módulo Descargar documento de la aplicación Workfront.
1. Configure la conexión de Workfront e incluya el ID de documento que ha copiado de la URL de Workfront.

   ![Imagen 3 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-3.png)

   **Analice los datos de entrada de tiempo.**

1. Añada otro módulo seleccionando Analizar CSV.
1. Configure Analizar CSV para siete columnas. Compruebe si la casilla CSV contiene encabezados. Elija el tipo de delimitador por coma y coloque los datos en el campo CSV.

   ![Imagen 4 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-4.png)

1. Haga clic en Ejecutar una vez para ver el resultado.
1. Abra el inspector de ejecución para ver las entradas y salidas del módulo Analizar CSV. Hay un paquete (un archivo CSV) como entrada y varios paquetes como salidas (un paquete para cada fila en el archivo CSV). Debería tener un aspecto similar al siguiente:

   ![Imagen 5 Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-5.png)

   **A continuación, transforme los datos en el formulario de salida deseado, con totales de tiempo agregados expresados en horas en lugar de minutos.**

1. Agregue un módulo de la herramienta del Agregador numérico.
1. Seleccione el módulo de origen, que es el módulo Analizar CSV.
1. Seleccione SUMA para la función de agregado.
1. El campo Valor es la columna 7 del archivo CSV. Son los minutos que registra cada usuario.
1. Para sumar los campos por grupo, haga clic en Configuración avanzada y establezca Agrupar por correo electrónico (columna 4), fecha (columna 5).

   + Esto sumará para cada combinación del correo electrónico y la fecha. Asegúrese de colocar una coma entre la columna 4 y la columna 5. Esto se utilizará como delimitador más adelante.

   **El panel de asignación debe tener este aspecto:**

   ![Imagen 6 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-6.png)

1. Haga clic en Ejecutar una vez para comprobar el resultado de la agregación.

   **Los paquetes de resultados deberían tener este aspecto:**

   ![Imagen 7 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-7.png)

   **Ahora, convierta los minutos agregados en horas.**

1. Agregue otro módulo de herramientas, seleccionando la variable Set.
1. Asigne a la variable el nombre de “Horas”.
1. Establezca el valor de la variable en formatNumber(result/60;2;.;,)

   **El panel de asignación debe tener este aspecto:**

   ![Imagen 8 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-8.png)

   **A continuación, obtenga los valores configurados para el archivo de salida. Para agrupar, debe utilizarse el ID de usuario y el valor de fecha. También se deben utilizar las horas calculadas.**

1. Agregue otro módulo CSV mediante el agregador Crear CSV (avanzado).
1. El módulo de origen es el agregador de Herramientas: numérico.
1. Haga clic en Agregar por medio de estructura de datos y asigne un nombre a la estructura de datos “Suma diaria con registro de tiempo”.
1. Haga clic en Agregar elemento para crear el primer elemento.
1. Asigne un nombre al elemento “UserID” y establezca el tipo en Texto. Haga clic en Agregar.
1. Vuelva a hacer clic en Agregar elemento para crear el segundo elemento.
1. Asigne un nombre al elemento “Fecha”, establezca el tipo en Fecha y haga clic en Agregar.
1. Haga clic en Agregar elemento una vez más.
1. Asigne un nombre al elemento “Horas”, establezca el tipo en Número y haga clic en Agregar.

   **La estructura de datos debería tener este aspecto:**

   ![Imagen 9 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-9.png)

1. Haga clic en Guardar para finalizar la estructura de datos Suma diaria con registro de tiempo.

   **Ahora se proporcionan los valores para los tres campos que se acaban de crear. Debería ver esos tres campos en el panel de asignación CSV.**

1. Haga clic en el campo UserID y seleccione GET en la pestaña funciones generales. En el primer parámetro, ponga División desde la pestaña texto y funciones binarias. El primer parámetro para la función División es el campo Clave. Agregue una coma como delimitador y 1 como índice. Esto indica que desea que GET recupere el primer campo de la matriz Clave.
1. Copie esta expresión en el campo Fecha. Cambie el índice de 1 a 2 para GET del segundo valor de la matriz.
1. Para el campo Horas, añada el campo Horas de la herramienta Establecer variable.

   **El panel de asignación CSV debería tener este aspecto:**

   ![Imagen 10 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-10.png)

   **Si ejecuta el escenario ahora, debería ver este resultado:**

   ![Imagen 11 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-11.png)

   **Ahora, agregue un módulo para tomar este resultado y cargarlo como documento en un proyecto existente en Workfront.**

1. Abra el proyecto en Workfront y copie el ID del proyecto de la dirección URL.
1. Vuelva al escenario en Fusion y agregue otro módulo: el módulo Cargar documento de la aplicación de Workfront.
1. Pegue el ID del proyecto en el campo ID de Registro relacionado.
1. Elija Proyecto para el Tipo de registro relacionado.
1. Elija la opción Mapa para el archivo de Origen.
1. Para el Nombre del documento, utilice el nombre de archivo que descargó y añada “Actualizado” delante de él.
1. Para el contenido de Archivo, utilice el resultado Texto del módulo Crear CSV.

   **El panel de asignación debe tener este aspecto:**

   ![Imagen 12 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-12.png)

1. Haga clic en Aceptar y en Guardar el escenario.
1. Haga clic en Ejecutar una vez para ejecutar el escenario.

   **Compruebe el inspector de ejecución en el módulo Cargar documento para confirmar que el documento se ha cargado.**

   ![Imagen 13 de Estructuras de datos](../12-exercises/assets/data-structures-walkthrough-13.png)
