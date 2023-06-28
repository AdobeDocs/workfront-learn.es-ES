---
title: Búsqueda y organización de recursos en [!UICONTROL WORKFRONT DAM]
description: Obtenga información sobre cómo buscar recursos, buscar en carpetas, optimizar los resultados de búsqueda, utilizar metadatos y palabras clave como filtros de búsqueda y mucho más en [!UICONTROL WORKFRONT DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Colaborador: buscar recursos

En este vídeo, aprenderá a hacer lo siguiente:

* Búsqueda de recursos
* Buscar en carpetas
* Optimizar los resultados de búsqueda
* Uso de metadatos y palabras clave como filtros de búsqueda
* Ver detalles de la carpeta
* Ver y actualizar metadatos y palabras clave de recursos

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on)

## Criterios básicos de búsqueda

Una búsqueda básica busca nombres de archivo, campos de metadatos, palabras clave y contenido de recursos (según el tipo de recurso). No incluye el nombre de la carpeta.

La mayoría de los resultados de búsqueda son coincidencias exactas. Una excepción a esta regla de &quot;coincidencia exacta&quot; es cuando el [!UICONTROL WORKFRONT DAM] busca en el campo nombre de archivo. [!UICONTROL WORKFRONT DAM] devuelve coincidencias parciales de nombre de archivo, en lugar de sólo coincidencias exactas de nombre de archivo.

## Operadores de usuario durante la búsqueda

Aunque las funciones de búsqueda básicas a menudo encontrarán los recursos que necesita, es posible que necesite utilizar parámetros de búsqueda adicionales de vez en cuando.

### Coincidencia parcial

Para buscar una coincidencia parcial, agregue un asterisco al término de búsqueda. El asterisco sólo puede utilizarse al final de una palabra.

### Operador AND

Para buscar resultados que contengan varios términos de búsqueda, escriba AND entre las palabras. Las palabras se pueden encontrar en cualquier orden. Al buscar en todos los campos, es posible que ambas palabras no estén presentes en el mismo campo. Por ejemplo, París Y Torre encontrarán recursos que tengan ambas palabras en cualquiera de los campos.

### Operador OR

Utilice el operador OR para buscar recursos que contengan cualquiera de los términos de búsqueda. Por ejemplo, París O Arco encontrará recursos que tienen cualquiera de las palabras, pero no necesariamente ambas.

### Frase

Para encontrar una frase exacta, utilice comillas dobles alrededor de las palabras. Todas las palabras se encontrarán juntas y en orden. Por ejemplo, &quot;Torre Eiffel&quot; encontrará esas palabras en ese orden exacto.

### Operador negativo

Si desea excluir una palabra de los resultados de búsqueda, coloque un signo menos (-) delante de la palabra. Asegúrese de que no haya ningún espacio entre el signo menos y la palabra. Por ejemplo, para excluir recursos que tengan la palabra &quot;torre&quot; en los metadatos, la búsqueda podría configurarse como Torre de París.

### Operador de campo vacío

Para buscar recursos que no tengan información en un campo de metadatos específico, introduzca el campo que desea buscar en este formato: ?[xxxxx]. Por ejemplo, si desea buscar recursos que no tengan asignadas palabras clave, escriba ?[palabra clave] en el campo de búsqueda.
