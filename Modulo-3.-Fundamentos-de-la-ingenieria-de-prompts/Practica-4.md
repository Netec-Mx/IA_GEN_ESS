# Práctica 4. Aplicar Chain of Thought y Few-Shot
## Objetivo
Diseñar prompts avanzados que incorporen razonamiento paso a paso y ejemplos previos, con el objetivo de mejorar la precisión en tareas complejas y reducir errores en los resultados generados.

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

### Parte 1. Incorporación de razonamiento paso a paso
Formas parte del área de Contabilidad de una empresa que utiliza herramientas de Inteligencia Artificial para apoyar cálculos financieros, proyecciones y análisis contables.
El equipo ha observado que, cuando las solicitudes incluyen varias operaciones encadenadas (ingresos, costos, gastos, impuestos aplicables), la IA puede cometer errores si no se le indica explícitamente cómo razonar o qué estructura contable seguir.

Nota: En esta práctica se utiliza el concepto de impuesto sobre la renta de forma genérica. Cada país de Latinoamérica puede aplicar diferentes nombres, tasas y reglas, pero el razonamiento contable es similar.

1. Ingresa a ChatGPT
2. Escribe el siguiente prompt sin agregar instrucciones adicionales:
    ```
    Calcula la utilidad neta mensual de una empresa considerando:
    - Ingresos mensuales: $850,000
    - Costos operativos: $520,000
    - Gastos administrativos: $95,000
    - Impuesto sobre la renta del 30%
    ```
3. Lee la respuesta generada y responde:
    - ¿Qué resultado entrega la IA?
    - ¿Explica cómo llega a la utilidad neta?
    - ¿Puedes identificar fácilmente si el cálculo es correcto?
4. Probablemente hubo algún dato que no llegamos a comprender. Solicita explícitamente que la IA te explique su razonamiento paso a paso.

Puedes utlizar este prompt como inspiración:
    ```
    Calcula la utilidad neta mensual de la empresa con la siguiente información:

    - Ingresos mensuales: $850,000
    - Costos operativos: $520,000
    - Gastos administrativos: $95,000
    - Impuesto sobre la renta: 30%

    Realiza el cálculo paso a paso:
    1. Determina la utilidad antes de impuestos.
    2. Calcula el impuesto correspondiente.
    3. Obtén la utilidad neta final.

    Explica cada paso antes de mostrar el resultado final.
    Explica qué representa cada uno de los conceptos relacionados con la utilidad neta mensual.
    ```
5. Lee la respuesta generada y responde:
   - ¿El procedimiento contable es claro y ordenado?
   - ¿Serías capaz de corroborar cada operación y resultado?
   - ¿Con la información entregada, crees que podrías presentar un informe de resultados?

6. Solicita a la IA que genere un análisis de esta información y lo redacte como un reporte que presentarás al Gerente de Contabilidad. Guarda el reporte generado en una carpeta de tu Escritorio.


### Parte 2. Aplicación de Few‑Shot para guiar cálculos contables
La información con la que trabajaste previamente no sigue el formato que se utiliza en la organización, por lo que tendremos que enseñarle a la IA cómo debe entregarla.

1. Utiliza el siguiente prompt con ejemplos (Few‑Shot):
    ```
    Ejemplo 1:
    Ingresos: $500,000  
    Costos y gastos: $300,000  
    Utilidad antes de impuestos: $200,000  
    Impuesto sobre la renta (30%): $60,000  
    Utilidad neta: $140,000  

    Ejemplo 2:
    Ingresos: $1,200,000  
    Costos y gastos: $820,000  
    Utilidad antes de impuestos: $380,000  
    Impuesto sobre la renta (30%): $114,000  
    Utilidad neta: $266,000  

    Ahora resuelve el siguiente caso siguiendo exactamente el mismo esquema:

    - Ingresos mensuales: $850,000
    - Costos operativos: $520,000
    - Gastos administrativos: $95,000
    - Impuesto sobre la renta: 30%
    ```
2. Analiza la respuesta y reflexiona:
    - ¿La IA siguió la misma estructura de los ejemplos?
    - ¿El cálculo es coherente y consistente?
3. Repite el paso 1 en Gemini y comenta qué observas.


### Parte 3. Reto: Integración de Rol, Contexto, Instrucción y Formato de salida + Chain of Thought

1. La empresa cuenta con la siguiente información:

```text
Ingresos y costos mensuales

Ingresos mensuales promedio: $1,450,000
Costos directos de operación: $870,000
Gastos administrativos: $210,000
Gastos comerciales y de ventas: $95,000

Impuestos y ajustes mensuales

Impuesto sobre la renta: 30%
Provisión mensual para contingencias: $40,000
Depreciación mensual de activos: $55,000

Escenario anual

Crecimiento esperado de ingresos: 6% anual
Incremento esperado de costos y gastos: 4% anual
```

