---
title: Comprender el [!UICONTROL Caso comercial]
description: Aprenda a utilizar el [!UICONTROL Caso comercial] en Workfront para evaluar los proyectos solicitados y compararlos con otros proyectos de su portafolio.
activity: use
team: Technical Marketing
feature: Strategic Planning
thumbnail: introduction-to-the-business-case.png
type: Tutorial
last-substantial-update: 2023-08-18T00:00:00Z
jira: KT-13836
role: User
level: Intermediate
exl-id: febb7378-81d4-4348-ac57-e9c4756966c0
source-git-commit: 64789af613bd6b38e58bd2c15df622729b883b22
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 57%

---

# Comprender el [!UICONTROL Caso comercial]

Como gerente, tu objetivo es asegurarte de que los proyectos contribuyan a los objetivos e iniciativas generales de la compañía de una manera positiva. Para tomar decisiones informadas, necesita información de los administradores del proyecto sobre lo que necesitarán para que sus proyectos avancen. Esto se puede hacer a través del [!UICONTROL Caso empresarial].

## ¿Qué es un [!UICONTROL Caso empresarial]?

Piense en un [!UICONTROL Caso empresarial] como modelo o propuesta para el trabajo que debe realizarse. Este capta estimaciones preliminares de alto nivel que le ayudan a planificar y administrar portafolios. Es donde se ingresan los posibles gastos, recursos y riesgos para construir un &quot;caso&quot; de por qué este proyecto beneficiaría a la compañía.

## Campos del [!UICONTROL Caso empresarial] recomendados para la priorización de proyectos

Cada sección del [!UICONTROL Caso empresarial] proporciona información única e importante sobre el proyecto. Vamos a echar un vistazo a las secciones que proporcionan información al [!UICONTROL Portfolio Optimizer] , que le ayudará a priorizar los proyectos de su portafolio.

## [!UICONTROL Información del proyecto]

La mayoría de la información introducida en la sección [!UICONTROL Información del proyecto] incluye detalles generales del proyecto, como el patrocinador y el programa al que pertenece el proyecto.

Sin embargo, hay un dato que podría afectar a la priorización del proyecto:[!UICONTROL Beneficio planificado].

![Una imagen del área del [!UICONTROL Beneficio planificado] en la sección [!UICONTROL Información del proyecto] del [!UICONTROL Caso empresarial]](assets/05-portfolio-management4.png)

El [!UICONTROL Beneficio planificado] representa la cantidad en dólares estimada de la que podría beneficiarse su empresa si se completa el proyecto.

Esta es una de las secciones que podría ser un punto de inflexión para que su empresa avance con este proyecto. Si puede mostrar que el proyecto contribuirá significativamente a los resultados finales de su empresa, las probabilidades son mayores de que se pueda aprobar más rápidamente.

## [!UICONTROL Gastos]

Los [!UICONTROL Gastos] representan los costes no laborales que se pueden incurrir durante la vida de un proyecto.

![Una imagen de la sección [!UICONTROL Gastos] en [!UICONTROL Caso empresarial]](assets/06-portfolio-management5.png)

Por ejemplo, los gastos de una conferencia de usuarios pueden incluir el pago del lugar, los artículos de regalo o los carteles para el vestíbulo del lugar.

## [!UICONTROL Presupuestación de recursos]

La sección [!UICONTROL Presupuestación de recursos] permite estimar la mano de obra que cree que se necesitará para que avance el proyecto. La información se extrae del [!UICONTROL Planificador de recursos] de [!DNL Workfront's].

![Una imagen de la sección [!UICONTROL Presupuestación de recursos] en el [!UICONTROL Caso empresarial]](assets/07-portfolio-management6.png)

Al introducir las necesidades estimadas para cada rol, esto crea un posible presupuesto necesario para el proyecto y da una idea de cuánto presupuesto del portafolio puede ser utilizado para el proyecto.

>[!NOTE]
>
>Debe tener conjuntos de recursos configurados en [!DNL Workfront] para usar esta sección del [!UICONTROL Caso empresarial].

## [!UICONTROL Riesgos]

Uno siempre tiene la más alta expectativa de que su proyecto se desarrolle sin contratiempos. Pero es importante identificar los riesgos y planificarlos en consecuencia. Ahí es donde el [!UICONTROL Riesgos] de la sección [!UICONTROL Caso comercial] puede ayudar.

![Una imagen de la sección [!UICONTROL Riesgos] en el [!UICONTROL Caso empresarial]](assets/08-portfolio-management7.png)

Debe intercambiar ideas con su equipo e identificar cualquier riesgo para el proyecto. Para los riesgos en los que puede estimar el coste si se produce el riesgo y la probabilidad de que se produzca, asegúrese de especificar estos valores. Workfront multiplicará el coste potencial por la probabilidad y lo colocará en una [!UICONTROL Riesgo potencial] fondos que se restarán de los fondos del proyecto [!UICONTROL Beneficio planificado] al calcular su [!UICONTROL Valor neto].

## [!UICONTROL Cuadros de resultados]

Los [!UICONTROL Cuadros de resultados] determinan en qué medida el proyecto propuesto se ajusta a las metas e iniciativas generales establecidos para el portafolio o la compañía.

Cada cuadro de resultados tiene una lista de preguntas y respuestas que tienen valores adjuntos. Cuando se rellena el informe de valoración, [!DNL Workfront] puede calcular la alineación del proyecto con los objetivos predeterminados de la organización.

![Una imagen de la sección del [!UICONTROL Cuadros de resultados] en el [!UICONTROL Caso empresarial]](assets/09-portfolio-management8.png)

>[!NOTE]
>
>Los jefes de proyecto no podrán ver los valores asignados a cada respuesta. Solo los usuarios que crean los cuadros de resultados pueden ver los valores.

## [!UICONTROL Caso empresarial] no obligatorio

El [!UICONTROL Caso empresarial] es flexible. Puede rellenar solo unas pocas secciones o ninguna. No se requiere ninguno de los campos. Sin embargo, cuanto más información rellene, más fácil será analizar y priorizar los proyectos que compiten por el mismo presupuesto o recursos.

Una vez que rellene el [!UICONTROL Caso empresarial], haga clic en el botón **[!UICONTROL Enviar]** en el panel de resumen del lado derecho de la ventana. Esto cambiará el estado del proyecto a [!UICONTROL Solicitado]. Ahora está listo para usar [!UICONTROL Optimización de Portfolio] para priorizar proyectos en el mismo portafolio.

>[!NOTE]
>
>La puntuación de alineación en la variable [!UICONTROL Caso comercial] el panel de resumen se genera al rellenar el cuadro de resultados. La puntuación de alineación es uno de los valores que se utiliza para calcular la puntuación [!UICONTROL Optimizador de portafolios].

<!-- 
Learn more graphic and links to documentation articles
* Overview of areas of the business case 
* Create a business case for a project   
* Create a scorecard 
* Apply a scorecard to a project and generate an alignment score 
-->
