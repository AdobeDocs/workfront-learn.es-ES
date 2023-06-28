---
title: 'Práctica recomendada: revisión'
description: Explore las recomendaciones sobre prácticas recomendadas de los expertos de Adobe Workfront acerca de la configuración, administración y uso de las pruebas en Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Práctica recomendada: revisión

## ¿Cuál es una &quot;práctica recomendada&quot; de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un curso de acción eficaz y eficiente; que usted y los usuarios de su compañía adoptan fácilmente; y que se pueden replicar correctamente en toda la organización.

Cuando revise estas recomendaciones, tenga en cuenta que algunas de las prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de trabajo para guiar las configuraciones y el uso del sistema de Workfront.

## Navegar por esta página

A medida que se desplaza por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas para el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles del &quot;por qué&quot;.

&quot;¿Por qué son estas prácticas recomendadas?&quot; , que se encuentra después de la lista de alto nivel, proporciona buenos detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., debe considerar la implementación con su instancia de Workfront.

</br>
</br>

## Prácticas recomendadas de revisión en Workfront

* Tómese el tiempo necesario para crear plantillas de flujo de trabajo de revisión.

* Deshabilite la configuración &quot;Enviar correos electrónicos desde Workfront cuando se haga un comentario en una prueba&quot; en las configuraciones de Workfront.

* Utilice solo lectura o Revisor para la configuración &quot;Funciones para usuarios que no son destinatarios y que abren una revisión de documento&quot; en Workfront.

* Ajuste la configuración del back-end de prueba para que los usuarios vean los plazos en formato de reloj de 12 horas.

* Establezca una fecha límite de prueba predeterminada como parte de la configuración del sistema.

* Ocultar la opción de decisión de prueba No relevante.

* No reordene las opciones de decisión de prueba en la configuración de prueba.

* Establezca los valores predeterminados de usuario para los roles de prueba y las alertas de correo electrónico.

* Establezca la función de prueba del creador de la prueba en Revisor.

* Evite utilizar la función de prueba Aprobador.

* Evite la opción de alerta de correo electrónico de todas las pruebas de actividad.

</br>
</br>

## ¿Por qué son estas prácticas recomendadas?

**Práctica recomendada**

Tómese el tiempo necesario para crear plantillas de flujo de trabajo de revisión.

**He aquí la razón**

Las plantillas no solo aceleran y optimizan el proceso de creación y asignación de pruebas, sino que también proporcionan coherencia en los flujos de trabajo de prueba para tipos de recursos similares. También garantizan que a cada destinatario de prueba se le asigne la función de prueba y la alerta de correo electrónico adecuadas y que se haya establecido un plazo.

</br>
</br>

**Práctica recomendada**

Deshabilite la configuración &quot;Enviar correos electrónicos desde Workfront cuando se haga un comentario en una prueba&quot; en las configuraciones de Workfront.



**He aquí la razón**

Cuando esta configuración está habilitada (y lo está de forma predeterminada), los usuarios pueden recibir varias notificaciones por correo electrónico por cada comentario en una prueba, una desde la funcionalidad de revisión y otra desde el propio Workfront. Estas notificaciones duplicadas producen interrupciones y confusión de las notificaciones por correo electrónico, así como una bandeja de entrada de correo electrónico completa, lo que en última instancia puede hacer que los usuarios ignoren las notificaciones de prueba que reciben. Lo que, a su vez, podría significar plazos incumplidos.



**Nota**: esta configuración se encuentra en el menú principal de Workfront > Configuración > Correo electrónico > Revisión y aprobación.

</br>
</br>

**Práctica recomendada**

Utilice solo lectura o Revisor para la configuración &quot;Funciones para usuarios que no son destinatarios y que abren una revisión de documento&quot; en Workfront.



**He aquí la razón**

El resto de opciones de esta configuración requieren que se tome una decisión sobre la prueba, lo que puede descarrilar el flujo de trabajo de prueba. Por lo general, las personas que no se agregan al flujo de trabajo de prueba solo necesitan ver la prueba o hacer comentarios, no aprobar realmente la prueba, por lo que las opciones Solo lectura o Revisor son las mejores.



**Nota**: esta configuración se encuentra en el menú principal de Workfront > Configuración > Revisión y aprobación.

</br>
</br>

**Práctica recomendada**

Ajuste la configuración del back-end de prueba para que los usuarios vean los plazos en formato de reloj de 12 horas.



**He aquí la razón**

