---
title: Creación de instrucciones OR en filtros
description: Aprenda a utilizar una instrucción OR para indicar a Workfront que desea ver esta condición OR en el informe.
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
ht-degree: 0%

---

# Creación de instrucciones OR en filtros

Cuando se genera un filtro con varias líneas de criterios, Workfront coloca de forma predeterminada una Y entre cada línea. Esto significa que cada resultado de la lista cuando se utiliza este filtro cumple todas las reglas de filtrado.

En este ejemplo, tenemos tres criterios o reglas para un filtro de proyecto:

1. El proyecto debe tener una fecha planificada de finalización que coincida con el mes actual.
1. El proyecto debe estar en el portafolio de marketing de eventos.
1. El proyecto debe ser un proyecto activo, lo que significa que debe tener el estado Actual.

![Imagen de creación de un filtro con instrucciones AND en [!DNL Workfront]](assets/or-statement-1.png)

Los proyectos de la lista de resultados cumplen los tres criterios, lo que le ayuda a reducir los resultados de búsqueda para que pueda ver la información exacta que necesita.

![Imagen de una lista filtrada en [!DNL Workfront]](assets/or-statement-2.png)

Sin embargo, puede haber ocasiones en las que desea que los resultados del filtro cumplan varios criterios, y es entonces cuando las instrucciones OR pueden ayudar. Con una instrucción OR, está diciendo al filtro que desea ver cosas que coincidan con CUALQUIERA de sus instrucciones OR en oposición a TODAS sus instrucciones AND.

## Uso de instrucciones OR

Las instrucciones OR expanden o aumentan la cantidad de información que encuentra el filtro porque, para aparecer en la lista de resultados, un elemento debe cumplir sólo una de las reglas de filtrado, no todas.

Veamos una instrucción OR simple: proyectos que usted es el administrador de proyectos (propietario) para proyectos OR creados por usted.

![Imagen de creación de un filtro con instrucciones OR en [!DNL Workfront]](assets/or-statement-3.png)

Después de configurar ambas reglas de filtro, haga clic en Y entre ellas y cambie a O.

![Imagen de creación de un filtro con instrucciones OR en [!DNL Workfront]](assets/or-statement-4.png)

La condición OR entre las dos reglas de filtro amplía los criterios de búsqueda, lo que indica a Workfront que busque proyectos que cumplan una de esas opciones (su nombre está en el campo del propietario del proyecto o usted es la persona que creó el proyecto).

## Varias reglas de filtro con instrucciones OR

Veamos ahora una instrucción OR que contiene varias reglas de filtro a cada lado de OR. Utiliza las mismas dos reglas que antes, pero añade una regla: los proyectos también deben tener el estado Actual.

![Imagen de creación de un filtro con instrucciones OR en [!DNL Workfront]](assets/or-statement-5.png)

Observe que Workfront &quot;agrupa&quot; las reglas de filtrado a cada lado del operador OR (hay un cuadro gris alrededor de ellas). Esto indica a Workfront que ejecute las reglas en cada lado del operador OR junto, buscando proyectos que cumplan ambos criterios porque están unidos con AND.

En este ejemplo, Workfront busca:

* Proyectos que tienen su nombre en el campo propietario del proyecto y que también tienen el estado Actual.
* **MÁS (O)**
* Proyectos que ha creado y que también tienen el estado Actual.

Colocar la regla &quot;el estado del proyecto es igual a actual&quot; a cada lado de OR garantiza que la regla funcione junto con cada una de las demás reglas. Esta regla común a veces se denomina &quot;constante&quot;.

>[!NOTE]
>
>No está limitado a una regla de filtro repetida a cada lado del quirófano. Según sus necesidades, puede tener varias. Workfront recomienda reducir al mínimo estas reglas repetidas para garantizar que el filtro proporcione los resultados que necesita.

## ¿Qué sucede sin la regla de filtro común?

Sin las reglas de filtro comunes, es posible que no obtenga los resultados de búsqueda anticipados.

Por ejemplo, si coloca la regla &quot;el estado del proyecto es igual a Actual&quot; solo en un lado del OR, solo funciona con las demás reglas de filtro de esa sección. En la imagen siguiente, verá que la regla &quot;el estado del proyecto es igual a actual&quot; solo se encuentra en la sección superior.

![Imagen de creación de un filtro con instrucciones OR en [!DNL Workfront]](assets/or-statement-6.png)

Esto significa que Workfront buscará lo siguiente:

* Proyectos que tienen su nombre en el campo de propietario del proyecto y tienen el estado Actual.
* **MÁS (O)**
* Todos los proyectos que ha creado.

Como puede ver, esta configuración de filtro le proporciona resultados ligeramente diferentes a los del filtro con la regla de filtro repetida. Es por eso que asegurarse de que el filtro esté configurado correctamente es importante para asegurarse de que obtiene los resultados que desea y necesita.

No puede utilizar instrucciones OR con frecuencia al crear filtros. Sin embargo, esto puede ayudarle a reducir el número de filtros que debe crear. Solo asegúrese de que los filtros no devuelvan demasiados resultados; una lista larga puede dificultar a los usuarios la búsqueda de la información exacta necesaria.

## Actividad de filtro O

Desea encontrar tareas incompletas que se le han asignado o que no se han asignado a nadie. Ha configurado un filtro para que se parezca al de abajo. ¿Este filtro le proporcionará los resultados que desea? ¿Por qué?

![Imagen de una instrucción OR creada incorrectamente en [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### Respuestas

No, este filtro no proporcionará los resultados esperados (tareas que no han finalizado y que no se le han asignado a usted o que no se le han asignado a nadie) porque la regla de filtrado para el estado de la tarea solo está a un lado del operador OR.

En su lugar, este filtro generará una lista que muestra:

* Tareas asignadas que tienen un estado de En curso o Nueva.
* **MÁS (O)**
* Todas las tareas sin asignar, independientemente del estado.

El filtro debe ser similar al de abajo. Observe que este filtro tiene la regla de filtro para el estado de la tarea a ambos lados de OR.

![Imagen de una instrucción OR creada correctamente en [!DNL Workfront]](assets/or-statement-your-turn-2.png)
