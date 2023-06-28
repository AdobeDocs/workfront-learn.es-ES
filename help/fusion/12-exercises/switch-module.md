---
title: Cambiar módulo
description: Aprenda a utilizar el módulo Switch cuando necesite realizar transformaciones de datos más complejas o dinámicas.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Cambiar módulo

Aprenda a utilizar el módulo Switch cuando necesite realizar transformaciones de datos más complejas o dinámicas.

## Resumen del ejercicio

Busque proyectos de correo postal en la unidad de prueba y, a continuación, cambie el nombre de cada proyecto en función de un valor seleccionado en un campo personalizado adjunto al proyecto.

![Imagen 1 del módulo del conmutador](../12-exercises/assets/switch-module-walkthrough-1.png)

## Pasos a seguir

1. Cree un nuevo escenario y asígnele el nombre &quot;Uso del módulo Switch&quot;.
1. Para el módulo déclencheur, utilice el módulo Búsqueda de Workfront.
1. Configure la conexión de Workfront y establezca el tipo de registro en Proyecto.
1. En los Criterios de búsqueda, especifique que solo desea ver los proyectos que tienen un valor en el campo personalizado Canal.
1. Para las salidas, seleccione ID, Nombre, Número de referencia y el campo personalizado Canal.

   ![Imagen 2 del módulo del conmutador](../12-exercises/assets/switch-module-walkthrough-2.png)

1. Añada el módulo Switch desde Herramientas.
1. Para el campo Entrada, asigne el campo personalizado Canal desde el módulo Buscar.

   ![Imagen 3 del módulo del conmutador](../12-exercises/assets/switch-module-walkthrough-3.png)

1. A continuación, añada casos para cada valor posible proveniente del campo personalizado Canal. El valor posible va al campo Patrón. Desea que el campo de salida incluya un código de 3 letras específico seguido del número de referencia del proyecto y, a continuación, el nombre del proyecto.

   **El panel de asignación debería tener un aspecto similar al siguiente:**

   ![Imagen 4 del módulo del conmutador](../12-exercises/assets/switch-module-walkthrough-4.png)

1. Puede añadir tantos casos adicionales como desee. Observe el campo Else en la parte inferior. Se utilizará si el valor de entrada no coincide con ninguno de los casos.

   **Actualice el nombre del proyecto en Workfront.**

   ![Imagen 5 del módulo del conmutador](../12-exercises/assets/switch-module-walkthrough-5.png)

1. Agregue un módulo Workfront Update Record.
1. En el campo ID, asígnelo al ID desde el módulo de déclencheur.
1. Establezca el Tipo de registro en Proyecto.
1. Seleccione el campo Nombre de la sección Seleccionar campos para asignar y asígnelo a la salida desde el módulo Interruptor.
1. Guarde el escenario y Ejecutar una vez. Vea los nombres de proyecto actualizados en su unidad de prueba.
