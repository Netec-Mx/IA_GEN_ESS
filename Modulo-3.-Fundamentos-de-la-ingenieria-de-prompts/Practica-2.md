# Práctica 2. Análisis financiero con y sin contexto para evaluar confiabilidad
## Objetivo
Comparar resultados generados por la IA con diferentes niveles de contexto para comprender cómo la calidad, precisión y utilidad de las respuestas depende de la información proporcionada.

## Duración aproximada
- 15 minutos.

## Tabla de ayuda
Para que puedas replicar esta práctica, se recomienda tener una cuenta en las siguientes plataformas:

| Sitio web | Enlace |
| --- | --- | 
| ChatGPT | https://auth.openai.com/create-account | 
| Copilot | https://copilot.microsoft.com/login o https://m365.cloud.microsoft/ |
| Gemini | https://gemini.google.com/app?hl=es |

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.

### Parte 1. Análisis financiero con diferentes contextos a partir de información en internet
Formas parte de un equipo que utiliza herramientas de Inteligencia Artificial para apoyar análisis financieros básicos, como estimaciones, comparaciones o resúmenes ejecutivos.
Antes de utilizar estos resultados para la toma de decisiones, es necesario evaluar qué tan confiables son las respuestas generadas según el prompt utilizado.

1. Ingresa a ChatGPT, Gemini o Copilot.
2. Escribe el siguiente prompt sin agregar contexto adicional:
    ```text
    Analiza la situación financiera de una empresa.
    ```
3. Lee cuidadosamente la respuesta generada y analiza:
    - ¿Qué supuestos realiza (tamaño, sector, país, ingresos)?
    - ¿De qué tipo de empresa habla la IA?
    - ¿Presenta datos concretos o generalidades?
    - ¿La respuesta podría aplicarse a cualquier empresa?
4. Ahora redacta un prompt incorporando contexto mínimo, por ejemplo:
    ```text
    Analiza la situación financiera de una empresa mediana del sector retail.
    ```
5. Analiza nuevamente la respuesta y responde:
    - ¿Qué cambió respecto al análisis anterior?
    - ¿La IA ajustó el lenguaje y los supuestos?
    - ¿Sigue siendo un análisis genérico?
6. Ahora utiliza un prompt más completo, considerando los elementos básicos de un buen prompt (contexto + instrucción + formato de salida), por ejemplo:
    ```text
    Analiza la situación financiera de una empresa mediana del sector retail en [nombre de tu País].
    La empresa tiene 10 años de operación, ingresos anuales aproximados de 2 millones de dólares y busca 
    identificar riesgos financieros generales.
    Elabora un análisis de alto nivel, sin usar datos confidenciales ni hacer suposiciones no fundamentadas.
    ```
7. Revisa la respuesta y analiza:
    - ¿El análisis es más específico?
    - ¿Se reducen las suposiciones arbitrarias?
    - ¿La respuesta se siente más coherente y enfocada?
    - ¿Cómo podrías obtener información más específica acerca de una empresa?
8. Ahora utiliza un prompt que incluya el nombre de una empresa real del sector retail en [nombre de tu País]. 
9. Escribe el siguiente prompt en la herramienta de IA:
    ```text
    Analiza la situación financiera de la empresa ["Cuidado con el Perro"] del sector retail en [México].
    ```
10. Analiza la respuesta generada y reflexiona:
    - ¿La IA presenta cifras financieras específicas?
    - ¿Indica de dónde obtiene la información o asume datos?
    - ¿Mezcla hechos conocidos con suposiciones?
    - ¿La respuesta suena convincente aunque no esté verificada?
11. Ahora prueba con un prompt más específico, por ejemplo:
    ```text
    Analiza la situación financiera de la empresa [Cuidado con el Perro], una empresa del 
    sector retail en [México] con más de 10 años de operación.
    Para este análisis:
    - Utiliza únicamente información pública y general.
    - Cita las fuentes de información que consultaste para obtener cada uno de los datos.
    - No asumas ingresos, utilidades o riesgos si no están explícitamente documentados.
    - Si no existe información suficiente, indícalo claramente.
    - Realiza un análisis de alto nivel y menciona las limitaciones del resultado utilizando 
    un lenguaje sin tecnicismos.
    ```
