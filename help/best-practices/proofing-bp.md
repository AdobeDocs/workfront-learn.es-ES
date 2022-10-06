---
title: 'Práctica recomendada: prueba'
description: Explore las recomendaciones de prácticas recomendadas de los expertos de Adobe Workfront sobre la configuración, administración y uso de pruebas en Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
kt: 10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: 444f059d3cc26d8e3074a7145bc5419407c786cf
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Práctica recomendada: prueba

## ¿Qué es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las mejores prácticas son directrices que representan un curso de acción eficaz y eficiente; sean adoptados fácilmente por usted y los usuarios de su empresa; y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, tenga en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco para ayudarle a guiar la configuración y el uso del sistema Workfront.

## Navegar por esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de &quot;por qué&quot;.

La pregunta &quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prueba de las prácticas recomendadas de Workfront

* Tómese el tiempo para crear plantillas de flujo de trabajo de prueba.

* Deshabilite la configuración &quot;Enviar correos electrónicos desde Workfront cuando se haga un comentario en una prueba&quot; en la configuración de Workfront.

* Utilice solo Solo lectura o Revisor para los ajustes &quot;Funciones para usuarios que no sean destinatarios que abran una prueba de documento&quot; en Workfront.

* Ajuste la configuración del back-end de prueba para que los usuarios vean las fechas límite en formato de reloj de 12 horas.

* Establezca una fecha límite de prueba predeterminada como parte de la configuración del sistema.

* Ocultar la opción de decisión de prueba no relevante .

* No reordene las opciones de decisión de prueba en la configuración de prueba.

* Establezca los valores predeterminados de usuario para las funciones de prueba y las alertas de correo electrónico.

* Establezca la función de prueba del creador de pruebas en Revisor.

* Evite utilizar la función de prueba de Aprobador .

* Evite la opción de alerta de correo electrónico de prueba de todas las actividades .

</br>
</br>

## ¿Por qué estas prácticas recomendadas?

**Práctica recomendada**

Tómese el tiempo para crear plantillas de flujo de trabajo de prueba.

**He aquí por qué**

Las plantillas no solo aceleran y optimizan el proceso de creación y asignación de pruebas, sino que también proporcionan coherencia entre los flujos de trabajo de prueba para tipos de recursos similares. También se aseguran de que a cada destinatario de la prueba se le asigne la función de prueba adecuada y la alerta de correo electrónico, y de que se haya establecido una fecha límite.

</br>
</br>

**Práctica recomendada**

Deshabilite la configuración &quot;Enviar correos electrónicos desde Workfront cuando se haga un comentario en una prueba&quot; en la configuración de Workfront.



**He aquí por qué**

Cuando esta configuración está habilitada (que es de forma predeterminada), los usuarios pueden obtener varias notificaciones por correo electrónico para cada comentario en una prueba, una desde la funcionalidad de prueba y otra desde la propia Workfront. Estas notificaciones duplicadas provocan confusión e interrupciones en las notificaciones por correo electrónico, así como una bandeja de entrada de correo electrónico completa, lo que puede hacer que los usuarios ignoren las notificaciones de prueba que reciben. Lo que, a su vez, podría significar la falta de plazos.



**Nota**: Esta configuración se encuentra en el menú principal de Workfront > Configuración > Correo electrónico > Revisión y aprobación.

</br>
</br>

**Práctica recomendada**

Utilice solo Solo lectura o Revisor para los ajustes &quot;Funciones para usuarios que no sean destinatarios que abran una prueba de documento&quot; en Workfront.



**He aquí por qué**

Las demás opciones para esta configuración requieren que se tome una decisión de prueba, lo que puede echar por tierra el flujo de trabajo de pruebas. Por lo general, las personas que no se agregan al flujo de trabajo de prueba solo tienen que ver la prueba o realizar comentarios, no aprueban la prueba, por lo que las opciones Solo lectura o Revisor son su mejor apuesta.



**Nota**: Esta configuración se encuentra en el menú principal de Workfront > Configuración > Revisar y aprobar.

</br>
</br>

**Práctica recomendada**

Ajuste la configuración del back-end de prueba para que los usuarios vean las fechas límite en formato de reloj de 12 horas.



**He aquí por qué**

Seleccione la opción F j, Y, gi:a en la configuración de prueba para los usuarios que deseen ver fechas y horas límite de prueba en formato AM/PM. Para las áreas que utilizan un reloj de 12 horas, esto ayuda con la claridad de la fecha límite.



