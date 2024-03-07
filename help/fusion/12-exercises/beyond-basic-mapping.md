---
title: Ejercicio sobre Más allá de la asignación básica
description: Información sobre cómo utilizar las fórmulas del panel de asignación para manipular o convertir los campos enviados a un módulo.
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
recommendations: noDisplay,noCatalog
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: a4e61514567ac8c2b4ad5c9ecacb87bd83947731
workflow-type: ht
source-wordcount: '314'
ht-degree: 100%

---

# Ejercicio sobre Más allá de la asignación básica

Información sobre cómo utilizar las fórmulas del panel de asignación para manipular o convertir los campos enviados a un módulo.

## Información general del ejercicio

Cambie el nombre del proyecto, la fecha de inicio planificada y la prioridad en los ejercicios de tutorial de asignación más allá de la asignación básica mediante las fórmulas del panel de asignación.

![Más allá de la asignación básica imagen 1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## Pasos a seguir

**Haga un clon del escenario de diseño de escenario inicial.**

1. Seleccione la opción Clonar a la derecha del diseño de escenario inicial en la sección de escenario, como se muestra a continuación. Denomínela “Más allá de la asignación básica”.

   ![Más allá de la asignación básica imagen 2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **Ahora vamos a usar el panel de asignación en el módulo Crear proyectos de Workfront para configurar los campos nombre del proyecto, fecha de inicio planificada y prioridad.**

1. Haga clic en el módulo Crear proyectos de Workfront para editar la configuración. Con el panel de asignación, cambie el campo Nombre a “[Mi nombre de proyecto] por [Patrocinador]”.

   + La variable [Mi nombre de proyecto] es la columna 1 del módulo CSV Parse, [Patrocinador] es la columna 6. La palabra “por” se escribe entre las dos.

1. A continuación, vaya a la Fecha de inicio planeada y utilice la fórmula addDays para añadir 15 días al campo, tal como se describe en el vídeo del tutorial Más allá de la asignación básica.
1. Busque el campo Prioridad y active el botón Asignar en la parte superior derecha del campo. El menú de la lista de selección cambia a un número. Cree una instrucción if para etiquetar un proyecto como de prioridad alta (4) si la clasificación de confianza de archivos CSV es inferior a 100; de lo contrario, puede ser Normal(2).

   + La clasificación de confianza se encuentra en la columna 4.

   **En este punto, el panel de asignación debería tener este aspecto:**

   ![Más allá de la asignación básica imagen 3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. Haga clic en Aceptar y, a continuación, en Ejecutar una vez.
1. Busque el proyecto en la instancia de Workfront para asegurarse de que todo estaba asignado correctamente.
1. Guarde el escenario.