12. ¿Qué diferencias notas con respecto a la primer solicitud?

### Parte 2. Análisis financiero con diferentes contextos a partir de datos específicos
En esta parte trabajarás con datos numéricos financieros, para analizar cómo la IA interpreta cifras cuando no se proporciona contexto suficiente, y cómo cambia el resultado al estructurar correctamente el prompt.
El objetivo no es obtener un cálculo perfecto, sino evaluar la confiabilidad del análisis generado por la IA según la calidad del prompt.

1. Escribe el siguiente prompt sin agregar contexto adicional:
    ```text
    Analiza los siguientes datos financieros y dame una conclusión:
    Ingresos: 50,000,000 MXN 
    Costos: 42,000,000 MXN 
    Utilidad: 8,000,000 MXN 
    ```
2. Analiza la respuesta generada y responde:
    - ¿La IA indica si la empresa es rentable?
    - ¿Asume que el desempeño es positivo o negativo?
    - ¿Menciona métricas como margen o crecimiento sin conocer el contexto?
    - ¿Qué información falta para interpretar correctamente los números?
3. Ahora utiliza el siguiente prompt, agregando un poco de contexto:
    ```text
    Analiza los siguientes datos financieros de una empresa:
    Ingresos anuales: 50,000,000 MXN  
    Costos operativos anuales: 42,000,000 MXN   
    Utilidad anual: 8,000,000 MXN   
    Proporciona una conclusión general sobre su desempeño financiero.
    ```
4. De acuerdo con los resultados:
    - ¿El análisis es más claro que el anterior?
    - ¿La IA calcula márgenes o porcentajes?
    - ¿Sigue asumiendo información que no fue proporcionada?
    - ¿Qué tan útil es ahora la conclusión?
5. Ahora utiliza un prompt más completo, siguiendo la estructura básica de un buen prompt:
    ```text
    Analiza los siguientes datos financieros de una empresa del sector retail en México:
    - Ingresos anuales: 50,000,000 MXN  
    - Costos operativos: 42,000,000 MXN  
    - Utilidad neta: 8,000,000 MXN  
    - La empresa tiene más de 10 años de operación  
    - Los datos corresponden al último año fiscal  
    El objetivo es evaluar si el desempeño financiero es saludable en términos generales.
    Realiza un análisis de alto nivel, sin asumir información adicional como crecimiento, deuda o 
    comparaciones con años anteriores.
    Si no hay información suficiente para alguna conclusión, indícalo claramente.
    ```
6. Compara las tres respuestas obtenidas (sin contexto, con contexto mínimo y con contexto estructurado) y responde:
    - ¿En cuál caso la IA entrega más información sin fundamentos?
    - ¿Dónde se presentan conclusiones más cuidadosas?
    - ¿Cuál versión sería más apropiada para compartir con tu equipo o con dirección?
    - ¿En qué caso el riesgo de mala interpretación es mayor?

### Reflexión
- ¿Qué diferencias observaste entre un análisis generado con poco contexto y uno con contexto estructurado?
- ¿Por qué la IA tiende a completar o asumir información cuando los datos son incompletos o ambiguos?
- ¿Qué riesgos existen al analizar datos financieros sin especificar el alcance o las limitaciones del análisis?
- ¿Cómo cambió la confiabilidad del análisis al agregar contexto, objetivos y restricciones al prompt?
- ¿Por qué los datos numéricos, por sí solos, no garantizan conclusiones correctas?
- ¿Qué responsabilidad tiene el usuario al interpretar y utilizar análisis generados por IA en entornos reales?

### Resultado esperado
Al finalizar esta práctica, el participante será capaz de:
- Comprender cómo la estructura y el contexto del prompt influyen directamente en la calidad de las respuestas generadas por la IA.
- Identificar riesgos asociados al uso de prompts ambiguos, especialmente en análisis financieros.
- Analizar críticamente resultados generados por IA cuando se presentan datos numéricos sin contexto suficiente.
- Diseñar prompts estructurados que incluyan contexto, objetivo y límites claros.
- Evaluar la confiabilidad de análisis generados por IA antes de utilizarlos para la toma de decisiones.
- Reconocer el rol del usuario como responsable de proporcionar el contexto adecuado y validar los resultados obtenidos.