# Práctica 4. Identificar PII y aplicar protocolos de anonimización antes de usar IA
## Objetivo
Reconocer datos sensibles dentro de la información utilizada en IA y aplicar técnicas de anonimización para proteger la privacidad y cumplir con buenas prácticas de manejo de datos.

## Duración aproximada
- 15 minutos.

## Tabla de ayuda
Para que puedas replicar esta práctica, se recomienda tener una cuenta en cualquiera de las siguientes plataformas:

| Sitio web | Enlace |
| --- | --- | 
| ChatGPT | https://auth.openai.com/create-account | 
| Copilot | https://copilot.microsoft.com/login |
| Gemini | https://gemini.google.com/app?hl=es |

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.


### Parte 1. Identificación de PII en información empresarial
Formas parte de un equipo que utilizará una herramienta de Inteligencia Artificial para analizar información interna y generar reportes, resúmenes o recomendaciones.
Antes de enviar cualquier información a la IA, es obligatorio identificar y proteger los datos personales.
1. Analiza el siguiente fragmento de información interna:

    Juan Pérez, con RFC JUAP800101XXX, trabaja en el área financiera desde 2018.
    Es responsable del proyecto Alfa para el cliente Comercial del Norte S.A.
    Su correo es juan.perez@empresa.com y su teléfono de contacto es 55‑1234‑5678.
    Actualmente reside en el estado de Jalisco.

2. (No respondas aún con la IA, este paso es completamente humano.) Identifica todos los datos personales o potencialmente sensibles (PII) presentes en el texto.
    - ¿Qué datos identifican a una persona de manera directa?
    - ¿Cuáles podrían permitir identificarla de forma indirecta?
    - ¿Existen datos que, al combinarse, aumenten el riesgo de identificar directa o indirectamente a una persona (reidentificación), incluso si algunos datos parecen poco sensibles por sí solos?
3. Para cada dato identificado, clasifica en:
    - Alto riesgo (identificación directa, datos oficiales, contacto)
    - Riesgo medio (ubicación, rol específico, proyecto)
    - Bajo riesgo (información general sin identificación)
    Este paso refuerza que no toda la información es igual de sensible.
4. Ingresa a Copilot, ChatGPT o Gemini y escribe el siguiente prompt:
    ```
    Anonimiza el siguiente texto eliminando datos personales identificables como nombres, RFC, correos, teléfonos y cualquier otro dato que permita identificar a una persona física. Mantén el contexto general del texto. 
    [pega aquí el texto del paso 1]
    ´´´
5. Analiza la respuesta de la IA:
    - ¿Eliminó o modificó correctamente los datos personales?
    - ¿Conserva el valor informativo del texto?
    - ¿El contexto sigue siendo útil para análisis?
    - ¿La anonimización fue suficiente o excesiva?
6. Ahora envía un prompt más específico:
    ```
    Anonimiza el siguiente texto eliminando cualquier dato personal identificable (PII), sustituyendo nombres y datos sensibles por roles genéricos. No elimines información relevante para el análisis organizacional.
    [pega aquí el texto del paso 1]
    ´´´
7. Compara ambos resultados y responde:
    - ¿Cuál versión es más útil para trabajar con IA?
    - ¿Cuál equilibra mejor privacidad y contexto?
    - ¿Por qué no siempre conviene "borrar" toda la información sensible?
    - ¿Qué riesgos existirían si el texto original se utilizara sin anonimizar?


### Parte 2. Anonimización insuficiente y riesgo de reidentificación
Después de aplicar un primer proceso de anonimización, el equipo considera que la información ya es “segura” para ser utilizada en una herramienta de IA que realizará análisis de desempeño y generación de reportes internos.
Sin embargo, no toda anonimización es suficiente, y ciertos datos, aun sin nombres explícitos, pueden permitir identificar indirectamente a una persona cuando se combinan.
1. Analiza el siguiente texto, que fue anonimizado antes de enviarse a una herramienta de IA:

    Un colaborador del área financiera, con más de 6 años en la empresa, es responsable del proyecto Alfa para un cliente del sector retail.
    El colaborador se ubica en el estado de Jalisco y es el principal contacto con el cliente.
    Su desempeño ha sido destacado en los últimos dos años.

2. Responde las siguientes preguntas:
    - ¿Este texto contiene todavía información que podría permitir identificar indirectamente a una persona?
    - ¿Qué datos, aunque no sean PII por sí solos, podrían contribuir a una reidentificación?
    - ¿Qué tan fácil sería identificar a este colaborador para alguien con conocimiento interno de la organización?
3. Reflexiona:
    - ¿Por qué eliminar el nombre y el correo no siempre es suficiente?
    - ¿Qué diferencia existe entre “anonimizar” y “hacer no identificable” un registro?
    - ¿Qué riesgos existen si la IA genera conclusiones o recomendaciones basadas en este texto?
