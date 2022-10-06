---
title: 'Práctica recomendada: zona de pruebas de vista previa'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso del entorno de espacio aislado de vista previa para Workfront.
feature: Strategic Planning
role: Admin, Leader, User
level: Beginner
kt: 10917
exl-id: 5e172ad5-7e75-41cd-bce0-858095d13c6c
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Práctica recomendada: zona de pruebas de vista previa

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las mejores prácticas son directrices que representan un curso de acción eficaz y eficiente; sean adoptados fácilmente por usted y los usuarios de su empresa; y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, tenga en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco para ayudarle a guiar la configuración y el uso del sistema Workfront.

## Navegar por esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

La pregunta &quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de la vista previa de Simulador para pruebas

* Defina, haga un diagrama y pruebe los cambios en los procesos o configuraciones de Workfront existentes en el entorno de espacio aislado de vista previa antes de realizar actualizaciones en la instancia de producción.

</br>
</br>

## ¿Por qué estas prácticas recomendadas?

**Práctica recomendada**

Defina, haga un diagrama y pruebe los cambios en los procesos o configuraciones de Workfront existentes en el entorno de espacio aislado de vista previa antes de realizar actualizaciones en la instancia de producción.

**He aquí por qué**

El entorno limitado de vista previa sirve como réplica del entorno en directo. Aunque no se recomienda crear un nuevo entorno completo en el Simulador para pruebas antes de crearlo en la instancia de Producción, ya que esto crea trabajo adicional, es bueno utilizarlo como un entorno de prueba para los cambios que desee implementar.

Realizar pruebas de aceptación de usuarios (UAT) e incluir a usuarios seleccionados durante la fase de prueba de un cambio puede ayudarle a comprender mejor las necesidades y los flujos de trabajo de los usuarios. Esta es una buena manera de mejorar los flujos de trabajo de Workfront y su adopción dentro de su organización.


**Nota**: No es necesario crear primero todos los cambios que desee implementar en Workfront en el entorno de espacio aislado de vista previa. Muchos cambios de Workfront, como la creación de una nueva cola de solicitudes o plantilla de proyecto, se pueden realizar dentro del entorno de producción. Una buena regla general a la hora de realizar pruebas en la instancia de Producción es controlar la visibilidad de los objetos hasta que esté preparado para publicar en una audiencia mayor. Asegúrese de eliminar cualquier cosa que no desee utilizar para que el sistema permanezca limpio y manejable.
