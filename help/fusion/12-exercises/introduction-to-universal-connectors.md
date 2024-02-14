---
title: Introducción al ejercicio de conectores universales
description: Amplíe sus conocimientos sobre el trabajo con conectores universales REST y el trabajo con los datos devueltos.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11042
thumbnail: KT11042.png
recommendations: noDisplay,noCatalog
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 98%

---

# Introducción al ejercicio de conectores universales

Amplíe sus conocimientos sobre el trabajo con conectores universales REST y el trabajo con los datos devueltos.

## Información general del ejercicio

Con un carácter Pokemon en una hoja de cálculo, llame a la API de Poke a través de un conector HTTP para recopilar y publicar más información sobre ese carácter.

![Imagen 1 de Introducción a los conectores universales](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## Pasos a seguir

**Descargue el archivo CSV desde Workfront.**

1. En la carpeta “Archivos de ejercicio de Fusion” de Workfront, seleccione “_Fusion2020_Shipping Manifest.csv” y haga clic en Detalles del documento.
1. Copie el primer número de ID de la dirección URL.
1. Cree un nuevo escenario en Workfront Fusion. Asígnele el nombre “Uso de conectores universales”.
1. Comience con el módulo Descargar documento de la aplicación Workfront.
1. Configure la conexión de Workfront e incluya el ID de documento que ha copiado de la URL de Workfront.
1. Cambie el nombre de este módulo “Descargar manifiesto de envío”.

   ![Imagen 9 de Introducción a los conectores universales](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **Analice los datos del manifiesto de envío.**

1. Añada otro módulo seleccionando Analizar CSV.
1. Configure el CSV de análisis para 11 columnas. Compruebe si la casilla CSV contiene encabezados. Elija Comma delimiterType y coloque Datos del módulo Descargar documento en el campo CSV.

   ![Imagen 2 de Introducción a los conectores universales](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. Cambie el nombre de este módulo “Analizar manifiesto de envío”.
1. Guarde el escenario y haga clic en Ejecutar una vez para poder ver los datos del archivo CSV en los pasos siguientes.

   **Obtenga los datos de Pokemon mediante el conector universal.**

1. Añada un módulo HTTP Realizar una solicitud.
1. En el campo URL, utilice `https://pokeapi.co/api/v2/pokemon/[Character]`, donde [Carácter] está asignado a la columna 3 desde el módulo CSV de análisis.
1. Active la casilla de verificación Analizar respuesta.
1. Seleccione Mostrar configuración avanzada y, a continuación, marque la casilla junto a “Evaluar todos los estados como errores”.
1. Haga clic en Aceptar y cambie el nombre del módulo “Obtener información de Pokemon”.

   **El panel de asignación debe tener este aspecto:**

   ![Imagen 3 de Introducción a los conectores universales](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **En esta parte del ejercicio, solo desea procesar la fila 1 en el archivo CSV.**

1. Añada un filtro antes de su módulo Obtener información de Pokemon. Denomínelo “Solo fila 1”.
1. Establezca la condición para permitir que solo pase el ID número 1. El ID número 1 se encuentra en la fila 1 y el campo ID se encuentra en la columna 1 del archivo CSV.

   ![Imagen 4 de Introducción a los conectores universales](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. Guarde el escenario.
1. Haga clic en Ejecutar una vez y observe el mensaje de error que recibe en el módulo HTTP Realizar una solicitud.

   >[!IMPORTANT]
   >
   >En el campo URL de datos de entrada, el nombre del carácter aparece en mayúsculas. Esto no funcionará para realizar esa llamada de API porque los nombres de caracteres deben estar en minúsculas.

   ![Imagen 5 de Introducción a los conectores universales](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. Utilice el panel de asignación en el campo HTTP Crear un URL de solicitud que el campo [Carácter] esté todo en letras minúsculas usando la variable **minúsculas**.

   ![Imagen 6 de Introducción a los conectores universales](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **Asigne información desde la API utilizando el módulo Establecer múltiples variables.**

1. Añada el módulo Establecer múltiples variables después de Obtener información de Pokemon. Nombre, altura, peso y capacidades del mapa.
1. Dado que el campo Capacidades es una matriz, recuerde que debe utilizar la función de mapa para acceder al nombre de cada capacidad de la matriz.

   ![Imagen 7 de Introducción a los conectores universales](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **Ejecute el escenario sin el filtro si desea descubrir otro error.**

1. Para procesar todas las filas del archivo CSV, elimine el filtro llamado Solo fila 1:

   + Haga clic en el icono de filtro para editarlo.
   + Elimine la etiqueta del filtro.
   + Elimine la condición.
   + Haga clic en Aceptar.

1. Guarde el escenario y haga clic en Ejecutar una vez.
1. Se produce un error en el módulo Obtener información de Pokemon. Verá que se ha transferido un carácter de superhéroe a la API de Pokemon.

   >[!NOTE]
   >
   >En el tutorial Enrutadores, verá cómo resolver este error creando una ruta separada para procesar superhéroes.

   ![Imagen 8 de Introducción a los conectores universales](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)