4. Ingresa a Copilot, Gemini o ChatGPT y escribe el siguiente prompt:
    ```
    Analiza el siguiente texto y genera un resumen del perfil del colaborador y posibles recomendaciones.
    [pega aquí el texto del paso 1]
    ´´´
5. Analiza la respuesta de la IA y responde:
    - ¿La IA refuerza o amplifica la identificación indirecta del colaborador?
    - ¿Genera inferencias adicionales sobre la persona?
    - ¿Presenta el perfil como si se tratara de un individuo claramente definido?
6. Solicita a la IA que reescriba el texto original del paso 1 aplicando una anonimización más robusta, considerando:
    - Eliminación o generalización de ubicación
    - Reducción de referencias temporales específicas
    - Evitar combinaciones únicas (rol + proyecto + ubicación)

    Podrías obtener como resultado algo parecido a:

    Un miembro del área financiera participa en un proyecto estratégico para un cliente del sector retail.
    Su colaboración ha contribuido positivamente a los resultados del proyecto.

7. Responde:
    - ¿Qué cambió entre la anonimización parcial y la anonimización reforzada?
    - ¿Cuál versión reduce mejor el riesgo de reidentificación?
    - ¿Cuál sería más segura para enviar a una herramienta de IA en un entorno real?


### Parte 3. Definición de reglas organizacionales para anonimización antes del uso de IA
Después de identificar riesgos de exposición de datos personales y comprender que una anonimización insuficiente puede llevar a la reidentificación de personas, la organización decide establecer reglas formales para el uso de información con herramientas de Inteligencia Artificial.
El objetivo es garantizar que cualquier área que utilice IA (RH, Comercial, Operaciones, Finanzas, etc.) aplique criterios consistentes de protección de datos antes de enviar información a un sistema de IA.

1. Responde lo siguiente:
    - ¿Qué pasaría si cada equipo decide por su cuenta qué datos "son seguros" para enviar a IA?
    - ¿Qué riesgos existen si no hay reglas claras y documentadas?
    - ¿Qué áreas de la empresa podrían verse más afectadas por un mal manejo de datos personales?
2. Como primer paso hacia una política interna, identifica los principios mínimos que debería cumplir cualquier información antes de ser utilizada con IA (de manera general o en tu área laboral).
Piensa, por ejemplo, en:
    - Minimización de datos
    - Necesidad real del dato
    - Riesgo de identificación directa o indirecta
    - Uso del dato con un propósito específico
Redacta al menos 3 principios clave.
3. Ingresa a Copilot, Gemini o ChatGPT y utiliza el siguiente prompt:
    ```
    Ayúdame a diseñar reglas organizacionales para anonimizar información antes de utilizar herramientas de Inteligencia Artificial.
    Las reglas deben:
    - Proteger datos personales y sensibles (PII)
    - Evitar reidentificación indirecta
    - Ser aplicables a [distintas áreas de una empresa o el nombre del área a la que perteneces]
    - Considerar que los datos se usarán para análisis o generación de reportes
    Propón un conjunto breve de reglas prácticas.
    ´´´
4. Analiza la respuesta generada por la IA y responde:
    - ¿Las reglas son claras y aplicables en la práctica?
    - ¿Incluyen la idea de minimizar datos y evaluar riesgos?
    - ¿Mencionan validación humana o responsabilidades?
    - ¿Qué regla agregarías o ajustarías desde tu criterio?
5. Ahora, define los elementos clave que consideras indispensables para un protocolo de anonimización que puedas usar en el futuro antes de enviar información a cualquier herramienta de IA.
Asegúrate de que tu protocolo contemple al menos:
- Identificación de datos personales (PII)
- Evaluación del riesgo de reidentificación (datos combinados)
- Acciones de anonimización (eliminar, generalizar, sustituir)
- Validación final antes de usar IA
- Criterios para decidir cuándo no es adecuado usar IA
Una vez definidos estos elementos, solicita apoyo a la IA para redactar el protocolo, puedes utilizar un prompt similar al siguiente:
    ```
    Ayúdame a redactar un protocolo personal, práctico y reutilizable para anonimizar información antes de usar herramientas de Inteligencia Artificial.
    El protocolo debe incluir:
    - Identificación de datos personales (PII)
    - Evaluación del riesgo de reidentificación
    - Acciones concretas de anonimización
    - Una validación final antes de usar IA
    - Criterios para definir cuándo no se debe usar IA

    Redáctalo en forma de pasos claros y accionables que una persona pueda seguir en [su trabajo diario, una actividad empresarial o un área específica].
    ´´´
6. Lee el protocolo generado por la IA:
    - ¿Eliminarías, ajustarías o agregarías algún paso?
    - ¿En qué tipo de actividades consideras que este protocolo podría ayudarte?
Realiza los ajustes necesarios para que el protocolo se alinee con tu criterio y contexto laboral.

### Reflexión
- ¿Qué tipo de información nunca debería ingresarse en una herramienta de IA, incluso en entornos corporativos?
- ¿Por qué eliminar nombres o correos no siempre es suficiente para proteger la privacidad?
- ¿Qué riesgos existen cuando datos aparentemente "no sensibles" se combinan?
- ¿Cómo puede la IA amplificar el riesgo cuando se le entrega información mal anonimizada?
- ¿Qué responsabilidad tiene el usuario frente al uso de datos personales al trabajar con IA?
- ¿Cómo aplicarías el protocolo de anonimización que diseñaste en tu trabajo o entorno académico?

### Resultado esperado
Al finalizar esta práctica, el participante será capaz de:
    - Identificar datos personales y sensibles (PII) en información empresarial
    - Reconocer riesgos de reidentificación a partir de datos combinados
    - Aplicar técnicas básicas de anonimización sin perder el contexto necesario
    - Utilizar herramientas de IA de forma segura y responsable al trabajar con datos
    - Diseñar y aplicar un protocolo personal de anonimización antes de usar IA
    - Comprender los riesgos legales, éticos y de privacidad asociados al uso indebido de datos con IA
