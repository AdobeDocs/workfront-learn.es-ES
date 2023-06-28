---
title: Almacenes de datos
description: Obtenga información sobre cómo sincronizar nombres de compañías entre dos sistemas. (Debe tener entre 60 y 160 caracteres, pero tiene 59)
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11055
thumbnail: KT11055.png
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Almacenes de datos

Obtenga información sobre cómo sincronizar nombres de compañías entre dos sistemas.

## Resumen del ejercicio

Esta es la primera parte de una sincronización unidireccional de compañías en Workfront y otro sistema. Por ahora, solo se sincroniza entre un almacén de datos de Fusion y Workfront. Una tabla de un almacén de datos realiza un seguimiento del Workfront ID (WFID) y del ID de empresa en el archivo CSV (CID) de cada empresa. Esto permite una sincronización bidireccional en algún momento futuro.

![Imagen 1 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-1.png)

## Pasos a seguir

**Descargue el archivo desde Workfront.**

1. En la carpeta &quot;Fusion Exercise Files&quot; de Workfront, seleccione &quot;_Companies.csv&quot; y haga clic en Detalles del documento.
1. Copie el primer número de ID de la dirección URL.
1. En Fusion, cree un nuevo escenario llamado &quot;Uso de almacenes de datos para sincronizar datos&quot;.
1. Para el módulo déclencheur, seleccione el módulo Descargar documento de Workfront.
1. Configure la conexión de Workfront e incluya el ID de documento copiado de la dirección URL de Workfront.
1. Asigne un nombre a este módulo &quot;Obtener archivo de empresas&quot;.
1. Ahora añada un módulo Analizar CSV.
1. Para el campo Número de columnas, escriba 2.
1. Asigne datos desde el módulo Descargar documento en el campo CSV.
1. Asigne un nombre a este módulo &quot;Analizar archivo de compañías&quot;.
1. Guarde el escenario y haga clic en Ejecutar una vez.

   **Crear un almacén de datos y una estructura de datos.**

1. Agregue un módulo de registros de búsqueda del almacén de datos.
1. Cree un nuevo almacén de datos con el nombre &quot;Sincronización de la compañía&quot;.
1. Dentro del almacén de datos, cree una estructura de datos denominada &quot;Sincronización de la compañía (struc)&quot;.
1. Cree cuatro campos.

   + CID: el ID de empresa del archivo CSV
   + Nombre de empresa
   + WFID: ID de empresa de Workfront
   + Fecha de creación: asegúrese de que el tipo de datos es fecha

   ![Imagen 2 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-2.png)

1. Haga clic en Guardar en la estructura de datos y, a continuación, establezca el tamaño del almacenamiento de datos en 1 y guarde el almacén de datos.
1. Si continúa en el módulo Almacén de datos, configure un Filtro en el que el CID sea igual al ID de la empresa desde el módulo Analizar CSV (columna 1).
1. Haga clic en Mostrar configuración avanzada y seleccione la opción para &quot;continuar con la ejecución del escenario o la ruta, incluso si este módulo se devuelve sin resultados&quot;.

   ![Imagen 3 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-3.png)

1. Cambie el nombre de este módulo a &quot;Empresas coincidentes&quot;.
1. Agregue un módulo de registros de búsqueda de Workfront.
1. Elija Compañía como tipo de registro.
1. Criterios de búsqueda: el nombre de la empresa en Workfront es igual al nombre de la empresa en el archivo CSV.
1. Para las salidas, seleccione el nombre de la empresa y el ID.

   ![Imagen 4 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-4.png)

1. Haga clic en Aceptar y cambie el nombre de este módulo a &quot;Empresas coincidentes&quot;.

   **Cree diferentes rutas en función de si la empresa existe en Workfront o en el almacén de datos.**

   **Ruta de enrutamiento 1: crear una empresa.**

1. Agregue un módulo de enrutador a la derecha del módulo Registros de búsqueda de Workfront.
1. Agregue un módulo Crear registro de Workfront a la ruta superior.
1. Establezca el tipo de registro en Empresa.
1. Seleccione Nombre de Campos para asignar. Asigne el campo de nombre a la salida del módulo Analizar CSV (columna 2).
1. Cambie el nombre de este módulo a &quot;Crear empresa&quot;.

   ![Imagen 5 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-5.png)

1. Añada un filtro después del enrutador para crear una empresa únicamente si aún no está en Workfront. Asígnele el nombre &quot;No está en Workfront&quot;.
1. Establezca la condición en el ID desde el módulo Búsqueda de Workfront y no existe.

   ![Imagen 6 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-6.png)

   **Prepare la actualización del almacén de datos en la siguiente ruta.**

1. Agregue un módulo Establecer variable al final de la ruta superior.
1. Establezca el Nombre de la variable en &quot;Workfront ID&quot;.
1. Establezca el valor Variable en el ID desde el módulo Crear empresa.
1. Cambie el nombre de este módulo a &quot;Set Workfront ID&quot;.

   **Ruta de enrutamiento 2: actualice el almacén de datos.**

1. Cree un filtro en la ruta de enrutamiento 2. Asígnele el nombre &quot;No está en el almacén de datos&quot;.

1. Establezca la condición en la clave desde el módulo Almacén de datos y no existe.

   ![Imagen 7 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-7.png)

1. El primer módulo de esta ruta es el módulo Obtener variable.
1. Establezca el Nombre de la variable en &quot;Workfront ID&quot;.
1. Cambie el nombre de este módulo a &quot;Obtener Workfront ID&quot;.
1. Añada otro módulo desde la aplicación del almacén de datos y añada o reemplace un registro.
1. En el campo Almacén de datos, elija Sincronización de la compañía. Este es el almacén de datos que creó anteriormente.
1. Deje el campo Clave en blanco.
1. Asigne el campo CID desde la columna 1 del módulo Analizar CSV.
1. Asigne el campo Nombre de la empresa de la columna 2 del módulo Analizar CSV.
1. Asigne el campo WFID desde el módulo Obtener Workfront ID.
1. Para el campo Fecha de creación, utilice la función formatDate de la pestaña Date and time para dar formato a la fecha actual como MM/DD/AAAA.

   ![Imagen 8 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-8.png)

1. Haga clic en Aceptar y cambie el nombre de este módulo a &quot;Crear entrada de empresa&quot;.

   **Ruta de enrutamiento 3: sincronice el almacén de datos entre sistemas.**

1. Comience creando un filtro en la ruta de enrutamiento 3. Asígnele el nombre &quot;La compañía existe, no en el almacén de datos&quot;.
1. Establezca la condición en la clave desde el módulo Registros de búsqueda del almacén de datos y no existe.
1. Haga clic en el botón Añadir regla AND y designe que el nombre de la empresa del archivo CSV (columna 2) es igual al nombre de la empresa que se encuentra en el módulo de búsqueda de Workfront.

   ![Imagen 9 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-9.png)

1. Ahora agregue otro módulo de registro Agregar o reemplazar clonando el que se encuentra al final de la ruta de enrutamiento 2.
1. Arrastre el módulo clonado a su lugar al final de la ruta de enrutamiento 3. Elimine el módulo vacío que había allí.
1. Haga clic en el módulo clonado. Todos los campos deben ser iguales, excepto el campo WFID. Asígnelo desde el módulo de búsqueda Compañías coincidentes.

   ![Imagen 10 de almacenes de datos](../12-exercises/assets/data-stores-walkthrough-10.png)

1. Haga clic en Aceptar y cambie el nombre de este módulo a &quot;Crear entrada de empresa&quot;.
