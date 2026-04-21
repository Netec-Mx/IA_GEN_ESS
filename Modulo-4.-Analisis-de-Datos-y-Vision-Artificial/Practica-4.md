# Práctica 4. Convertir diagramas a estructuras digitales
## Objetivos
Transformar representaciones visuales o esquemas en estructuras digitales organizadas mediante IA, facilitando la documentación formal y la comunicación de procesos dentro de la organización.

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
Formas parte del área de Procesos dentro de una organización.

En distintas áreas del negocio (operaciones, atención al cliente, aprobaciones internas), los procesos suelen documentarse inicialmente de manera informal: dibujos a mano, esquemas rápidos o diagramas sin estructura clara.

Esto genera problemas como:
- Ambigüedad en la ejecución
- Falta de estandarización
- Dificultad para documentar y comunicar procesos

El negocio planea utilizar Inteligencia Artificial para interpretar los diagramas informales y comenzar a estructurar procesos de forma clara.

### Parte 1. Análisis del diagrama
En esta etapa interpretarás un diagrama hecho a mano.

1. Descarga el contenido de esta carpeta: [diagramas](../images/M4/P4/)
2. Selecciona alguno de los esquemas
3. Ingresa a ChatGPT
4. Carga la imagen del diagrama y escribe el siguiente prompt:

```text
Actúa como un sistema de interpretación de diagramas de procesos.
Analiza la imagen e identifica:
- Etapas del proceso
- Secuencia lógica
- Decisiones (sí/no u otras)
- Inicio y fin del flujo
- Posibles ambigüedades
Describe el flujo de manera clara.
```

2. Observa la respuesta:
- ¿La IA comprendió correctamente el flujo?
- ¿Identificó decisiones y secuencia?
- ¿Detectó ambigüedades del dibujo?

### Parte 2. Extracción estructurada del proceso
Ahora transformarás el flujo en una estructura organizada.

1. Utiliza el siguiente prompt:

```text
Convierte el flujo identificado en una estructura ordenada.

Devuelve:
- Lista numerada de pasos
- Decisiones claramente definidas
- Rutas alternativas del proceso
- Actores involucrados (si se identifican)

Formato claro y estructurado.
```

2. Observa la respuesta:
- ¿Los pasos siguen una secuencia lógica?
- ¿Las decisiones están bien definidas?
- En caso de que existan, ¿Se comprenden las rutas alternativas?

### Parte 3. Normalización a lenguaje profesional
En esta etapa convertirás el proceso en lenguaje empresarial formal.

1. Utiliza el siguiente prompt:

```text
Transforma la estructura en un proceso empresarial formal.
Asegúrate de:
- Usar lenguaje profesional
- Eliminar ambigüedades
- Definir claramente cada paso
- Mantener coherencia lógica

Entrega el proceso listo para documentación.
```

2. Analiza la respuesta:
- ¿El lenguaje es claro y profesional?
- ¿Se eliminaron ambigüedades?
- ¿El proceso es entendible para terceros?

### Parte 4. Generación de diagrama digital
Ahora transformarás el proceso en un formato replicable.

1. Utiliza el siguiente prompt:

```text
Convierte este proceso en una estructura de diagrama profesional.
Devuelve en formato que pueda replicarse en PowerPoint:

- Tipo de figura (Inicio, Proceso, Decisión)
- Texto de cada nodo
- Conexiones entre nodos

Formato tipo:
[Inicio] → [Proceso] → [Decisión: condición] → ...
```

2. Observa la respuesta:
- ¿El diagrama es claro y lógico?
- ¿Se puede replicar fácilmente?
- ¿Las conexiones son coherentes?

3. Ingresa el siguiente prompt para obtener una imagen profesional del diagrama:

```text
Genera una versión del proceso en una imagen con un estilo profesional 
que se utilizará para documentación.
```

4. Observa la respuesta:
- ¿El texto en la imagen es claro? 
- ¿El proceso es comprensible por cualquier usuario que lo lea?

### Parte 5. Documentación del proceso
En esta etapa generarás documentación formal.

1. Utiliza el siguiente prompt:

```text
Actúa como analista de procesos.
Genera un documento formal con:
- Nombre del proceso
- Objetivo
- Alcance
- Descripción del flujo
- Roles involucrados
- Consideraciones

Basado en el diagrama digital generado.
```

2. Analiza la respuesta:
- ¿El documento es claro y estructurado?
- ¿Está listo para uso empresarial?
- ¿La información es consistente con el flujo?

### Parte 6. Validación y mejora del proceso
Ahora analizarás críticamente el proceso generado.

1. Utiliza el siguiente prompt:
```text
Analiza el proceso generado y propón mejoras:
- Simplificación de pasos
- Eliminación de redundancias
- Mejora de decisiones
- Identificación de riesgos operativos

Entrega recomendaciones claras y justificadas.
```

2. Analiza la respuesta:
- ¿Las mejoras son relevantes?
- ¿Detecta problemas reales del proceso?
- ¿Las recomendaciones son accionables?


### Reflexión
- ¿Qué valor aporta transformar diagramas informales en procesos estructurados?
- ¿Qué desafíos identificas al interpretar información visual ambigua?
- ¿Qué tan importante es estandarizar procesos dentro de una organización?
- ¿Qué riesgos existen si un proceso no está claramente definido?
- ¿Cómo influye el lenguaje utilizado en la comprensión de un proceso?
- ¿Qué limitaciones observas al depender de la IA para interpretar diagramas?


### Resultado esperado
Al finalizar la práctica, el participante será capaz de:
- Interpretar diagramas informales mediante herramientas de IA multimodal.
- Convertir flujos visuales en estructuras ordenadas y comprensibles.
- Diseñar prompts para generar diagramas digitales replicables.
- Crear documentación empresarial formal a partir de procesos.
- Proponer mejoras estructuradas en procesos organizacionales.