Seleccione la opción F j, Y, gi:a en la configuración de prueba para los usuarios que deseen ver los plazos y horas de prueba en formato AM/PM. Para las áreas que utilizan un reloj de 12 horas, esto ayuda con la claridad del plazo.



**Nota**: esta configuración se encuentra en el menú principal de Workfront > Revisión > Configuración de cuenta > Usuarios > y editando el campo Formato de fecha para cada usuario.

</br>
</br>

**Práctica recomendada**

Establezca una fecha límite de prueba predeterminada como parte de la configuración del sistema.



**He aquí la razón**

Cuando se establece un plazo de prueba predeterminado (la fecha de carga + x número de días laborables), si el creador de la prueba olvida añadir un plazo, Workfront aplica automáticamente este plazo a cada prueba cargada.



**Nota**: esta configuración se encuentra en el campo Menú principal de Workfront > Revisión > Configuración de cuenta > Configuración > Valores predeterminados de prueba > Plazo (+ días laborables).

</br>
</br>


**Práctica recomendada**

Ocultar la opción de decisión de prueba No relevante.



**He aquí la razón**

Esta opción de decisión suele causar confusión entre los aprobadores, ya que las organizaciones a menudo no definen cuándo se debe utilizar la opción No relevante. La opción No relevante generalmente indica que la prueba no es relevante para el destinatario de la prueba y no necesitan tomar una decisión aprobada o rechazada. Al seleccionar No relevante, esto permite que continúe el flujo de trabajo de prueba.


La opción No relevante no es necesaria en la mayoría de los flujos de trabajo de prueba.

**Nota**: esta configuración se encuentra en el menú principal de Workfront > Revisión > Configuración de cuenta > Decisiones.

</br>
</br>

**Práctica recomendada**

No reordene las opciones de decisión de prueba en la configuración de prueba.



**He aquí la razón**

Cada configuración de decisión de prueba contiene un valor/peso específico que, si se reordena, puede confundir las configuraciones de prueba. El orden de decisión y el valor/peso se utilizan como déclencheur de activación de la fase de prueba y en los informes.



**Nota**: esta configuración se encuentra en el menú principal de Workfront > Revisión > Configuración de cuenta > Decisiones.

</br>
</br>

**Práctica recomendada**

Establezca los valores predeterminados de usuario para los roles de prueba y las alertas de correo electrónico.



**He aquí la razón**

Esta configuración se rellena automáticamente al asignar un flujo de trabajo de prueba, lo que acelera el proceso y contribuye a la coherencia en todos los flujos de trabajo de prueba.



**Nota**: la configuración predeterminada del usuario se encuentra en el menú principal de Workfront > Revisión > Configuración de cuenta > Usuarios > y seleccionando el usuario para el que se establecerán los valores predeterminados.

</br>
</br>

**Práctica recomendada**

Establezca la función de prueba del creador de la prueba en Revisor.



**He aquí la razón**

La función de revisor de prueba garantiza que el creador de la prueba pueda realizar comentarios y acceder a los dejados por otros. La mayoría de las veces, el creador de la prueba no tiene que tomar una decisión sobre una prueba que ha cargado. Las funciones de aprobador, revisor y aprobador, autor o moderador requieren que se tome una decisión. Si al creador de la prueba se le asigna una de estas funciones de prueba pero nunca toma una decisión, esto puede afectar negativamente a los plazos de prueba.

</br>
</br>

**Práctica recomendada**

Evite utilizar la función de prueba Aprobador.



**He aquí la razón**

La función de prueba Aprobador no permite que el usuario realice comentarios sobre esta prueba. Esto podría hacer que un usuario rechazara la prueba, sin ninguna explicación, porque no podía hacer comentarios. En su lugar, utilice la función Revisor y aprobador para que el usuario pueda proporcionar comentarios.

</br>
</br>

**Práctica recomendada**

Evite la opción de alerta de correo electrónico de todas las pruebas de actividad.

**He aquí la razón**

Esta opción envía una notificación de correo electrónico de prueba cada vez que sucede algo con una prueba: se hace un comentario, se publica una respuesta, se toma una decisión, etc. El destinatario básicamente ve la actividad de prueba a medida que se produce.

Para los propietarios y creadores de pruebas, la alerta de correo electrónico de Decisions funciona mejor con flujos de trabajo de prueba de varias fases y la Decisión final funciona mejor con flujos de trabajo de una sola fase. Por lo general, todos los demás pueden configurarse como Deshabilitado, a menos que deseen que se les notifique de que otras personas están realizando comentarios o tomando decisiones (en cuyo caso, una de las opciones de correo electrónico de resumen podría funcionar mejor).
