---
title: Almacenes de datos
description: Obtenga información sobre cómo sincronizar nombres de empresas entre dos sistemas. (Debe tener entre 60 y 160 caracteres, pero 59 caracteres)
feature: Workfront Fusion
role: User
level: Beginner
kt: 11055
thumbnail: KT11055.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---


# Almacenes de datos

Obtenga información sobre cómo sincronizar nombres de empresas entre dos sistemas.

## Información general del ejercicio

Esta es la primera parte de una sincronización unidireccional de empresas en Workfront y otro sistema. Por ahora, solo se sincroniza entre un almacén de datos de Fusion y Workfront. Una tabla de un almacén de datos realiza un seguimiento del Workfront ID (WFID) y el ID de la empresa en el archivo CSV (CID) de cada empresa. Esto permite una sincronización bidireccional en algún momento futuro.

![Almacenes de datos Imagen 1](../12-exercises/assets/data-stores-walkthrough-1.png)

## Pasos a seguir

**Descargue el archivo desde Workfront.**

1. En la carpeta &quot;Archivos de ejercicio de fusión&quot; de Workfront, seleccione &quot;_Companies.csv&quot; y haga clic en Detalles del documento.
1. Copie el primer número de ID de la dirección URL.
1. En Fusion, cree un nuevo escenario denominado &quot;Uso de almacenes de datos para sincronizar datos&quot;.
1. Para el módulo déclencheur, seleccione el módulo Descargar documento de Workfront.
1. Configure la conexión de Workfront e incluya el ID de documento copiado de la URL de Workfront.
1. Asigne a este módulo el nombre &quot;Obtener archivo de empresas&quot;.
1. Ahora agregue un módulo CSV de análisis.
1. Para el campo Number of columns , escriba 2.
1. Asigne datos desde el módulo Descargar documento del campo CSV.
1. Asigne a este módulo el nombre &quot;Analizar archivo de empresas&quot;.
1. Guarde el escenario y haga clic en Ejecutar una vez.

   **Cree un almacén de datos y una estructura de datos.**

1. Agregue un módulo de registros de búsqueda del almacén de datos.
1. Cree un nuevo almacén de datos con el nombre &quot;Sincronización de la empresa&quot;.
1. Dentro del almacén de datos, cree una estructura de datos denominada &quot;Sincronización de la empresa (estructura)&quot;.
1. Cree cuatro campos.

   + CID: el ID de empresa del archivo CSV
   + Nombre de la empresa
   + WFID: El ID de empresa de Workfront
   + Fecha de creación: asegúrese de que el tipo de datos es fecha

   ![Almacenes de datos Imagen 2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. Haga clic en Guardar en la estructura de datos y, a continuación, establezca el tamaño de almacenamiento de datos en 1 y guarde el almacén de datos.
1. Continuando en el módulo Almacén de datos, configure un Filtro donde el CID sea igual al ID de la empresa desde el módulo CSV de análisis (columna 1).
1. Haga clic en Mostrar configuración avanzada y seleccione la opción para &quot;continuar con la ejecución del escenario o la ruta, incluso si este módulo se devuelve sin resultados&quot;.

   ![Almacenes de datos Imagen 3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. Cambie el nombre de este módulo &quot;Compañías coincidentes&quot;.
1. Agregue un módulo de registros de búsqueda de Workfront.
1. Elija Empresa como tipo de registro.
1. Los criterios de búsqueda son el nombre de empresa dentro de Workfront que es igual al nombre de empresa en el archivo CSV.
1. Para los resultados, seleccione el nombre de la empresa y el ID.

   ![Almacenes de datos Imagen 4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. Haga clic en Aceptar y cambie el nombre de este módulo por &quot;Empresas coincidentes&quot;.

   **Cree diferentes rutas en función de si la empresa existe en Workfront o en el almacén de datos.**

   **Ruta de enrutamiento 1: Cree una empresa.**

1. Agregue un módulo de enrutador a la derecha del módulo de registros de búsqueda de Workfront.
1. Agregue un módulo Crear registro de Workfront a la ruta superior.
1. Establezca el tipo de registro en Empresa.
1. Seleccione Nombre en Campos para Asignar. Asigne el campo de nombre al resultado del módulo CSV de análisis (columna 2).
1. Cambie el nombre de este módulo &quot;Crear empresa&quot;.

   ![Almacenes de datos Imagen 5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. Añada un filtro después del enrutador para crear solo una empresa si no está ya en Workfront. Denomínela &quot;No en Workfront&quot;.
1. Establezca la condición en el ID desde el módulo de búsqueda de Workfront y no exista.

   ![Almacenes de datos Imagen 6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **Prepárese para actualizar el almacén de datos en la siguiente ruta.**

1. Agregue un módulo Set variable al final de la ruta superior.
1. Establezca el nombre de la variable en &quot;Workfront ID&quot;.
1. Establezca el valor Variable en el ID desde el módulo Crear empresa .
1. Cambie el nombre de este módulo &quot;Set Workfront ID&quot;.

   **Ruta de enrutamiento 2: Actualice el almacén de datos.**

1. Cree un filtro en la ruta de enrutamiento 2. Asígnele el nombre &quot;No en el almacén de datos&quot;.

1. Establezca la condición en Clave desde el módulo Almacén de datos y no existe.

   ![Almacenes de datos Imagen 7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. El primer módulo de esta ruta es el módulo Get variable .
1. Establezca el nombre de la variable en &quot;Workfront ID&quot;.
1. Cambie el nombre de este módulo &quot;Obtener Workfront ID&quot;.
1. Agregue otro módulo desde la aplicación Almacén de datos y añada/sustituya un registro.
1. En el campo Almacén de datos , seleccione Sincronización de empresa. Este es el almacén de datos que creó anteriormente.
1. Deje el campo Key en blanco.
1. Asigne el campo CID de la Columna 1 del módulo CSV de análisis.
1. Asigne el campo de nombre de empresa de la columna 2 en el módulo CSV de análisis.
1. Asigne el campo WFID desde el módulo Get Workfront ID .
1. Para el campo Fecha de creación , utilice la función formatDate de la ficha Fecha y hora para dar formato a la fecha actual como MM/DD/AAAA.

   ![Almacenes de datos Imagen 8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. Haga clic en Aceptar y cambie el nombre de este módulo por &quot;Crear entrada de empresa&quot;.

   **Ruta de enrutamiento 3: sincronice el almacén de datos entre sistemas.**

1. Comience creando un filtro en la ruta de enrutamiento 3. Denomínela &quot;La empresa existe, no en el almacén de datos&quot;.
1. Establezca la Condición en Clave desde el módulo Registros de búsqueda del almacén de datos y no existe.
1. Haga clic en el botón Agregar regla AND y designe que el nombre de la empresa del archivo CSV (Columna 2) es igual al nombre de la empresa que se encuentra en el módulo Workfront Search.

   ![Almacenes de datos Imagen 9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. Ahora agregue otro módulo Add/replace a record clonando el que se encuentra al final de la ruta de enrutamiento 2.
1. Arrastre el módulo clonado a su lugar al final de la ruta de enrutamiento 3. Elimine el módulo vacío que estaba allí.
1. Haga clic en el módulo clonado. Todos los campos deben permanecer iguales excepto el campo WFID. Asignarlo desde el módulo Búsqueda de empresas coincidentes .

   ![Almacenes de datos Imagen 10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. Haga clic en Aceptar y cambie el nombre de este módulo por &quot;Crear entrada de empresa&quot;.
