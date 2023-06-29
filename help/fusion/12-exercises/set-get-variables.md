---
title: Variables Set/Get
description: Aprenda a utilizar los módulos de variables Set/Get para utilizar los campos disponibles en una ruta en otra diferente.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11045
thumbnail: KT11045.png
exl-id: 225f0090-0428-40e2-8a4b-9c6b18b205d2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '628'
ht-degree: 100%

---

# Variables Set/Get

Aprenda a utilizar los módulos de variables Set/Get para utilizar los campos disponibles en una ruta en otra diferente.

## Información general del ejercicio

Busque datos acerca de un proyecto en Workfront y envíe un correo electrónico con la información relacionada.

![Imagen 1 de las Variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## Pasos a seguir

1. Cree un nuevo escenario y asígnele el nombre “Uso compartido de variables entre rutas de enrutamiento”.
1. Para el activador, seleccione el módulo Búsqueda en la aplicación de Workfront.

   + Establezca el Tipo de registro en Proyecto.
   + Para el conjunto de resultados, seleccione Todos los registros coincidentes.
   + Para los criterios de búsqueda, establézcalos en Estado igual a CUR.
   + Para las salidas, seleccione ID, Nombre, Descripción e ID del patrocinador.

   ![Imagen 2 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![Imagen 3 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. Haga clic en Aceptar y cambie el nombre de este módulo a “Buscar proyectos actuales”.
1. Añada otro módulo y seleccione el módulo Leer un registro de Workfront.

   + En Tipo de registro, seleccione Usuario.
   + En Resultados, seleccione Nombre.
   + Asigne el ID del patrocinador del módulo Búsqueda al campo ID.

1. Haga clic en Aceptar.
1. Cambie el nombre del módulo a “Buscar nombre del patrocinador”.

   ![Imagen 4 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. Guarde el escenario y haga clic en Ejecutar una vez.

   Si recibe un error en el módulo Leer un registro, es probable que se deba a que el módulo Búsqueda encuentra un proyecto sin un patrocinador enumerado.

   **Para evitar este error, cree dos rutas: una para los proyectos que tienen un ID de patrocinador y otra para los que no.**

1. Añada un enrutador entre los dos módulos haciendo clic en el icono de llave inglesa situado entre el enrutador y el módulo Leer un registro. Configure un filtro denominado “El patrocinador existe” y establezca la Condición en El ID del patrocinador existe.

   ![Imagen 5 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. Haga clic en el enrutador para crear otra ruta. Añada un módulo Enviar un correo electrónico desde la aplicación Correo electrónico.

   + Coloque su propia dirección de correo electrónico en el campo Para.
   + En el campo Asunto, escriba “Información del proyecto actual”.
   + En el campo Contenido, ponga el nombre, la descripción y el patrocinador del proyecto.
   + No puede extraer la salida del nombre del patrocinador desde el módulo Leer un registro. Solo puede acceder al ID del patrocinador desde el módulo de búsqueda antes del enrutador. Tendrá que encontrar una manera de acceder a él desde la otra ruta del enrutador.

   ![Imagen 6 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. Haga clic en Aceptar por ahora y cambie el nombre de este módulo a “Enviar información del proyecto”

   **Utilice las variables Set/Get para compartir datos entre diferentes rutas.**

1. Después del módulo Buscar nombre de patrocinador, añada un módulo de herramienta de variable Establecer.

   + Ponga “Nombre del patrocinador” como nombre de la variable.
   + Deje la duración de la Variable en un ciclo.
   + Asigne el campo al resultado del nombre desde el módulo Buscar nombre del patrocinador.

1. Haga clic en Aceptar y cambie el nombre del módulo a “Establecer nombre del patrocinador”.

   ![Imagen 7 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. A continuación, haga clic con el botón derecho del ratón entre el enrutador y el módulo Enviar un correo electrónico para añadir un módulo de herramienta de variable Get. Introduzca “Nombre del patrocinador” en el campo Nombre de la variable.
1. Haga clic en Aceptar. Cambie el nombre del módulo a “Obtener nombre del patrocinador”.

   ![Imagen 8 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. Vuelva al módulo Enviar un correo electrónico y asigne el valor del módulo Obtener nombre del patrocinador al campo Contenido. Haga clic en Aceptar.

   ![Imagen 8 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >Antes de probar el escenario, se recomienda restringir el número de proyectos que se procesan para evitar recibir una inundación de correos electrónicos.

1. Diríjase a la unidad de prueba de Workfront y busque el proyecto Northstar Fashion Exhibitors Booth. Este es un proyecto actual que tiene un patrocinador. Copie el ID del proyecto desde la dirección URL.

   ![Imagen 10 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. En su escenario, haga clic en el módulo Buscar proyectos actuales. Agregue otra condición a los criterios de búsqueda haciendo clic en el botón verde “Añadir regla AND”. Especifique que el ID debe ser igual a el ID de proyecto que ha copiado. Haga clic en Aceptar.
1. Guarde su escenario y haga clic en Ejecutar una vez.
1. Revise los inspectores de ejecución y el correo electrónico que reciba.

   ![Imagen 11 de las variables Set/Get](../12-exercises/assets/set-get-variables-walkthrough-11.png)
