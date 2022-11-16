---
title: Crear instrucciones OR en filtros
description: Aprenda a utilizar una instrucción OR para indicar a Workfront que quiere ver esta condición O la que figura en el informe.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
kt: 9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: 252ba3ba44f22519a35899fcda9c6bca597a6c2c
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Crear instrucciones OR en filtros

Cuando crea un filtro con varias líneas de criterios, de forma predeterminada coloca una Y entre cada línea. Esto significa que cada resultado de la lista cuando utiliza este filtro cumple todas las reglas de filtro.

En este ejemplo, tenemos tres criterios, o reglas, para un filtro de proyecto:

1. El proyecto debe tener una fecha de finalización planificada que corresponda al mes actual.
1. El proyecto debe estar en el portafolio de marketing de eventos.
1. El proyecto debe ser un proyecto activo, lo que significa que debe tener el estado Actual.

![Imagen de la creación de un filtro con instrucciones AND en [!DNL Workfront]](assets/or-statement-1.png)

Los proyectos de la lista de resultados cumplen los tres criterios, lo que le ayuda a reducir los resultados de búsqueda para que pueda ver la información exacta que necesita.

![Imagen de una lista filtrada en [!DNL Workfront]](assets/or-statement-2.png)

Sin embargo, puede haber ocasiones en las que quiera que los resultados del filtro cumplan varios criterios, y es entonces cuando las instrucciones OR pueden ayudar. Con una instrucción OR, le está diciendo al filtro que desea ver esta O esa.

## Uso de instrucciones OR

Las instrucciones OR amplían o aumentan la cantidad de información que encuentra el filtro, ya que para aparecer en la lista de resultados, un elemento debe cumplir solamente una de las reglas de filtro, no todas.

Veamos una declaración OR simple: proyectos que usted es el administrador de proyectos (propietario) para proyectos OR creados por usted.

![Una imagen de la creación de un filtro con instrucciones OR en [!DNL Workfront]](assets/or-statement-3.png)

Después de configurar ambas reglas de filtro, haga clic en Y entre ellas y cambie a O.

![Una imagen de la creación de un filtro con instrucciones OR en [!DNL Workfront]](assets/or-statement-4.png)

O entre las dos reglas de filtro amplía los criterios de búsqueda, lo que indica a Workfront que busque proyectos que cumplan una o varias de esas opciones: su nombre está en el campo propietario del proyecto o usted es la persona que creó el proyecto.

## Varias reglas de filtro con instrucciones OR

Ahora veamos una instrucción OR que contiene varias reglas de filtro a cada lado del operador OR. Esto utiliza las mismas dos reglas que antes, pero agrega una regla: los proyectos también deben tener el estado Actual.

![Una imagen de la creación de un filtro con instrucciones OR en [!DNL Workfront]](assets/or-statement-5.png)

Observe que Workfront &quot;agrupa&quot; las reglas de filtro a cada lado del operador OR (hay un cuadro gris alrededor de ellas). Esto le indica a Workfront que ejecute las reglas a cada lado de la condición OR de forma conjunta, buscando proyectos que cumplan ambos criterios porque están unidos con AND.

En este ejemplo, Workfront busca:

* Proyectos que tienen su nombre en el campo propietario del proyecto que también tienen el estado Actual.
* **MÁS (O)**
* Proyectos que ha creado que también tienen el estado Actual.

Colocar la regla &quot;estado del proyecto es igual a actual&quot; en cada lado de la condición OR garantiza que la regla funciona junto con cada una de las demás reglas. Esta regla común a veces se denomina &quot;constante&quot;.

>[!NOTE]
>
>No está limitado a una regla de filtro repetido en cada lado del operador OR. Según sus necesidades, puede tener varias. Workfront recomienda mantener como mínimo estas reglas repetidas para garantizar que el filtro proporcione los resultados que necesita.

## ¿Qué sucede sin la regla de filtro común?

Sin las reglas de filtro comunes, es posible que no obtenga los resultados de búsqueda que anticipó.

Por ejemplo, si pone la regla &quot;estado del proyecto es igual a actual&quot; solo en un lado de la condición OR, solo funciona con las otras reglas de filtro de esa sección. En la imagen siguiente, verá que la regla &quot;estado del proyecto es igual a actual&quot; solo está en la sección superior.

![Una imagen de la creación de un filtro con instrucciones OR en [!DNL Workfront]](assets/or-statement-6.png)

Esto significa que Workfront buscará:

* Proyectos que tienen su nombre en el campo propietario del proyecto y que tienen el estado Actual.
* **MÁS (O)**
* Todos los proyectos que ha creado.

Como puede ver, esta configuración de filtro le proporciona resultados ligeramente diferentes al filtro con la regla de filtro repetido. Por eso es importante asegurarse de que el filtro esté configurado correctamente para garantizar que obtiene los resultados que desea y necesita.

No es posible utilizar instrucciones OR con frecuencia al crear filtros. Pero si lo hace, puede reducir el número de filtros que necesita crear. Asegúrese de que los filtros no devuelvan demasiados resultados; una lista larga puede dificultar la búsqueda de la información exacta que necesitan los usuarios.

## Actividad de filtro OR

Desea encontrar tareas incompletas que están asignadas a usted o que no están asignadas a nadie. Configure un filtro de modo que se asemeje al que se muestra a continuación. ¿Le dará este filtro los resultados que desea? ¿Por qué o por qué no?

![Una imagen de una instrucción OR creada incorrectamente en [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Respuestas

No, este filtro no proporciona los resultados que desea (tareas que no han finalizado y que están asignadas a usted o a nadie), ya que la regla de filtro para el estado de la tarea solo está en una parte de la condición OR.

En su lugar, este filtro genera una lista que muestra:

* Tareas asignadas a usted que tengan un estado en curso o nuevo.
* **MÁS (O)**
* Todas las tareas no asignadas, independientemente del estado.

El filtro debe ser similar al que se muestra a continuación. Observe que este filtro tiene la regla de filtro para el estado de la tarea en ambos lados del operador OR.

![Una imagen de una instrucción OR creada correctamente en [!DNL Workfront]](assets/or-statement-your-turn-2.png)
