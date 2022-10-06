---
title: Buscar y organizar recursos en [!UICONTROL DAM de Workfront]
description: Obtenga información sobre cómo buscar recursos, buscar dentro de carpetas, optimizar los resultados de búsqueda, usar metadatos y palabras clave como filtros de búsqueda y más en [!UICONTROL DAM de Workfront].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
source-git-commit: d1f5c4a558f737cb8188e209a16b91b67d32285c
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Colaborador: buscar recursos

En este vídeo, aprenderá a:

* Buscar recursos
* Buscar en carpetas
* Optimizar resultados de búsqueda
* Utilizar metadatos y palabras clave como filtros de búsqueda
* Ver detalles de la carpeta
* Ver y actualizar metadatos y palabras clave de recursos

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12)

## Criterios de búsqueda básicos

Una búsqueda básica examina los nombres de archivo, los campos de metadatos, las palabras clave y el contenido del recurso (según el tipo de recurso). No incluye el nombre de la carpeta.

La mayoría de los resultados de búsqueda son coincidencias exactas. Una excepción a esta regla de &quot;coincidencia exacta&quot; es cuando la variable [!UICONTROL DAM de Workfront] busca el campo filename . [!UICONTROL DAM de Workfront] devuelve coincidencias de nombre de archivo parciales, en lugar de coincidir exactamente con el nombre de archivo.

## Operadores de usuario al buscar

Aunque las funciones básicas de búsqueda a menudo encontrarán los recursos que necesita, es posible que tenga que usar parámetros de búsqueda adicionales de vez en cuando.

### Coincidencias parciales

Para encontrar una coincidencia parcial, añada un asterisco al término de búsqueda. El asterisco sólo puede utilizarse al final de una palabra.

### operador AND

Para encontrar resultados que contengan varios términos de búsqueda, escriba Y entre las palabras. Las palabras se pueden encontrar en cualquier orden. Al buscar en todos los campos, es posible que ambas palabras no estén presentes en el mismo campo. Por ejemplo, la torre Y de París encontrará activos que tengan ambas palabras en cualquiera de los campos.

### Operador OR

Utilice el operador OR para buscar recursos que contengan cualquiera de los términos de búsqueda. Por ejemplo, París o Arco encontrarán activos que tengan alguna de las palabras, pero no necesariamente ambas.

### Frase

Para encontrar una frase exacta, utilice comillas dobles alrededor de las palabras. Todas las palabras se encontrarán juntas y en orden. Por ejemplo, &quot;Torre Eiffel&quot; encontrará esas palabras en ese orden exacto.

### Operador negativo

Si desea excluir una palabra de los resultados de búsqueda, ponga un signo de resta (-) delante de la palabra. Asegúrese de que no haya un espacio entre el signo menos y la palabra. Por ejemplo, para excluir los recursos que tengan la palabra &quot;torre&quot; en los metadatos, la búsqueda se puede configurar como París-tower.

### Operador de campo vacío

Para buscar recursos que no tengan información en un campo de metadatos específico, introduzca el campo que desee buscar con este formato: ?[xxxxx]. Por ejemplo, si desea buscar recursos que no tienen asignadas palabras clave, introduzca ?[keyword] en el campo de búsqueda.
