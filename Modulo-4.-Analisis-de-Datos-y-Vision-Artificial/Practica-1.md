# Práctica 1. Categorizar datos con NLP
## Objetivos
Aplicar técnicas de procesamiento de lenguaje natural para organizar grandes volúmenes de datos no estructurados, transformándolos en información útil que facilite el análisis y la generación de indicadores estratégicos.

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
Formas parte del área de Experiencia del Cliente en una empresa de telefonía celular que, además de ofrecer servicios de telecomunicaciones, comercializa dispositivos móviles.

Durante los últimos meses, la empresa ha recopilado una gran cantidad de comentarios de clientes provenientes de encuestas de satisfacción, redes sociales y canales de soporte. Sin embargo, esta información se encuentra en formato no estructurado, lo que dificulta su análisis y aprovechamiento para la toma de decisiones.

La empresa quiere utilizar herramientas de Inteligencia Artificial para transformar estos comentarios en información estructurada, identificar patrones relevantes y generar indicadores estratégicos que permitan mejorar la experiencia del cliente y optimizar los servicios ofrecidos.

### Parte 1. Comprensión inicial de los datos
En esta primera etapa, analizarás un conjunto de comentarios de clientes para identificar patrones generales y comprender la información disponible.

1. Descarga el archivo [comentarios_clientes.txt](../images/M4/P1/comentarios_clientes.txt)
2. Ingresa a Copilot y en una nueva conversación carga el archivo comentarios_clientes.txt
3. Escribe el siguiente prompt:

```text
Analiza los comentarios de clientes que se encuentran en este archivo.
Identifica patrones generales, problemas frecuentes y posibles áreas de mejora.
```

4. Analiza la respuesta generada y responde:
- ¿Qué tipo de problemas identifica la IA con mayor frecuencia?
- ¿Existen patrones repetitivos en los comentarios?

### Parte 2. Definición de categorías de clasificación
En esta etapa, guiarás a la IA para estructurar los datos mediante categorías claras.

1. Utiliza el siguiente prompt:

```text
Actúa como analista de experiencia del cliente.
A partir de los comentarios del archivo comentarios_clientes.txt, define entre 5 y 8 categorías claras y mutuamente excluyentes para clasificar los comentarios.

Devuelve:
- Nombre de la categoría
- Descripción breve
- Ejemplos de comentarios que pertenecerían a ella
```

2. Analiza la respuesta generada:
- ¿Las categorías son claras y no se traslapan?
- ¿Cubren la mayoría de los comentarios?
- ¿Son útiles para un análisis empresarial?

### Parte 3. Clasificación masiva de comentarios (NLP)

1. Ahora aplicarás clasificación automática sobre los datos. Utiliza el siguiente prompt:

```text
Clasifica cada comentario en UNA sola categoría.

Además:
- Asigna un sentimiento: Positivo, Negativo o Neutral
- Genera una tabla estructurada

Formato de salida:
id_cliente | comentario | categoria | sentimiento
```

2. Observa la respuesta y responde:
- ¿La clasificación es consistente?
- ¿El sentimiento asignado tiene sentido?

### Parte 4. Generación de KPIs

1. Los datos clasificados se pueden tranformar en indicadores clave. Para lograr esto, puedes utilizar el siguiente prompt:

```text
A partir de la tabla clasificada, genera KPIs clave para la empresa.

Incluye:
- % de comentarios negativos
- Top 3 categorías con más incidencias
- % de experiencias positivas
- Principales causas de insatisfacción
- Indicadores accionables para mejora

Presenta los resultados en formato claro y ejecutivo.
```

2. Analiza la respuesta:
-  ¿Los indicadores son relevantes para la toma de decisiones?
- ¿Podrías usar estos KPIs en un reporte real?

### Parte 5. Generación de insights estratégicos

1. Interpreta los resultados desde una perspectiva de negocio, para lo cual puedes usar el siguiente prompt:

```text
Actúa como consultor de Customer Experience.

Con base en los KPIs anteriores:
- Identifica los principales problemas de la empresa
- Propón 5 acciones concretas de mejora
- Prioriza las acciones por impacto

Responde de forma ejecutiva (nivel directivo).
```

2. Analiza la respuesta obtenida:
- ¿Las recomendaciones están alineadas con los datos obtenidos en anteriores pasos?
- ¿Las acciones son claras y aplicables en el mundo real?
- ¿Consideras que la definición de prioridades tiene sentido lógico o existe algún factor que se omite?


### Reflexión
- ¿Cómo cambia tu capacidad de análisis al pasar de leer comentarios individuales a trabajar con datos clasificados y estructurados?
- ¿En qué tipo de escenarios empresariales resulta crítico clasificar grandes volúmenes de texto automáticamente?
- ¿Cómo podrías utilizar este tipo de análisis para generar mejoras reales en productos o servicios dentro de tu organización?


### Resultado esperado
Al finalizar la práctica, el participante será capaz de:
- Diseñar prompts que permitan identificar patrones y problemáticas recurrentes en grandes volúmenes de texto.
- Transformar datos procesados en indicadores clave (KPIs) relevantes para negocio.
- Generar insights estratégicos que permitan identificar áreas de mejora y oportunidades.
- Evaluar la calidad de los resultados generados por la IA en términos de coherencia, utilidad y aplicabilidad empresarial.
