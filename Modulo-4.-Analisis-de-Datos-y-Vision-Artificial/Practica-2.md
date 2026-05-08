# Práctica 2. Extraer información de imágenes y cruzarla con datos
## Objetivos
Utilizar capacidades de visión artificial para extraer información relevante de imágenes y combinarla con datos estructurados, generando análisis más completos y útiles para la toma de decisiones.

## Duración aproximada
- 20 minutos.

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
Formas parte del área de Operaciones en una empresa logística encargada de la distribución y entrega de productos.

Para validar la correcta ejecución de las operaciones, la empresa cuenta con:

Evidencia visual (imágenes de entregas, almacenes y equipos)
Registros operativos en Excel donde se documenta el estado reportado por el personal

Sin embargo, se ha detectado que en algunos casos la información reportada no coincide con la evidencia visual, lo que puede generar riesgos operativos y decisiones incorrectas.

El objetivo de esta práctica es utilizar Inteligencia Artificial para analizar imágenes, estructurar la información obtenida y cruzarla con datos operativos para identificar inconsistencias y generar un análisis confiable.


### Parte 1. Análisis de imagenes
1. Ingresa a Gemini y crea una nueva conversación
2. Descarga el contenido de estas carpetas: [entregas e incidencias](https://drive.google.com/drive/folders/1fNY2BpTU4FF3QMicvA52tHzuRSQiDpQ3?usp=sharing) y selecciona una imagen (la que prefieras).
3. Carga la imagen en la herramienta y redacta el siguiente prompt:

```text
Actúa como un sistema de visión artificial aplicado a operaciones logísticas.

Analiza la imagen e identifica:
- Tipo de operación observada
- Estado general (correcto / incorrecto)
- Evidencia de cumplimiento o incumplimiento
- Posibles incidencias (daños, faltantes, desorden, riesgos)

Responde de forma estructurada.
Considera que la imagen fue tomada en el periodo del 10/abril/2026 al 16/abril/2026.
```

4. Analiza la respuesta:
- ¿La IA identifica correctamente la situación?
- ¿El análisis es claro y estructurado?
- ¿Existen ambigüedades en la interpretación?

### Parte 2. Extracción de puntos clave
Ahora transformarás el análisis visual en datos estructurados.

1. Utiliza el siguiente prompt y agrega la imagen seleciconada:

```text
A partir del análisis de la imagen, genera los siguientes campos:

- id_operacion
- resultado_visual (Correcto / Incorrecto)
- tipo_incidente (si aplica)
- nivel_riesgo (Alto / Medio / Bajo)
- descripcion_resumida (máx. 20 palabras)

Devuelve la información en formato de tabla.
```

2. Analiza la respuesta obtenida:
- ¿La información es clara y estructurada?
- ¿Los campos son útiles para análisis posterior?
- ¿La descripción es precisa y concisa?

### Parte 3. Estandarización de datos para cruce
En esta etapa asegurarás que los datos sean compatibles con sistemas en operación.

1. Utiliza el siguiente prompt:

```text
Normaliza los resultados para que sean compatibles con un archivo Excel operativo.

Asegúrate de:
- Usar categorías consistentes
- Evitar ambigüedades
- Mantener valores comparables con "estado_reportado"

Devuelve la tabla actualizada con lo solicitado.
```

2. Analiza la respuesta:
- ¿Los valores son consistentes?
- ¿Se pueden comparar fácilmente con datos de Excel?
- ¿Se eliminaron ambigüedades?

### Parte 4. Cruce con datos de Excel
Ahora integrarás la información visual con datos estructurados.

1. Descarga el archivo [registro_operaciones.xlsx](../images/M4/P2/registro_operaciones.xlsx)
2. Utiliza el siguiente prompt y agrega el archivo registro_operaciones.xlsx:

```text
Actúa como analista de operaciones.
Vas a trabajar con dos fuentes de información:

1. Datos del Excel "registro_operaciones.xlsx":
   - Contienen el campo "estado_reportado" (lo que el operador registró)

2. Resultados del análisis visual anterior:
   - Contienen el campo "resultado_visual" (lo que se observa en la imagen)

Tu tarea es:

1. Alinear ambos campos aunque tengan nombres diferentes, considerando su significado.
2. Comparar el estado reportado vs el resultado_visual (estado observado).
3. Identificar coincidencias e inconsistencias.

Genera:

- Tabla comparativa con:
  id_operacion | estado_reportado | resultado_visual | coincidencia (Sí/No)

- Lista de inconsistencias con explicación clara.
```

3. Analiza la respuesta:
- ¿Se identifican correctamente las discrepancias?
- ¿La respuesta generada es verificable y tiene sentido lógico?
- ¿Detectas posibles errores reales? ¿Cómo podrías corregirlo?

4. Utiliza ahora una versión mejorada del prompt para lograr que Gemini asocie la imagen analizada con alguno de los id_operacion que se encuentran en el archivo de excel. Puedes usar el siguiente prompt como inspiración para lograrlo:

```text
Actúa como analista de operaciones.

Tienes dos fuentes:

1. Evidencia visual (imagen analizada)
2. Registros del archivo Excel con:
   - id_operacion
   - estado_reportado
   - observaciones

IMPORTANTE:
- No inventes información.
- No asumas datos que no estén presentes.

Tu tarea es:

1. Analizar la imagen y describir brevemente la operación observada.
2. Comparar esa descripción con los registros del Excel.
3. Identificar qué id_operacion coincide mejor con la evidencia visual.

Para la coincidencia considera:
- estado_reportado
- observaciones
- coherencia operativa

Genera:

- id_operacion más probable
- nivel de confianza (Alto / Medio / Bajo)
- justificación breve basada en los datos

Si no hay suficiente información, indícalo explícitamente.
```

5. Analiza la respuesta generada:
- ¿Qué elementos del prompt permitieron que la IA realizara el cruce de información correctamente?
- ¿Cómo influyó el contexto asignado (rol de analista de operaciones) en la calidad de la respuesta?
- ¿Qué instrucciones fueron clave para evitar que la IA inventara información?
- ¿Cómo ayudó la estructura del prompt a guiar el razonamiento del modelo?
- ¿Qué habría pasado si el prompt no incluyera restricciones como “no inventes información”?
- ¿Qué tan importante fue especificar los campos disponibles (estado_reportado, observaciones, resultado_visual)?
- ¿La IA expresó algún nivel de incertidumbre o confianza? En caso contrario, ¿cómo podrías modificar el prompt para forzar este comportamiento?


### Reflexión
- ¿Qué valor aporta el uso de visión artificial en la validación de operaciones frente a depender únicamente de reportes manuales?
- ¿Qué riesgos pueden surgir cuando la evidencia visual no se contrasta con los datos registrados en sistemas?
- ¿Qué tan importante es estructurar correctamente la información extraída de imágenes antes de integrarla con otros datos?
- ¿Qué desafíos identificas al interpretar imágenes de forma automatizada (ambigüedad, contexto, calidad de imagen)?
- ¿Cómo impacta la estandarización de datos en la capacidad de análisis y comparación?
- ¿Qué limitaciones observas al depender exclusivamente de la IA para interpretar evidencia visual?
- ¿Cómo podrías aplicar este tipo de análisis en procesos reales de auditoría u operaciones?


### Resultado esperado
Al finalizar la práctica, el participante será capaz de:
- Utilizar herramientas de visión artificial para analizar imágenes en contextos operativos.
- Extraer información relevante y convertirla en datos estructurados.
- Diseñar prompts que permitan identificar incidencias, riesgos y estados operativos a partir de evidencia visual.
- Estandarizar datos para asegurar su compatibilidad con sistemas empresariales.
- Integrar información visual con datos estructurados mediante cruces analíticos.
- Detectar inconsistencias entre evidencia visual y reportes operativos.