**Nota**: Para encontrar esta configuración, vaya al menú principal de Workfront > Corrección > Configuración de la cuenta > Usuarios > y edite el campo Formato de fecha para cada usuario.

</br>
</br>

**Práctica recomendada**

Establezca una fecha límite de prueba predeterminada como parte de la configuración del sistema.



**He aquí por qué**

Cuando se establece una fecha límite de prueba predeterminada (la fecha de carga + x número de días laborables), si el creador de pruebas olvida añadir una fecha límite, Workfront aplica automáticamente esta fecha límite a cada prueba cargada.



**Nota**: Para encontrar esta configuración, vaya al campo Menú principal de Workfront > Prueba > Configuración de la cuenta > Configuración > Proof Defaults > Deadline (+ días laborables) .

</br>
</br>


**Práctica recomendada**

Ocultar la opción de decisión de prueba no relevante .



**He aquí por qué**

Esta opción de decisión suele causar confusión entre los aprobadores, ya que las organizaciones a menudo no definen cuándo se debe utilizar la opción No relevante. La opción No relevante generalmente indica que la prueba no es relevante para el destinatario de la prueba y que no necesitan tomar una decisión aprobada o rechazada. Al seleccionar No relevante, esto permite que continúe el flujo de trabajo de prueba.


La opción No relevante no es necesaria en la mayoría de los flujos de trabajo de prueba.

**Nota**: Para encontrar esta configuración, vaya al menú principal de Workfront > Corrección > Configuración de la cuenta > Decisiones.

</br>
</br>

**Práctica recomendada**

No reordene las opciones de decisión de prueba en la configuración de prueba.



**He aquí por qué**

Cada configuración de decisión de prueba contiene un valor/peso específico que, si se reordena, puede generar confusión en las configuraciones de prueba. El orden de decisión y el valor/peso se utilizan como déclencheur de activación de la fase de prueba y en los informes.



**Nota**: Para encontrar esta configuración, vaya al menú principal de Workfront > Corrección > Configuración de la cuenta > Decisiones.

</br>
</br>

**Práctica recomendada**

Establezca los valores predeterminados de usuario para las funciones de prueba y las alertas de correo electrónico.



**He aquí por qué**

Estos ajustes se rellenan automáticamente al asignar un flujo de trabajo de prueba, acelerar el proceso y contribuir a la coherencia en todos los flujos de trabajo de prueba.



**Nota**: La configuración predeterminada del usuario se encuentra en el menú principal de Workfront > Corrección > Configuración de la cuenta > Usuarios > y seleccionando al usuario para establecer los valores predeterminados de .

</br>
</br>

**Práctica recomendada**

Establezca la función de prueba del creador de pruebas en Revisor.



**He aquí por qué**

La función de prueba del revisor garantiza que el creador de la prueba pueda realizar comentarios y acceder a los comentarios dejados por otros. La mayoría de las veces, el creador de pruebas no está obligado a tomar una decisión sobre una prueba que ha cargado. Las funciones de prueba Aprobador, Revisor y Aprobador, Autor o Moderador requieren que se tome una decisión. Si al creador de pruebas se le asigna una de estas funciones de prueba, pero nunca se decide, esto puede afectar negativamente a los plazos de prueba.

</br>
</br>

**Práctica recomendada**

Evite utilizar la función de prueba de Aprobador .



**He aquí por qué**

La función de prueba del aprobador no permite al usuario realizar comentarios sobre esta prueba. Esto podría llevar a que un usuario rechace la prueba, sin ninguna explicación porque no puede hacer comentarios. Utilice la función de prueba de Revisor y Aprobador en su lugar para que el usuario pueda proporcionar comentarios.

</br>
</br>

**Práctica recomendada**

Evite la opción de alerta de correo electrónico de prueba de todas las actividades .

**He aquí por qué**

Esta opción envía una notificación de correo electrónico de prueba cada vez que sucede algo con una prueba: se realiza un comentario, se publica una respuesta, se toma una decisión, etc. El destinatario ve esencialmente la actividad de prueba mientras sucede.

Para los propietarios y creadores de pruebas, la alerta de correo electrónico de Decisiones funciona mejor para los flujos de trabajo de prueba en varias etapas y la Decisión final funciona mejor para los flujos de trabajo en una sola etapa. Por lo general, todos los demás pueden configurarse como Deshabilitado, a menos que deseen que se les notifique a otras personas que realicen comentarios o decisiones (en cuyo caso, una de las opciones de correo electrónico de resumen podría funcionar mejor).
