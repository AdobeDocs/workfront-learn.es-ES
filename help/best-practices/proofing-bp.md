---
title: 'Práctica recomendada: revisión'
description: Explore las prácticas recomendadas de los expertos de Adobe Workfront acerca de la configuración, administración y uso de revisión en Workfront.
feature: Workfront Proof
role: Admin, Leader, User
level: Beginner
last-substantial-update: 2024-11-06T00:00:00Z
jira: KT-10920
exl-id: 394485ee-bb8f-4248-86a9-4c86174dd37f
source-git-commit: d9ccf45b157a4c66184cca0afadba35ef4c8615e
workflow-type: ht
source-wordcount: '1182'
ht-degree: 100%

---

# Práctica recomendada: revisión

## ¿Qué es una “práctica recomendada” de Adobe Workfront?

Las prácticas recomendadas son directrices que representan un procedimiento eficaz y efectivo, se adoptan fácilmente en la compañía y se pueden replicar correctamente en toda la organización.

Al revisar estas recomendaciones, hay que tener en cuenta que algunas prácticas recomendadas de Workfront son universales, mientras que otras pueden ser más específicas del tema. Utilice estas prácticas recomendadas como marco de ayuda para guiar la configuración y el uso del sistema Workfront.

## Navegación de esta página

Al desplazarse por esta página, primero encontrará una lista de alto nivel de todas las prácticas recomendadas sobre el tema. Esto le permite revisar las recomendaciones sin profundizar en los detalles de “por qué”.

La pregunta “¿Por qué son estas prácticas recomendadas?” se encuentra después de la lista de alto nivel, proporciona mayores detalles sobre algunas de las prácticas recomendadas y por qué se consideran un proceso, una herramienta, etc., cuya implementación se debe considerar al trabajar con Workfront.

</br>
</br>

## Revisión en las prácticas recomendadas de Workfront

* Tómese el tiempo para crear plantillas de flujos de trabajo de revisión.

* Deshabilite la configuración “Enviar correos electrónicos por medio de Workfront cuando un comentario se convierta en revisión” en los ajustes de Workfront.

* Utilice únicamente Solo lectura o Revisor para los ajustes “Funciones para usuarios que no sean destinatarios que abran una prueba de documento” en Workfront.

* Ajuste la configuración del back-end de prueba para que los usuarios vean las fechas límite en formato de reloj de 12 horas.

* Establezca una fecha límite de la revisión predeterminada como parte de la configuración del sistema.

* Ocultar la opción de decisión de la revisión no relevante.

* No reordene las opciones de decisión de la revisión en la configuración de la prueba.

* Establezca los valores predeterminados de usuario para las funciones de prueba y las alertas de correo electrónico.

* Establezca la función de prueba del creador de pruebas en el Revisor.

* Evite utilizar la función de revisión del Aprobador.

* Evite la opción de alerta de correo electrónico de revisión de todas las actividades.

</br>
</br>

## ¿Por qué estas son prácticas recomendadas?

**Práctica recomendada**

Tómese el tiempo para crear plantillas de flujos de trabajo de revisión.

**He aquí por qué**

Las plantillas no solo aceleran y optimizan el proceso de creación y asignación de pruebas, sino que también proporcionan coherencia entre los flujos de trabajo de prueba para tipos de recursos similares. También se aseguran de que a cada destinatario de la prueba se le asigne la función de prueba adecuada y la alerta de correo electrónico, y de que se haya establecido una fecha límite.

</br>
</br>

**Práctica recomendada**

Deshabilite la configuración “Enviar correos electrónicos por medio de Workfront cuando un comentario se convierta en revisión” en los ajustes de Workfront.



**He aquí por qué**

Cuando esta configuración está habilitada (que es de forma predeterminada), los usuarios pueden recibir varias notificaciones por correo electrónico para cada comentario en una prueba, una desde la funcionalidad de revisión y otra desde el propio Workfront. Estas duplicidades provocan confusión e interrupciones en los avisos por correo electrónico, así como una bandeja de entrada llena, lo que puede hacer que los usuarios ignoren las notificaciones de prueba. Esto, a su vez, podría suponer el incumplimiento de los plazos.



**Nota**: Este ajuste se encuentra en el menú principal de Workfront > Configuración > Correo electrónico > Revisión y aprobación.

</br>
</br>

**Práctica recomendada**

Utilice únicamente Solo lectura o Revisor para los ajustes “Funciones para usuarios que no sean destinatarios que abran una prueba de documento” en Workfront.



**He aquí por qué**

Las demás opciones para esta configuración requieren que se tome una decisión de la revisión, lo que puede entorpecer el flujo de trabajo. Por lo general, las personas que no están añadidas al flujo de trabajo solo tienen que ver la prueba o comentar, no aprobar, por lo que las opciones Solo lectura o Revisor son la mejor elección.



**Nota**: Este ajuste se encuentra en el menú principal de Workfront > Configuración > Revisión y aprobación.

</br>
</br>

