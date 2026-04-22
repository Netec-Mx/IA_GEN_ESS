# Práctica 3. Evaluar multimodalidad en análisis empresarial
## Objetivos
Determinar el valor de integrar texto e imágenes en el análisis con IA, comparando resultados frente a enfoques tradicionales basados únicamente en información textual.

## Duración aproximada
- 15 minutos.

## Tabla de ayuda
Para que puedas replicar esta práctica, se recomienda tener una cuenta en cualquiera de las siguientes plataformas:

| Sitio web | Enlace |
| --- | --- | 
| ChatGPT | https://auth.openai.com/create-account | 
| Copilot | https://copilot.microsoft.com/login o https://m365.cloud.microsoft/ |
| Gemini | https://gemini.google.com/app?hl=es |

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.

## Contexto de la práctica
Formas parte del área de Estrategia en una organización que analiza información económica para la toma de decisiones.

Trabajarás con el documento: “Perspectivas del Comercio Internacional de América Latina y el Caribe” (CEPAL)

Este documento contiene múltiples elementos visuales clave:
- Gráficas de aranceles por país
- Evolución del comercio (exportaciones/importaciones)
- Indicadores de intensidad tecnológica
- Datos comparativos históricos

El objetivo es evaluar qué herramienta interpreta mejor esta información visual y genera análisis más confiables.

### Parte 1. Interpretación de gráficas económicas
Primero evaluarás la capacidad de interpretar visualizaciones.

1. Descarga el archivo [impacto.pdf](../images/M5/P3/impacto.pdf)
2. Selecciona una gráfica del documento:

- Gráfico 1 Estados Unidos: aranceles aplicados a los países de América Latina y el Caribe, promedio ponderado, enero de 2025 y desde agosto de 2025 (En porcentajes)
- Gráfico 2 América Latina y el Caribe: variación anual del comercio de bienes por precio,
volumen y valor, 2015-2024 y proyección para 2025 (En porcentajes)
- Gráfico 3 Exportaciones mundiales de bienes y servicios, por intensidad tecnológica y de capital humano, 2005-2024 (En billones de dólares)

3. Sube el documento completo en Copilot, ChatGPT y Gemini y utiliza el siguiente prompt:

```text
Actúa como analista económico.
Analiza el Gráfico [Coloca el nombre del gráfico que seleccionaste] y responde:

1. ¿Qué muestra la gráfica?
2. ¿Cuáles son los patrones principales?
3. ¿Qué países o variables destacan?
4. ¿Qué conclusiones se pueden obtener?

Evita suposiciones que no estén respaldadas visualmente.
```

4. Observa la información del archivo y analiza las respuestas generadas:
-  ¿Interpretan correctamente la gráfica?
-  ¿Identifican patrones reales?
- ¿Confunden variables o ejes?
- ¿Generalizan sin evidencia?

### Parte 2. Extracción de datos desde visuales
Ahora evaluarás la precisión de los datos.

1. Utiliza el siguiente prompt:

```text
Extrae de la gráfica:
- Valores clave (por ejemplo: máximos, mínimos)
- Comparaciones entre países o variables
- Tendencias relevantes

Presenta la información en un formato de tabla.
```

2. Analiza las respuestas:
- ¿Los valores son correctos?
- ¿Se inventan datos?
- ¿La tabla es consistente con la gráfica?

### Parte 3. Interpretación de tendencias complejas
Evaluarás profundidad analítica con cada herramienta.

1. Selecciona el gráfico 2 o 3 y utiliza el siguiente prompt:

```text
Analiza la evolución mostrada en el Gráfico [Coloca el nombre del gráfico que seleccionaste].

Responde:
1. ¿Qué tendencia se observa a lo largo del tiempo?
2. ¿Existen cambios relevantes o puntos de quiebre?
3. ¿Qué posibles causas pueden explicar estos cambios?
4. ¿Qué implicaciones tiene para la región?

Diferencia claramente entre los datos observados e interpretación.
```

2. Analiza las respuestas:
- ¿Se distinguen correctamente los datos mostrados en el archivo contra la interpretación?
- ¿Se etectan cambios reales?
- ¿Las causas son razonables o no tienen justificación?

### Parte 4. Detección de inconsistencias
Aquí evalarás pensamiento crítico de las herramientas.

1. Utiliza el siguiente prompt:

```text
Compara lo que indica el texto del documento con lo que muestran las 3 gráficas.
Identifica:
- Posibles inconsistencias
- Diferencias de interpretación
- Información que podría ser mal entendida

No inventes información.
```

2. Analiza las respuestas:
- ¿Detectan contradicciones?
- ¿Evitan inventar inconsistencias?

### Parte 5. Aplicación a negocio
Ahora evaluarás la utilidad real.

1. Utiliza el siguiente prompt:

```text
Actúa como directivo.
Con base en la información visual del documento:

1. Identifica oportunidades de negocio
2. Señala riesgos relevantes
3. Propón acciones estratégicas

Justifica cada punto con evidencia de las gráficas.
```

2. Analiza las respuestas:
- ¿Las decisiones están basadas en los datos de las gráficas?
- ¿Usan únicamente la evidencia visual?
- ¿Las acciones estratégicas se pueden llevar a cabo de manera realista?
	

### Reflexión
- ¿Qué herramienta interpreta mejor los gráficos presentados?
- ¿Cuál es más precisa al analizar los datos de los gráficos?
- ¿Cuál comete más errores?
- ¿Cuál sería más confiable para realizar análisis de gráficos que se encuentran en archivos?


### Resultado esperado
Al finalizar la práctica, el participante será capaz de:
- Evaluar la capacidad de IA para interpretar gráficas y datos visuales.
- Detectar errores en la interpretación de información visual.
- Identificar riesgos de interpretación incorrecta.
- Comparar herramientas de IA en escenarios multimodales reales.
