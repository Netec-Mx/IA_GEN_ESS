# Práctica 3. Comparar prompts genéricos vs estructurados
## Objetivo
Evaluar la diferencia entre prompts simples y estructurados, identificando cómo el uso de criterios, restricciones y objetivos mejora significativamente la precisión de los resultados obtenidos.

## Duración aproximada
- 15 minutos.

## Tabla de ayuda
Para que puedas replicar esta práctica, se recomienda tener una cuenta las siguientes plataformas:

| Sitio web | Enlace |
| --- | --- | 
| ChatGPT | https://auth.openai.com/create-account | 
| Copilot | https://copilot.microsoft.com/login |
| Gemini | https://gemini.google.com/app?hl=es |

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.

### Parte 1. Comparar prompts genéricos vs estructurados en la gestión de proveedores
Formas parte del área de Logística de una empresa que trabaja con múltiples proveedores de transporte y servicios.
El equipo está comenzando a usar Inteligencia Artificial para apoyar el análisis y selección de proveedores, con el objetivo de optimizar costos, tiempos de entrega y niveles de servicio.
Antes de adoptar estos resultados en procesos reales, se debe evaluar qué tan confiables son las respuestas según el tipo de prompt utilizado.

1. Ingresa a ChatGPT, Gemini o Copilot.
2. Escribe el siguiente prompt:
    ```
    Dime cuál es el mejor proveedor logístico.
    ```
3. Lee cuidadosamente la respuesta generada y analiza:
    - ¿La IA menciona algún proveedor específico?
    - ¿Explica con base en qué criterios define “mejor”?
    - ¿La respuesta es aplicable a tu empresa?
4. Ahora escribe un prompt con un poco más de contexto, pero aún sin una estructura clara:
    ```
    Dime cuál es el mejor proveedor logístico para una empresa en [México].
    ```
5. Analiza la respuesta y responde:
    - ¿La IA ajusta la respuesta al país o contexto?
    - ¿Es ahora una recomendación más específica?
    - ¿La información es verificable?
    - ¿Qué información te sería útil para tomar una decisión?
6. Ahora utiliza un prompt estructurado, incorporando los elementos básicos de la ingeniería de prompts, por ejemplo:
    ```
    Actúa como un analista del área de Logística.
    Necesito evaluar proveedores de transporte para una empresa ubicada en [México] 
    que maneja envíos nacionales.
    Considera los siguientes criterios:
    - Cumplimiento de tiempos de entrega
    - Costo del servicio
    - Cobertura geográfica
    - Confiabilidad operativa
    El objetivo es identificar qué tipo de proveedor sería el más adecuado a partir de esos criterios.
    Realiza un análisis de alto nivel y explica los factores a considerar.
    ```
7. Revisa la respuesta y analiza:
    - ¿La IA logró el objetivo planteado?
    - ¿Respeta las restricciones?
    - ¿Reconoce límites en lugar de "adivinar" información?
8. Para evaluar si tu empresa realmente está optimizando costos, tiempos de entrega y niveles de servicio, es necesario definir métricas claras antes de solicitar un análisis. Para ello, vamos a proporcionar información y métricas básicas antes de pedir un análisis.

Define  los siguientes indicadores para tu empresa logística:
   - Costo promedio por envío
   - Tiempo promedio de entrega
   - Nivel de cumplimiento de entregas a tiempo (%)
   - Número mensual de incidencias o reclamaciones

Puedes usar el siguiente ejemplo como referencia:
    ```
    Actúa como un analista de logística.
    Nuestra empresa opera en [México] y actualmente trabaja con proveedores logísticos con 
    los siguientes indicadores promedio:
    - Costo promedio por envío: [$1,200 MXN]
    - Tiempo promedio de entrega: [3.5 días]
    - Nivel de entregas a tiempo: [85%]
    - Incidencias operativas mensuales: [23]
    El objetivo es evaluar si estos indicadores reflejan un buen desempeño logístico y 
    si existe margen de mejora en costos, tiempos de entrega o niveles de servicio.
    Realiza un análisis de alto nivel, explica cómo interpretar estas métricas y señala 
    qué tendencias o riesgos podrían evaluarse antes de tomar decisiones.
    ```
9. Solicita a la IA que con base en estos datos, determine qué proveedor o tipo de proveedor sería más conveniente para nuestra empresa.
Puedes usar este ejemplo como referencia:
    ```
    Compara las métricas anteriores con referencias generales del mercado logístico en
     [México] y con rangos de desempeño esperados para proveedores de paquetería y transporte conocidos.
    Con base en esta comparación:
    - Explica si el desempeño actual es bueno, promedio o mejorable
    - Justifica qué proveedor o tipo de proveedor podría ser más adecuado para mejorar costos, 
    tiempos de entrega y nivel de servicio.
    - Indica qué métricas deberían priorizarse para tomar la decisión final.
    Aclara cuando una comparación sea general o estimada para justificar la recomendación.
    ```
10. Analiza la respuesta de la IA y responde:
    - ¿La IA explicó por qué recomienda cierto proveedor o tipo de proveedor?
    - ¿Usó tus métricas como base para la comparación?
    - ¿Indicó claramente cuándo hablaba de referencias generales del mercado?
    - ¿La recomendación está sustentada o es solo descriptiva?
    - ¿Qué información adicional requerirías antes de tomar una decisión definitiva?

### Reflexión
- ¿Por qué un prompt poco estructurado puede llevar a recomendaciones poco confiables o difíciles de justificar?
- ¿Cómo influyó la definición de métricas (costos, tiempos, nivel de servicio) en la calidad del análisis generado por la IA?
- ¿Cómo aplicarías esta forma de estructurar prompts en procesos reales de evaluación y selección de proveedores dentro del área de Logística?

### Resultado esperado
Al finalizar esta práctica, el participante será capaz de:
   - Distinguir claramente entre prompts genéricos y prompts estructurados en contextos logísticos.
   - Reconocer los riesgos de utilizar IA con instrucciones ambiguas para la evaluación de proveedores.
   - Diseñar prompts que incorporen contexto, rol, instrucciones y formato de salida.
   - Evaluar de forma crítica recomendaciones de proveedores propuestas por IA, identificando supuestos, límites y necesidades de información adicional.
   - Utilizar la IA como apoyo para el análisis en la toma de decisiones logísticas, manteniendo control, criterio humano y responsabilidad final.