**Práctica recomendada**

Ajuste la configuración del back-end de prueba para que los usuarios vean las fechas límite en formato de reloj de 12 horas.



**He aquí por qué**

El valor predeterminado es un formato de reloj de 24 horas, que puede resultar confuso para aquellos que no estén familiarizados con él. Para cambiar el formato, vaya al menú principal de Workfront > Revisión > Configuración de la cuenta > Usuarios. Haga doble clic en un usuario para seleccionar uno y, a continuación, edite el campo Formato de fecha en la sección Configuración personal. Debe seleccionar cada usuario de uno en uno para cambiarlos.

</br>
</br>

**Práctica recomendada**

Establezca una fecha límite de la revisión predeterminada como parte de la configuración del sistema.



**He aquí por qué**

Cuando se establece la fecha límite de la revisión predeterminada (la fecha de carga + x número de días laborables), si el creador de pruebas olvida añadir una fecha límite, Workfront aplica automáticamente esta fecha límite a cada prueba cargada.



**Nota**: Para encontrar esta configuración, vaya al Menú principal de Workfront > Revisión > Configuración de la cuenta > Configuración > Valores predeterminados de la prueba > Campo Fecha límite (+ días laborables).

</br>
</br>


**Práctica recomendada**

Ocultar la opción de decisión de la revisión no relevante.



**He aquí por qué**

Esta opción de decisión suele causar confusión entre los aprobadores, ya que las organizaciones a menudo no definen cuándo se debe utilizar la opción No relevante. La opción No relevante generalmente indica que la prueba no es relevante para el destinatario de la prueba y que no necesita tomar una decisión de aprobado o rechazado. Al seleccionar No relevante, esto permite que continúe el flujo de trabajo de prueba.


La opción No relevante no es necesaria en la mayoría de los flujos de trabajo de prueba.

**Nota**: Para encontrar esta configuración, vaya al menú principal de Workfront > Revisión > Configuración de la cuenta > Decisiones.

</br>
</br>

**Práctica recomendada**

No reordene las opciones de decisión de la revisión en la configuración de la prueba.



**He aquí por qué**

Cada configuración de la decisión de la revisión contiene un valor/peso específico que, si se reordena, puede generar confusión en las configuraciones de prueba. El orden de decisión y el valor/peso se utilizan como activadores de la fase de prueba y en la creación de informes.



**Nota**: Para encontrar esta configuración, vaya al menú principal de Workfront > Revisión > Configuración de la cuenta > Decisiones.

</br>
</br>

**Práctica recomendada**

Establezca los valores predeterminados de usuario para las funciones de prueba y las alertas de correo electrónico.



**He aquí por qué**

Estos ajustes se rellenan automáticamente al asignar un flujo de trabajo de prueba; aceleran el proceso y contribuyen a la coherencia de todos los flujos de trabajo de prueba.



**Nota**: La configuración predeterminada del usuario se encuentra en el menú principal de Workfront > Revisión > Configuración de la cuenta > Usuarios > y seleccionando al usuario para el cual se establecen los valores predeterminados.

</br>
</br>

**Práctica recomendada**

Establezca la función de prueba del creador de pruebas en el Revisor.



**He aquí por qué**

La función de prueba del Revisor garantiza que el creador de la prueba pueda realizar comentarios y acceder a los comentarios dejados por otros. La mayoría de las veces, el creador de la prueba no está obligado a tomar una decisión sobre una prueba que ha cargado. Las funciones de revisión Aprobador, Revisor y Aprobador, Autor, o Moderador requieren que se tome una decisión. Si al creador de pruebas se le asigna una de estas funciones de prueba, pero nunca toma una decisión, esto puede afectar negativamente a los plazos de la revisión.

</br>
</br>

**Práctica recomendada**

Evite utilizar la función de revisión del Aprobador.



**He aquí por qué**

La función de revisión del Aprobador no permite al usuario realizar comentarios sobre esta revisión. Esto podría llevar a que un usuario rechace la revisión, sin ninguna explicación porque no puede hacer comentarios. Utilice la función de revisión del Revisor y Aprobador en su lugar para que el usuario pueda proporcionar comentarios.

</br>
</br>

**Práctica recomendada**

Evite la opción de alerta de correo electrónico de revisión de todas las actividades.

**He aquí por qué**

Esta opción envía una notificación de correo electrónico de revisión cada vez que sucede algo con una revisión: se realiza un comentario, se publica una respuesta, se toma una decisión, etc. El destinatario ve esencialmente la actividad de revisión mientras sucede.

Para los propietarios y creadores de pruebas, la alerta de correo electrónico de Decisiones funciona mejor para los flujos de trabajo de revisión en varias etapas y la Decisión final funciona mejor para los flujos de trabajo de una sola etapa. Por lo general, todos los demás pueden configurarse como Deshabilitado, a menos que deseen que se les notifique a otras personas que realicen comentarios o decisiones (en cuyo caso, una de las opciones de correo electrónico de resumen podría funcionar mejor).
