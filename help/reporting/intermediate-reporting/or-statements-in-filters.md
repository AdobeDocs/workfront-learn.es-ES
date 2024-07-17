---
title: Crear instrucciones OR en filtros
description: Aprenda a utilizar una instrucción O para indicar a Workfront que quiere ver esta condición O la que figura en el informe.
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 100%

---

# Crear instrucciones OR en filtros

Cuando genera un filtro con varias líneas de criterios, Workfront coloca de forma predeterminada una AND entre cada una. Esto significa que cada resultado de la lista, cuando utiliza este filtro, cumple todas las reglas.

En este ejemplo, tenemos tres criterios, o reglas, para un filtro de proyecto:

1. El proyecto debe tener una fecha planificada de finalización que corresponda al mes actual.
1. El proyecto debe estar en el portafolio de marketing de eventos.
1. El proyecto debe ser un proyecto activo, lo que significa que debe tener el estado Actual.

![Una imagen de la creación de un filtro con instrucciones Y en [!DNL Workfront]](assets/or-statement-1.png)

Los proyectos de la lista de resultados cumplen los tres criterios, lo que le ayuda a reducir los resultados de búsqueda para que pueda ver la información exacta que necesita.

![Una imagen de una lista filtrada en [!DNL Workfront]](assets/or-statement-2.png)

Sin embargo, puede haber ocasiones en las que quiera que los resultados del filtro cumplan varios criterios, y es entonces cuando las instrucciones OR pueden ayudar. Con una instrucción OR, está diciendo al filtro que desea ver cosas que coincidan con CUALQUIERA de sus instrucciones OR en oposición a TODAS sus instrucciones AND.

## Uso de instrucciones O

Las instrucciones O amplían o aumentan la cantidad de información que encuentra el filtro, ya que, para aparecer en la lista de resultados, un elemento debe cumplir solamente una de las reglas de filtro, no todas.

Veamos una instrucción OR: proyectos en los que es el administrador del proyecto (propietario) para proyectos OR creados por usted.

![Una imagen de la creación de un filtro con instrucciones O en [!DNL Workfront]](assets/or-statement-3.png)

Después de configurar ambas reglas de filtro, haga clic en Y entre ellas y cámbielo a O.

![Una imagen de la creación de un filtro con instrucciones O en [!DNL Workfront]](assets/or-statement-4.png)

El O entre las dos reglas de filtro amplía los criterios de búsqueda, lo que indica a Workfront que busque proyectos que cumplan una o varias de esas opciones: su nombre está en el campo propietario del proyecto o usted creó el proyecto.

## Varias reglas de filtro con instrucciones O

Ahora veamos una instrucción OR que contiene varias reglas de filtro a cada lado del OR. Utiliza las mismas dos reglas que antes, pero agrega otra: los proyectos también deben tener el estado Actual.

![Una imagen de la creación de un filtro con instrucciones O en [!DNL Workfront]](assets/or-statement-5.png)

Observe que Workfront “agrupa” las reglas de filtro a cada lado del operador OR (hay una casilla gris alrededor de ellas). Esto le indica a Workfront que ejecute las reglas a cada lado de OR de forma conjunta, buscando proyectos que cumplan ambos criterios porque están unidos con AND.

En este ejemplo, Workfront busca lo siguiente:

* Proyectos que tienen su nombre en el campo Propietario del proyecto y también el estado Actual.
* **MÁS (O)**
* Proyectos que ha creado que también tienen el estado Actual.

Colocar la regla “estado del proyecto es igual a Actual” en cada lado de OR garantiza que la regla funcione conjuntamente con cada una de las otras reglas. Esta regla común a veces se denomina “constante”.

>[!NOTE]
>
>No está limitado a una regla de filtro repetida en cada lado de O. Según sus necesidades, puede tener varias. Workfront recomienda mantener como mínimo estas reglas repetidas para garantizar que el filtro proporcione los resultados que necesita.

## ¿Qué sucede sin la regla de filtro común?

Sin las reglas de filtro comunes, es posible que no obtenga los resultados de búsqueda previstos.

Por ejemplo, si pone la regla “estado del proyecto es igual a Actual” solo en un lado de la condición OR, únicamente funciona con las otras reglas de filtro de esa sección. En la siguiente imagen verá que la regla “estado del proyecto es igual a Actual” solo está en la sección superior.

![Una imagen de la creación de un filtro con instrucciones O en [!DNL Workfront]](assets/or-statement-6.png)

Esto significa que Workfront buscará lo siguiente:

* Proyectos que tienen su nombre en el campo Propietario del proyecto y que tienen el estado Actual.
* **MÁS (O)**
* Todos los proyectos que ha creado.

Como puede ver, esta configuración le proporciona resultados ligeramente diferentes al filtro con la regla de filtro repetido. Por eso es importante asegurarse de que el filtro esté configurado correctamente, para garantizar que obtiene los resultados que desea y necesita.

No es posible utilizar instrucciones O con frecuencia al crear filtros. Pero, si lo hace, puede reducir el número de filtros que necesita crear. Asegúrese de que los filtros no devuelvan demasiados resultados; una lista larga puede dificultar la búsqueda de la información exacta que necesitan los usuarios.

## Actividad de filtro O

Desea encontrar tareas incompletas que están asignadas a usted o que no están asignadas a nadie. Configure un filtro de modo que se asemeje al que se muestra a continuación. ¿Le dará este filtro los resultados que desea? ¿Por qué sí o por qué no?

![Una imagen de una instrucción O creada incorrectamente en [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Respuestas

No, este filtro no proporciona los resultados que desea (tareas que no han finalizado y que, o bien están asignadas a usted o a nadie), ya que la regla de filtro para el estado de la tarea solo está en una parte de la instrucción OR.

En su lugar, este filtro genera una lista que muestra:

* Las tareas asignadas a usted que tengan un estado En curso o Nueva.
* **MÁS (O)**
* Todas las tareas no asignadas, independientemente del estado.

El filtro debe ser similar al que se muestra a continuación. Observe que este filtro tiene la regla de filtro para el estado de la tarea en ambos lados del operador O.

![Una imagen de una instrucción O creada correctamente en [!DNL Workfront]](assets/or-statement-your-turn-2.png)
