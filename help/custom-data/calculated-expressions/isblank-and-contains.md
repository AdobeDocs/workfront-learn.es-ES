---
title: Uso de las expresiones ISBLANK y CONTAINS
description: Aprenda a utilizar y crear las expresiones ISBLANK y CONTAINS en un campo calculado de Adobe [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
TQID: 'https://experienceleague.adobe.com/q25cuV-wKAkoEJTzDIho1Ab-XTexGhEZCHReoE0TFxg'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 93%
---
# Uso de las expresiones ISBLANK y CONTAINS

Las expresiones CONTAINS e ISBLANK se utilizan para proporcionar valores verdaderos o falsos simples. La diferencia es que la expresión ISBLANK comprueba si el campo contiene un valor mientras la expresión de texto CONTAINS busca una cadena específica dentro de un campo.

Por ejemplo, para ver si un proyecto tiene una descripción, use la expresión ISBLANK. Si el campo de descripción está en blanco, la expresión devuelve un valor de verdadero. Si el campo de descripción no está en blanco, devuelve el valor de falso.

![Equilibrador de carga de trabajo con informe de utilización](assets/isblank01.png)

Para buscar un valor específico en la descripción, como &quot;evento de caridad&quot;, utilice la expresión de texto CONTAIN. Si encuentra &quot;evento de caridad&quot; en la descripción, el campo calculado dice &quot;verdadero&quot;. Muestra “falso” si no encuentra &quot;evento de caridad&quot;.

![Equilibrador de carga de trabajo con informe de utilización](assets/isblank02.png)

## ISBLANK

La expresión de texto ISBLANK incluye el nombre de la expresión y un punto de datos.

**ISBLANK({data point})**

![Equilibrador de carga de trabajo con informe de utilización](assets/isblank03.png)

En el ejemplo anterior (donde desea saber si el proyecto tiene una descripción), la expresión sería la siguiente:

ISBLANK({description})

## CONTAINS

La expresión de texto CONTAINS incluye el nombre de la expresión, la palabra o frase que está buscando y el campo en el que buscarlo.

**CONTAINS(&quot;frase&quot;,{fields})**

Asegúrese de colocar comillas alrededor de la palabra o frase que está buscando; de lo contrario, la expresión no será válida.

En el ejemplo anterior (al buscar &quot;evento de caridad&quot; en la descripción del proyecto), la expresión sería la siguiente:

**CONTAINS(&quot;evento de caridad&quot;,{description})**

![Equilibrador de carga de trabajo con informe de utilización](assets/isblank04.png)

**Nota**: La expresión CONTAINS distingue entre mayúsculas y minúsculas. Por ejemplo, si &quot;Evento de caridad&quot; aparece en mayúsculas en el campo de descripción, ponga en mayúsculas esta frase en la expresión.

**CONTAINS(&quot;Evento de caridad&quot;,{description})**

Tanto las expresiones ISBLANK como CONTAINS son útiles si desea ver si hay un valor presente. Sin embargo, puede ser más útil saber cuál es el valor, para verlo realmente o tener algún tipo de descriptor para proporcionar una mejor perspectiva.

Por ejemplo, en lugar de saber simplemente que un proyecto se ha convertido a partir de una solicitud, quiere averiguar el nombre de la solicitud original.

En ese caso, utilice la expresión CONTAINS junto con la expresión IF.

La mayoría de las veces, las expresiones de texto ISBLANK y CONTAINS se utilizan con IF.
