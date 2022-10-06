---
title: Introducción a los conectores universales
description: Amplíe su comprensión de trabajar con conectores universales REST y trabajar con los datos devueltos.
feature: Workfront Fusion
role: User
level: Beginner
kt: 11042
thumbnail: KT11042.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '591'
ht-degree: 0%

---


# Introducción a los conectores universales

Amplíe su comprensión de trabajar con conectores universales REST y trabajar con los datos devueltos.

## Información general del ejercicio

Usando un carácter Pokemon en una hoja de cálculo, llame a la API de Poke a través de un conector HTTP para recopilar y publicar más información sobre ese carácter.

![Introducción a los conectores universales Imagen 1](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## Pasos a seguir

**Descargue el archivo CSV desde Workfront.**

1. En la carpeta &quot;Archivos de ejercicio de fusión&quot; de Workfront, seleccione &quot;_Fusion2020_Shipping Manifest.csv&quot; y haga clic en Detalles del documento.
1. Copie el primer número de ID de la dirección URL.
1. Cree un nuevo escenario en Workfront Fusion. Asígnele el nombre &quot;Uso de conectores universales&quot;.
1. Comience con el módulo Descargar documento de la aplicación Workfront.
1. Configure la conexión de Workfront e incluya el ID de documento que ha copiado de la URL de Workfront.
1. Cambie el nombre de este módulo &quot;Descargar manifiesto de envío&quot;.

   ![Introducción a los conectores universales Imagen 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **Analice los datos del manifiesto de envío.**

1. Añada otro módulo seleccionando Analizar CSV.
1. Configure el CSV de análisis para 11 columnas. Marque la casilla CSV contiene encabezados . Elija Comma delimiterType y coloque Datos del módulo Descargar documento en el campo CSV.

   ![Introducción a los conectores universales Imagen 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. Cambie el nombre de este módulo &quot;Analizar manifiesto de envío&quot;.
1. Guarde el escenario y haga clic en Ejecutar una vez para poder ver los datos del archivo CSV en los pasos siguientes.

   **Obtenga los datos de Pokemon mediante el conector universal.**

1. Añada un módulo HTTP Make a Request .
1. En el campo URL, utilice https://pokeapi.co/api/v2/pokemon/[Carácter], donde [Carácter] está asignado a la columna 3 desde el módulo CSV de análisis.
1. Active la casilla de verificación Analizar respuesta .
1. Seleccione Mostrar configuración avanzada y, a continuación, marque la casilla junto a &quot;Evaluar todos los estados como errores&quot;.
1. Haga clic en Aceptar y cambie el nombre del módulo &quot;Obtener información de Pokemon&quot;.

   **El panel de asignación debe tener este aspecto:**

   ![Introducción a los conectores universales Imagen 3](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **En esta parte del ejercicio, solo desea procesar la fila 1 en el archivo CSV.**

1. Añada un filtro antes de su módulo Get Pokemon info . Denomínela &quot;Solo fila 1&quot;.
1. Establezca la condición para permitir que solo pase el ID número 1. El ID número 1 se encuentra en la fila 1 y el campo ID se encuentra en la columna 1 del archivo CSV.

   ![Introducción a los conectores universales Imagen 4](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. Guarde el escenario.
1. Haga clic en Ejecutar una vez y observe el mensaje de error que recibe en el módulo HTTP Realizar una solicitud .

   >[!IMPORTANT]
   >
   >En el campo URL de datos de entrada, el nombre del carácter aparece en mayúsculas. Esto no funcionará para realizar esa llamada de API porque los nombres de caracteres deben estar en minúsculas.

   ![Introducción a los conectores universales Imagen 5](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. Utilice el panel de asignación en el campo HTTP Make a request URL para realizar la [Carácter] field todas las letras minúsculas usando la variable **lower** función.

   ![Introducción a los conectores universales Imagen 6](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **Asigne información desde la API utilizando el módulo Set multiple variables .**

1. Agregue el módulo Set multiple variables después de Get Pokemon info. Nombre, altura, peso y capacidades del mapa.
1. Dado que el campo Capacidades es una matriz, recuerde utilizar la función de mapa para acceder al nombre de cada capacidad de la matriz.

   ![Introducción a los conectores universales Imagen 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **Ejecute el escenario sin el filtro para descubrir otro error.**

1. Para procesar todas las filas del archivo CSV, elimine el filtro llamado Solo fila 1:

   + Haga clic en el icono de filtro para editarlo.
   + Elimine la etiqueta del filtro.
   + Elimine la condición.
   + Haga clic en Aceptar.

1. Guarde el escenario y haga clic en Ejecutar una vez.
1. Se produce un error en el módulo Get Pokemon info . Verá que se ha pasado un carácter de superhéroe a la API de Pokemon.

   >[!NOTE]
   >
   >En el tutorial Enrutadores, verá cómo resolver este error creando una ruta separada para procesar superhéroes.

   ![Introducción a los conectores universales Imagen 8](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)