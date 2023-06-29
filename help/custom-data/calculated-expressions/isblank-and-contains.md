---
title: Uso de las expresiones ISBLANK y CONTAINS
description: Aprenda a utilizar y crear las expresiones ISBLANK y CONTAINS en un campo calculado en Adobe  [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 37a222dd921c0c3ffe72a8e091f6dbf1f18cee68
workflow-type: ht
source-wordcount: '404'
ht-degree: 100%

---

# Uso de las expresiones ISBLANK y CONTAINS

Las expresiones CONTAINS e ISBLANK se utilizan para proporcionar valores verdaderos o falsos simples. La diferencia es que la expresión ISBLANK comprueba si el campo contiene un valor mientras la expresión de texto CONTAINS busca una cadena específica dentro de un campo.

Por ejemplo, para ver si un proyecto tiene una descripción, use la expresión ISBLANK. Si el campo de descripción está en blanco, la expresión devuelve un valor de verdadero. Si el campo de descripción no está en blanco, devuelve el valor de falso.

![Equilibrador de carga de trabajo con informe de utilización](assets/isblank01.png)

Para buscar un valor específico en la descripción, como “evento de caridad”, utilice la expresión de texto CONTAIN. Si encuentra “evento de caridad” en la descripción, el campo calculado dice “verdadero”. Muestra “falso” si no encuentra “evento de caridad”.

![Equilibrador de carga de trabajo con informe de utilización](assets/isblank02.png)

## ISBLANK

La expresión de texto ISBLANK incluye el nombre de la expresión y un punto de datos.

**ISBLANK({data point})**

![Equilibrador de carga de trabajo con informe de utilización](assets/isblank03.png)

En el ejemplo anterior (donde desea saber si el proyecto tiene una descripción), la expresión sería la siguiente:

ISBLANK({description})

## CONTAINS

La expresión de texto CONTAINS incluye el nombre de la expresión, la palabra o frase que está buscando y el campo en el que buscarlo.

**CONTAINS(“frase”,{fields})**

Asegúrese de colocar comillas alrededor de la palabra o frase que está buscando; de lo contrario, la expresión no será válida.

En el ejemplo anterior (al buscar “evento de caridad” en la descripción del proyecto), la expresión sería la siguiente:

**CONTAINS(“evento de caridad”,{description})**

![Equilibrador de carga de trabajo con informe de utilización](assets/isblank04.png)

**Nota**: La expresión CONTAINS distingue entre mayúsculas y minúsculas. Por ejemplo, si “Evento de caridad” aparece con inicial mayúscula en el campo de descripción, escríbalo del mismo modo.

**CONTAINS(“Evento de caridad”,{description})**

Tanto las expresiones ISBLANK como CONTAINS son útiles si desea ver si hay un valor presente. Sin embargo, puede ser más útil saber cuál es el valor, para verlo realmente o tener algún tipo de descriptor para proporcionar una mejor perspectiva.

Por ejemplo, en lugar de saber simplemente que un proyecto se ha convertido a partir de una solicitud, quiere averiguar el nombre de la solicitud original.

En ese caso, utilice la expresión CONTAINS junto con la expresión IF.

La mayoría de las veces, las expresiones de texto ISBLANK y CONTAINS se utilizan con IF.
