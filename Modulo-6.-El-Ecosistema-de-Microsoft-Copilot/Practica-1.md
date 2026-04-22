# Práctica 1. Generar planes de proyecto con Copilot
## Objetivos
Utilizar Microsoft Copilot para transformar descripciones generales en planes de trabajo estructurados, incluyendo tareas, responsables y tiempos, facilitando la organización de proyectos.

## Duración aproximada
- 20 minutos.

## Tabla de ayuda
Para que puedas replicar esta práctica, se recomienda tener una cuenta en cualquiera de las siguientes plataformas:

| Sitio web | Enlace |
| --- | --- | 
| ChatGPT | https://auth.openai.com/create-account | 
| Copilot | https://copilot.microsoft.com/login |
| Gemini | https://gemini.google.com/app?hl=es |

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.

## Contexto de la práctica
Formas parte del área de Operaciones y Transformación Digital en una organización que busca mejorar su servicio al cliente mediante la implementación de nuevas herramientas tecnológicas.
Actualmente, los proyectos se definen de forma manual, lo que genera:

- Falta de claridad en tareas
- Retrasos por mala planificación
- Dificultad para asignar responsabilidades
- Problemas en el seguimiento

Se te ha solicitado diseñar un plan de proyecto completo y estructurado a partir de una idea inicial, utilizando Microsoft 365 Copilot Chat para acelerar la planeación y asegurar una ejecución más eficiente.

El resultado deberá ser lo suficientemente claro como para ser llevado directamente a herramientas operativas como Planner o Loop, facilitando la gestión del proyecto en equipo.

### Parte 1. Generación del plan de proyecto

1. Abre Copilot y envía el siguiente prompt:

```text
Actúa como project manager.
A partir de esta descripción:

"Implementar un nuevo sistema de atención al cliente en la empresa.
El proyecto debe incluir:
Selección de herramienta
Capacitación del equipo
Implementación
Seguimiento de resultados

Duración estimada: 2 meses
Equipo: TI, Operaciones y Atención al Cliente"

Genera un plan de proyecto que incluya:
- Fases del proyecto
- Tareas principales por fase
- Duración estimada
- Orden lógico de ejecución

Entrega la respuesta siguiendo un formato claro y estructurado.
```

2. Observa la información:

- ¿Las fases tienen sentido lógico?
- ¿El orden del proyecto es coherente?
- ¿El nivel de detalle es adecuado para iniciar la planeación?

### Parte 2. Desglose detallado de tareas
Profundizarás en el plan generado para convertirlo en un backlog operativo.

1. Ingresa el siguiente prompt:

```text
Convierte el plan en una lista detallada de tareas.
Incluye:
- Nombre de la tarea
- Descripción breve
- Dependencias entre tareas

Organiza la información en un formato tipo backlog.
```

2. A partir de las respuestas generadas, responde:

- ¿Las tareas son accionables?
- ¿Las dependencias están claramente identificadas?
- ¿Se puede ejecutar el proyecto solo con esta información?

### Parte 3. Asignación de responsables
Distribuirás el trabajo entre las áreas involucradas.

1. Ingresa el siguiente prompt:

```text
Asigna responsables a cada tarea considerando que estará involucrado:
- Equipo de TI
- Operaciones
- Atención al Cliente

Asegura una distribución lógica del trabajo.
```

2. A partir de las respuestas generadas, responde:

- ¿La asignación es realista?
- ¿Las responsabilidades están balanceadas?
- ¿Cada tarea tiene un responsable claro?


### Parte 4. Definición de fechas
Agrega temporalidad al plan.

1. Ingresa el siguiente prompt:

```text
Integra fechas estimadas para realizar cada tarea considerando:
- Duración total de 2 meses
- Dependencias entre tareas
- Secuencia lógica del proyecto
- Inicio el 20 de mayo de 2026
- El equipo de TI solo puede trabajar en sus tareas los días martes y viernes de 2 pm a 4 pm

Devuelve un cronograma estructurado.
```

2. Observa las respuestas generadas:

- ¿El cronograma es viable para implementarse en dos meses a partir de la fecha de inicio?
- ¿Respeta dependencias y secuencia de tareas?

### Parte 5. Preparación para Loop o Planner
Transformarás la información en un formato operativo. Adáptalo a la herramienta que utilices.

1. Existen muchas herramientas que permiten tener una mejor gestión de proyectos. Si conoces alguna, modifica el prompt para que el contenido se adapte a ella, en caso contrario, selecciona Planner o Loop (propias de Microsoft).

Envía el siguiente prompt a Copilot:

```text
Convierte esta información en un formato listo para usar en [Planner o Loop].

Incluye:
- Tarea
- Responsable
- Fecha de inicio
- Fecha de fin
- Estado (No iniciado)

Devuelve la respuesta en formato de tabla.
```

2. A partir de la respuesta generada, responde:
- ¿La estructura es directamente usable?
- ¿La tabla permite llevar un seguimiento claro?
- ¿Esta información se puede copiar fácilmente en Planner o Loop?

### Parte 6. Seguimiento del proyecto
Identifica los riesgos asociados al desarrollo del proyecto.

1. Envía el siguiente prompt a Copilot:

```text
Actúa como project manager.
A partir del plan generado:
- Identifica posibles riesgos del proyecto
- Propón indicadores de seguimiento (KPIs)
- Sugiere acciones correctivas en caso de retrasos

Responde de forma estructurada.
```

2. Análiza la información:
- ¿Los riesgos son realistas?
- ¿Los KPIs son medibles?
- ¿Las acciones ayudan a mantener el control del proyecto?

### Reflexión
- ¿Qué tanto reduce el tiempo de planeación el uso de Copilot?
- ¿Qué riesgos existen al depender completamente de la IA para estructurar proyectos?
- ¿En qué casos sería necesario validar manualmente el plan generado?
- ¿Qué valor aporta integrar este flujo con herramientas como Loop o Planner?
- ¿Cómo cambiaría la calidad del resultado si la descripción inicial del proyecto fuera más detallado?

### Resultado esperado
Al finalizar la práctica, el participante será capaz de:
- Transformar descripciones simples en planes de proyecto estructurados
- Generar tareas, responsables y cronogramas automáticamente
- Diseñar prompts para planeación y gestión de proyectos
- Preparar información para herramientas operativas como Loop o Planner
- Identificar riesgos y definir mecanismos de seguimiento