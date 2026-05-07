---
title: Comprender la búsqueda de recursos como colaborador
description: Obtenga información sobre cómo buscar recursos, buscar dentro de carpetas, optimizar los resultados de búsqueda, usar metadatos y palabras clave como filtros de búsqueda en [!UICONTROL DAM de Workfront].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-05T20:25:54.114Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 407
ht-degree: 89%

---

# Comprender la búsqueda de recursos como colaborador

Este vídeo contiene información sobre:

* Buscar recursos
* Buscar en carpetas
* Optimizar resultados de búsqueda
* Utilizar metadatos y palabras clave como filtros de búsqueda
* Ver detalles de la carpeta
* Ver y actualizar metadatos y palabras clave de recursos

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on&enablevpops=1)

## Criterios de búsqueda básicos

Una búsqueda básica examina los nombres de archivo, los campos de metadatos, las palabras clave y el contenido del recurso (según el tipo de recurso). No incluye el nombre de la carpeta.

La mayoría de los resultados de búsqueda son coincidencias exactas. Una excepción a esta regla de “coincidencia exacta” es cuando [!UICONTROL DAM de Workfront] busca el campo de nombre de archivo. [!UICONTROL DAM de Workfront] devuelve coincidencias de nombre de archivo parciales, en lugar de coincidencias exactas con el nombre de archivo.

## Operadores de usuario al buscar

Aunque las funciones básicas de búsqueda a menudo encontrarán los recursos que necesita, es posible que tenga que utilizar parámetros de búsqueda adicionales de vez en cuando.

### Coincidencias parciales

Para encontrar una coincidencia parcial, añada un asterisco al término de búsqueda. El asterisco sólo puede utilizarse al final de una palabra.

### Operador AND

Para encontrar resultados que contengan varios términos de búsqueda, escriba AND entre las palabras. Las palabras se pueden encontrar en cualquier orden. Al buscar en todos los campos, es posible que ambas palabras no estén presentes en el mismo campo. Por ejemplo, París AND torre encontrará recursos que tengan ambas palabras en cualquiera de los campos.

### Operador O

Utilice el operador O para buscar recursos que contengan cualquiera de los términos de búsqueda. Por ejemplo, París O Arco encontrarán recursos que tengan alguna de las palabras, pero no necesariamente ambas.

### Frase

Para encontrar una frase exacta, utilice comillas dobles alrededor de las palabras. Todas las palabras se encontrarán juntas y en orden. Por ejemplo, “Torre Eiffel” encontrará estas palabras en este orden exacto.

### Operador negativo

Si desea excluir una palabra de los resultados de búsqueda, ponga un signo menos (-) delante de la palabra. Asegúrese de que no haya un espacio entre el signo menos y la palabra. Por ejemplo, para excluir los recursos que tengan la palabra “torre” en los metadatos, la búsqueda se puede configurar como París -torre.

### Operador de campo vacío

Para buscar recursos que no tengan información en un campo de metadatos específico, escriba el campo que desea buscar con este formato: ?[xxxxx]. Por ejemplo, si desea buscar recursos que no tengan palabras clave asignadas, escriba ?[keyword] en el campo de búsqueda.
