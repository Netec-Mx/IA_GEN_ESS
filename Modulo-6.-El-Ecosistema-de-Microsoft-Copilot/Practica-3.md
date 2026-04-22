# Práctica 3. Integrar análisis de datos y generación de contenido
## Objetivos
Automatizar un flujo completo que integre análisis de datos, generación de documentos y creación de presentaciones, demostrando el potencial de la IA en procesos end-to-end.

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

Formas parte del área de Inteligencia de Negocio (BI) en una empresa de tecnología que comercializa productos a nivel nacional.

La dirección general ha detectado:

- Variabilidad en ventas entre regiones
- Problemas en tiempos de entrega
- Impacto negativo en satisfacción del cliente
- Incremento en incidencias operativas

Se te ha solicitado realizar un análisis integral que permita:

- Identificar qué está pasando realmente
- Detectar riesgos y oportunidades
- Proponer acciones estratégicas

### Parte 1. Análisis automático en Excel

1. Descarga el archivo [analisis_ventas_clientes.xlsx](../images/M6/P3/analisis_ventas_clientes.xlsx)
2. Ingresa a Copilot, crea una nueva conversación, integra el archivo analisis_ventas_clientes.xlsx y añade el siguiente prompt:

```text
Analiza este conjunto de datos y genera:

- Principales tendencias de ventas
- Productos más y menos rentables
- Regiones con mejor y peor desempeño
- Relación entre incidencias, satisfacción y tiempo de entrega

Entrega insights claros, estructurados y accionables.
```

2. Analiza la respuesta generada:

- ¿Los insights realmente explican las actividades que realiza el negocio?
- ¿Se identifican problemas concretos?
- ¿Las conclusiones son accionables o solo descriptivas?

### Parte 2. Generación de KPIs
Para poder tomar decisiones, es necesario obtener algunas métricas.

1. Añade el siguiente prompt:

```text
Genera KPIs clave a partir de los datos:

- Ventas totales
- Margen promedio
- % de incidencias
- Satisfacción promedio
- Tiempo promedio de entrega

Incluye la interpretación de cada indicador en términos de negocio.
```

2. Analiza la respuesta generada:

- ¿Los KPIs son relevantes para Dirección?
- ¿Incluyen interpretación o solo números?
- ¿Permiten tomar decisiones?

### Parte 3. Identificación de patrones de negocio
La detección de patrones ayuda a identificar de manera más rápida las variables que influyen en el comportamiento de los datos.

1. Envía el siguiente prompt:

```text
Identifica patrones relevantes en los datos:

- Impacto de incidencias en satisfacción
- Diferencias entre canal Online vs Tienda
- Problemas operativos recurrentes

Explica la información como un analista de negocio, incluyendo posibles causas.
```

2. Analiza la respuesta generada:

- ¿Se identifican relaciones causa-efecto?
- ¿Las explicaciones son lógicas o superficiales?
- ¿Se detectan oportunidades de mejora?

### Parte 4. Creación de informe ejecutivo

1. Para generar un informe, envía el siguiente prompt:

```text
Genera un informe ejecutivo basado en estos resultados.

Incluye:

- Resumen ejecutivo
- KPIs clave
- Hallazgos principales
- Problemas detectados
- Recomendaciones estratégicas

Integra la información en un formato claro, estructurado y orientado a dirección.
```

2. Analiza la respuesta generada:

- ¿El informe comunica claramente los hallazgos?
- ¿Está enfocado en negocio y no en técnica?
- ¿Las recomendaciones son accionables?

### Parte 5. Refinamiento del informe
Optimiza el informe para una audiencia directiva.

1. Envía la siguiente solicitud:

```text
Mejora el informe para que tenga:

- Mayor claridad
- Lenguaje ejecutivo
- Enfoque en toma de decisiones

Elimina redundancias y simplifica el contenido.
```

Finalmente, solicita a Copilot que te entregue el informe en un archivo Word descargable.

2. Analiza la respuesta generada:

- ¿Se eliminó información innecesaria?
- ¿Está listo para presentar a dirección?

### Parte 6. Creación de infografía
En algunos casos, crear una imagen o una infografía puede hacer más sencilla y rápida la comprensión de contenidos.

1. Envía la siguiente solicitud:

```text
Crea una infografía basada en el informe anterior.

Incluye:
- KPIs principales
- Insights clave
- Problemas detectados
- Recomendaciones

Debe tener un formato visual tipo dashboard, debe ser claro y ejecutivo.
```

2. Analiza la respuesta generada:

- ¿La información es fácil de entender visualmente?
- ¿Se destacan los puntos clave?
- ¿Se evita saturación de información?

### Parte 7. Creación de presentación ejecutiva
Para mostrar el contenido del informe ante un público, vamos a crear una presentación de powerpoint.

1. Envía la siguiente solicitud:

```text
Crea una presentación ejecutiva descargable basada en el informe anterior.

Estructura de la PPT:
1. Resumen ejecutivo
2. KPIs
3. Hallazgos
4. Problemas
5. Recomendaciones
6. Sección de preguntas

Hazlo claro, profesional y orientado a toma de decisiones. 
Integra un diseño ejecutivo.
```

2. Analiza la respuesta generada:

- ¿La presentación cuenta una historia clara?
- ¿Está alineada a nivel directivo?
- ¿Integró todas las características definidas?

### Reflexión
- ¿Qué diferencia hay entre analizar datos y generar decisiones?
- ¿Qué valor aporta Copilot en la velocidad de análisis?
- ¿Qué riesgos existen si no se validan los insights?
- ¿Qué parte del proceso aporta más valor (análisis, informe o visualización)?
- ¿Cómo cambiaría el resultado si los datos fueran más complejos o incompletos?

### Resultado esperado
Al finalizar la práctica, el participante será capaz de:
- Analizar datos con Copilot en Excel de forma estructurada
- Generar KPIs e insights de negocio
- Transformar análisis en un informe ejecutivo claro
- Comunicar resultados mediante infografías y presentaciones
- Integrar múltiples herramientas de M365 Copilot en un flujo completo
- Convertir datos en decisiones estratégicas