El objetivo es entender:
- la utilidad neta mensual actual
- la utilidad neta anual proyectada
- si el escenario es financieramente saludable

Analiza la información anterior para lograr el objetivo. Implementa Chain Of Thought en tu prompt junto con el Rol, Contexto, Instrucción y Formato de salida para comprender toda la respuesta generada y adaptarla al escenario en el que te encuentras.

Puedes inspirarte del siguiente prompt:

```text
Actúa como un analista contable y financiero.

Voy a proporcionarte información contable de una empresa.
Tu tarea es realizar los cálculos de forma clara, ordenada
y verificable, explicando paso a paso cada resultado.

Información mensual:
- Ingresos: $1,450,000
- Costos operativos: $870,000
- Gastos administrativos: $210,000
- Gastos comerciales y de ventas: $95,000
- Provisión para contingencias: $40,000
- Depreciación: $55,000
- Impuesto sobre la renta: 30%

Parte 1: 
Calcula la utilidad neta mensual, siguiendo estos pasos:
1. Calcula la utilidad antes de impuestos.
2. Aplica el impuesto correspondiente.
3. Obtén la utilidad neta final.

Parte 2:
A partir de la utilidad neta mensual, estima la utilidad neta anual actual.

Parte 3:
Proyecta la utilidad neta anual considerando:
- Crecimiento de ingresos del 6% anual.
- Incremento de costos y gastos del 4% anual.

Explica claramente cada paso, muestra los cálculos intermedios
y aclara cualquier supuesto que realices.
```

2. Una vez obtenida la respuesta, analiza y responde:
- ¿La IA siguió un orden lógico en los cálculos?
- ¿Obedeció cada una de las solicitudes definidas?
- ¿A partir de la respuesta generada, podrías explicar cuál es la diferencia entre utilidad antes de impuestos y utilidad neta?
- ¿La IA indica cuándo está haciendo proyecciones y cuándo realiza cálculos reales?
- ¿El razonamiento te permitiría defender los números ante un tercero?

3. Con base en los resultados obtenidos, solicita:
- Analizar si el margen de utilidad neta es saludable.
- Identificar qué rubros tienen mayor impacto negativo.
- Propón dos escenarios: conservador y optimista, y que la IA explique qué variables cambian en cada uno.
- Implementa Chain of Thought

4. El área de Contabilidad necesita preparar un reporte financiero ejecutivo que será presentado a la Dirección.

El reporte debe incluir:
- Resumen ejecutivo
- Análisis de resultados
- Evaluación de rentabilidad
- Proyección de escenarios y riesgos
- Conclusiones (claras y justificadas)

Para asegurar consistencia y calidad, debes guiar explícitamente a la IA sobre cómo estructurar sus respuestas, de forma que puedan integrarse directamente en el reporte final siguiendo una estructura parecida a la de este documento: [estructura_reporte.docx](../images/M3/P4/estructura_reporte.docx)

Crea tu prompt hasta obtener un resultado que cumpla con todas las características definidas.


### Reflexión
- ¿Qué diferencias observas en la calidad y confiabilidad de las respuestas cuando no se guía el razonamiento de la IA frente a cuando se solicita explícitamente un proceso paso a paso?
- ¿En qué tipo de tareas consideras más crítico utilizar Chain of Thought y por qué?
- ¿Cómo impacta el uso de ejemplos previos (Few-Shot) en la consistencia, estructura y precisión de las respuestas generadas?
- ¿Cómo cambia el comportamiento de la IA cuando se le asigna un rol específico dentro de un contexto profesional?
- ¿Qué ventajas aporta estructurar explícitamente el formato de salida en comparación con dejar la respuesta abierta?


### Resultado esperado
Al finalizar la práctica, el participante será capaz de:
- Diseñar prompts que obliguen a la IA a explicar su razonamiento paso a paso, facilitando la validación de cálculos complejos.
- Utilizar la técnica de Few-Shot para estandarizar formatos de salida y mejorar la consistencia en tareas repetitivas.
- Integrar rol, contexto, instrucciones claras y formato de salida para obtener respuestas alineadas a escenarios empresariales reales.
- Diferenciar entre resultados calculados y estimaciones proyectadas, identificando supuestos implícitos.
- Construir prompts que permitan obtener reportes ejecutivos listos para presentación, sin necesidad de retrabajo significativo.
- Evaluar críticamente las respuestas de la IA, determinando si son coherentes, verificables y defendibles ante terceros.