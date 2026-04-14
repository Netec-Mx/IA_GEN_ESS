# Práctica 2. Verificación cruzada y razonamiento lógico para detectar inconsistencias
## Objetivo
Aplicar metodologías de validación y contraste de información para identificar inconsistencias en las respuestas generadas por la IA, fortaleciendo la confiabilidad en procesos de análisis y toma de decisiones.

## Duración aproximada
- 15 minutos.

## Tabla de ayuda
Para que puedas replicar esta práctica, se recomienda tener una cuenta en las siguientes plataformas:

| Sitio web | Enlace |
| --- | --- | 
| ChatGPT | https://auth.openai.com/create-account | 
| Copilot | https://copilot.microsoft.com/login |
| Gemini | https://gemini.google.com/app?hl=es |

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.


### Parte 1. Confiabilidad en la información
Formas parte de un equipo de análisis dentro de una empresa de logística. La Dirección General recibió un reporte operativo con resultados extraordinariamente positivos y te ha pedido validarlo antes de usarlo para la toma de decisiones estratégicas y su posible presentación ante el consejo directivo.

1. Descarga el archivo [reporte_operativo.docx](images/M2/P2/reporte_operativo.docx)
2. Ingresa a ChatGPT y selecciona el modelo "Instant: Para chats cotidianos".
    <img src="images/M2/P2/M2P2_1.png" alt="logo"/>
3. Escribe el siguiente prompt e integra el archivo reporte_operativo.docx:
    ```
    Analiza este reporte y dame conclusiones clave para la dirección.
    ´´´
4. Analiza la respuesta:
    - ¿La IA cuestiona los datos o da por hecho que son correctos?
    - ¿Presenta conclusiones sin validar la plausibilidad de la información?
5. Detecta inconsistencias de forma manual:
    - ¿Los porcentajes son realistas?
    - ¿Hay datos sospechosos?
6. Investiga en el explorador de tu preferencia:
    - Rangos realistas de eficiencia logística
    - Porcentajes comunes de reducción de costos
    - Limitaciones reales en transporte y telecomunicaciones
7. Compara con el reporte:
    - ¿Los valores son creíbles?
8. Regresa a ChatGPT y escribe:
    ```
    Analiza este reporte, identifica posibles inconsistencias y cuestiona los datos si parecen poco realistas. Además, realiza un análisis profundo para verificar si la información mencionada tiene sentido lógico.
    ´´´
9. Ejecuta nuevamente y analiza las respuestas.
10. Toma una postura como analista responsable:
    - ¿Confiarías en este reporte para presentarlo a la dirección?
    - ¿Qué datos requerirías verificar antes de avalarlo?
    - ¿Qué riesgos existirían si este reporte se acepta sin cuestionarlo?
11. ¿Qué respuestas crees que obtendrías si ejecutas estas instrucciones en el modelo "Thinking: Para preguntas complejas"?


### Parte 2. Mitigación de riesgos operativos mediante verificación lógica
Formas parte del equipo de Operaciones de una organización que utiliza un servicio basado en Inteligencia Artificial para analizar interacciones de atención al cliente y generar reportes ejecutivos breves.
Estos reportes, una vez aprobados internamente, se comparten con líderes directivos para apoyar decisiones estratégicas sobre inversión, procesos y calidad del servicio.

1. Analiza el siguiente caso:

    En el último reporte generado con apoyo de IA se incluyó la siguiente información:
    - Según el manual de operaciones, el tiempo de respuesta para clientes Gold es de 2 horas.
    - El reporte de infraestructura indica que el servidor tarda 3 horas en procesar cada solicitud Gold.
    - La política de marketing comunica que los clientes Gold reciben respuestas en tiempo real (menos de 5 minutos).
    El equipo sospecha que esta información no es consistente y que publicarla sin validación podría generar errores operativos, decisiones incorrectas o pérdida de confianza en los reportes ejecutivos.

2. Ingresa a Gemini y redacta un prompt para solicitar a la IA que audite la información anterior antes de que sea compartida con los líderes ejecutivos.
    Como referencia, puedes usar un prompt similar al siguiente:
    ```
    [Integra la información del paso anterior.]
    Analiza la información proporcionada y aplica razonamiento lógico paso a paso para detectar inconsistencias entre las distintas fuentes. Identifica qué datos entran en conflicto, explica por qué no pueden considerarse válidos al mismo tiempo y evalúa el riesgo operativo de compartir esta información sin validación. No inventes una respuesta oficial ni resuelvas la contradicción; limita tu análisis a la detección de inconsistencias y al nivel de riesgo que representan para la toma de decisiones.
    ```
3. Ejecuta tu prompt en Gemini y revisa cuidadosamente la respuesta obtenida.
4. Analiza el resultado y responde:
    - ¿La IA detectó todas las contradicciones?
    - ¿Explicó claramente por qué la información es inconsistente?
    - ¿Intentó imponer una respuesta como si fuera la correcta?
    - ¿Admitió que no es posible confirmar un dato oficial sin validación adicional?
5. Ahora solicita a la IA que proponga un protocolo breve de auditoría previa a la publicación de reportes operativos. 
    Puedes inspirarte en el siguiente prompt:
    ```
    Diseña un protocolo breve de 3 pasos que un empleado de Operaciones debe seguir antes de publicar cualquier dato generado o resumido por una IA sobre métricas de servicio al cliente. El protocolo debe ayudar a detectar contradicciones, validar fuentes y reducir riesgos operativos.
    ```
6. Ejecuta el prompt y revisa la propuesta generada.
7. Con base en la respuesta de la IA, identifica si el protocolo incluye elementos como:
    - Revisión de fuentes originales
    - Comparación entre documentos o áreas responsables
    - Validación humana antes de publicar
    - Escalamiento del caso cuando existan contradicciones
8. Finalmente, redacta en tus propias palabras una versión final del protocolo de auditoría que tu organización podría aplicar antes de compartir información operativa generada con IA.
9. Con base en lo anterior, responde:
    - ¿Qué pasaría si el reporte se presenta sin haber detectado las inconsistencias?
    - ¿Qué tipo de decisiones incorrectas podrían tomarse?
    - ¿Cómo impactaría esto en la operación o en la experiencia del cliente?

### Reflexión
- ¿La IA detectó automáticamente inconsistencias?
- ¿Qué cambió al definir instrucciones específicas?
- ¿Qué riesgos existen si una organización comparte información generada por IA sin verificarla?
- ¿Qué riesgos se generan cuando la IA intenta “resolver” contradicciones en lugar de alertar que la información no es confiable?
- ¿Qué papel juega el razonamiento humano en la validación de información?

### Resultado esperado
Al finalizar esta práctica, el participante será capaz de:
    - Detectar alucinaciones o errores en información generada por IA
    - Aplicar pensamiento crítico en el análisis de datos
    - Validar información en contextos empresariales
    - Diseñar protocolos de auditoría para reducir riesgos antes de la toma de decisiones