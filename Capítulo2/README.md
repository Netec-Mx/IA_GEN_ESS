# Práctica 1. Optimización de _prompts_ según el contexto
## Objetivos
Al finalizar la práctica, serás capaz de:
- Aplicar los fundamentos de la ingeniería de prompts.
- Identificar las diferencias entre zero-shot, few-shot y chain-of-thought.

## Duración aproximada
- 60 minutos.

## Tabla de ayuda
Para que puedas replicar las prácticas, se recomienda crear una cuenta **gratuita** en las siguientes plataformas:

| Sitio web | Enlace |
| --- | --- | 
| ChatGPT | https://auth.openai.com/create-account | 
| Copilot | https://copilot.microsoft.com/login |
| DeepSeek | https://www.deepseek.com/en |

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.

### Tarea 1. Evaluación comparativa de razonamiento (zero-shot vs. chain-of-thought)

#### Objetivo visual 
Al explorar prompts de razonamiento en problemas técnicos con ChatGPT y DeepSeek, se obtendrán resultados similares a los siguientes.

<img width="543" height="372" alt="P1_T1_1" src="https://github.com/user-attachments/assets/e962df91-e222-4c00-9685-4570d8ac235b" />

<img width="637" height="575" alt="P1_T1_4" src="https://github.com/user-attachments/assets/5b3af997-9770-48eb-a05c-5a2eb85d7e6d" />

**Paso 1.** Entrega un problema de optimización de TI para verificar respuestas tipo zero-shot.

Ingresa el siguiente prompt en ChatGPT y DeepSeek:

```
Tienes un servidor con 8 GB de RAM y 4 CPU. Se ejecutan tres procesos A, B y C con consumo distinto.
¿Cómo distribuirías recursos para maximizar throughput?
```

- Envía el prompt y analiza la respuesta generada por cada servicio.

**Paso 2.** Implementa chain-of-thought.

Ingresa el siguiente prompt en ChatGPT y DeepSeek.

```
Tienes un servidor con 8 GB de RAM y 4 CPUs. Se ejecutan tres procesos A, B y C con consumo distinto.
¿Cómo distribuirías recursos para maximizar throughput?
Resuelve paso a paso, primero analiza consumo, luego distribuye recursos; finalmente, explica ventajas y limitaciones.
```

- Envía el prompt y analiza la respuesta generada por cada servicio.

**Paso 3.** Compara los resultados obtenidos con ChatGPT y DeepSeek.
- ¿Qué mejoras se obtuvieron con chain-of-thought?
- ¿Cuál de los modelos razonó con mayor detalle?

## Resultado esperado
Respuestas con chain-of-thought con ChatGPT y DeepSeek

<img width="342" height="1063" alt="P1_T1_2" src="https://github.com/user-attachments/assets/908b07e9-cb63-4585-88b7-7583f3a1f265" />

<img width="427" height="1051" alt="P1_T1_3" src="https://github.com/user-attachments/assets/c43a9747-ef81-48ef-99ef-ef0580a58fcb" />

### Tarea 2. Planeación estratégica, implementación con few-shot
Adaptar un mismo prompt base a diferentes audiencias (ejecutivos, técnicos y diseñadores de roadmap) utilizando la técnica de few-shot prompting.

Tu equipo debe diseñar una estrategia para migrar servicios a la nube en 6 meses.

## Objetivo visual 
<img width="406" height="497" alt="P1_T2_1" src="https://github.com/user-attachments/assets/bfa59ba1-6712-49f2-8ca2-af366c3a7e07" />


**Paso 1.** Entrega el prompt que define la necesidad del equipo.
Ingresa el siguiente prompt en ChatGPT, Copilot y DeepSeek.
```
Diseña una estrategia para migrar servicios a la nube en 6 meses.
```

Envía el prompt y analiza la respuesta generada por cada servicio (nivel de detalle y estilo).

**Paso 2.** Entrega el prompt que define la necesidad del equipo implementando ejemplos.
Ingresa el siguiente prompt en ChatGPT, Copilot y DeepSeek:
```
Ejemplo 1 (salida esperada):
Título: “Transformación Digital en 6 meses”
Resumen: Estrategia clara y concisa, 3 bullets de beneficios clave.
Estilo: Lenguaje ejecutivo, sin detalles técnicos.

Ejemplo 2 (salida esperada):
Título: “Migración a la nube: Impacto en el negocio”
Resumen: 3 objetivos estratégicos y una conclusión inspiradora.
Estilo: Formal y persuasivo.

Ahora diseña una estrategia para migrar servicios a la nube en 6 meses en este estilo ejecutivo para crear una presentación de PowerPoint.
```

- Envía el prompt y analiza la respuesta generada por cada servicio (formato, nivel de detalle y estilo).

**Paso 3.** Entrega el prompt que define la necesidad del equipo implementando ejemplos.
Ingresa el siguiente prompt en ChatGPT, Copilot y DeepSeek:
```
Ejemplo 1 (salida esperada)
Secciones: Introducción, Alcance, Arquitectura propuesta, Plan de migración, Riesgos.
Estilo: Detallado, técnico, con terminología de TI.

Ejemplo 2 (salida esperada)
Formato de lista numerada con pasos técnicos específicos y referencias a buenas prácticas de seguridad.

Ahora, diseña la estrategia para migrar servicios a la nube en 6 meses en este estilo técnico para crear un documento técnico.
```

- Envía el prompt y analiza la respuesta generada por cada servicio (formato, nivel de detalle y estilo).

**Paso 4.** Entrega el prompt que define la necesidad del equipo implementando ejemplos.
Ingresa el siguiente prompt en ChatGPT, Copilot y DeepSeek:
```
Ejemplo 1 (salida esperada)
Fase 1 (Mes 1-2): Evaluación → Actividades
Fase 2 (Mes 3-4): Migración piloto → Actividades
Fase 3 (Mes 5-6): Migración total → Actividades
Formato: tabla

Ejemplo 2 (salida esperada)
Diagrama tipo timeline con milestones clave y entregables en cada mes.

Ahora, diseña la estrategia para migrar servicios a la nube en 6 meses en este formato para crear un roadmap visual.
```

- Envía el prompt y analiza la respuesta generada por cada servicio (formato, nivel de detalle y estilo).

**Paso 5.** Analiza:
- ¿Qué herramienta se adaptó mejor al estilo esperado?
- ¿Qué diferencias hubo en el nivel de detalle?
- ¿Qué tanto ayudaron los ejemplos (few-shots) a guiar las respuestas?

## Resultado esperado
Los resultados generados podrían parecerse a los siguientes:

<img width="403" height="934" alt="P1_T2_2" src="https://github.com/user-attachments/assets/cc5eb046-ed3c-448c-ac3e-a7c97cd33414" />

<img width="407" height="929" alt="P1_T2_3" src="https://github.com/user-attachments/assets/52f8d77a-1644-4570-81db-0b702573e63f" />

<img width="525" height="839" alt="P1_T2_4" src="https://github.com/user-attachments/assets/de9da833-cdf1-443b-ad93-8b1e5ff6ffc3" />


### Tarea 3. Resolución de problemas de código
Eres un programador y encuentras dos fragmentos de código Python que no funcionan como esperabas. Necesitas identificar el error y entender por qué ocurre.

Los códigos con los que se trabajarán son los siguientes:
```python
def calcular_promedio(numeros):
    total = 0
for numero in numeros:
        total += numeros
    return total / len(numeros)

lista = [10, 20, 30]
print(calcular_promedio(lista))
```

```python
import pandas as pd
import dataframe_image as dfi

data = {
    "Criterio": [
        "Modelos disponibles",
        "Fine-tuning",
        "Precios",
        "Seguridad",
        "Caso ideal"
    ],
    "Amazon Bedrock": [
        "Claude, Llama 2, Cohere, etc.",
        "Sí (con datos propios)",
        "Pago por token + costo de modelo"
        "Privacidad AWS (HIPAA, GDPR)",
        "Empresas AWS, chatbots empresariales"
    ],
    "OpenAI (ChatGPT API)": [
        "GPT-4, GPT-3.5",
        "Limitado (solo para empresas)",
        "Alto (escalado por tokens)"
        "Estándar (API pública)",
        "Prototipos rápidos"
    ],
    "Azure OpenAI": [
        "GPT-4 + modelos de Microsoft",
        "Sí",
        Similar a OpenAI",
        "Integrado con Azure AD",
        "Empresas Microsoft"
    ],
    "Google Vertex AI": [
        "PaLM 2, Gemini",
        "Sí",
        "Costo variable por llamada",
        "Encriptación GCP",
        "Usuarios de Google Cloud"
    ]
}

df = pd.DataFrame(data)

print(df.to_markdown(index=False, tablefmt="github"))

dfi.export(df, "comparativa_modelos.png", max_cols=-1)
```

**Paso 1.** Entrega el prompt de manera directa.
Ingresa el siguiente prompt en ChatGPT, Copilot y DeepSeek:
```
Corrige el error en este código Python.
```

**Paso 2.** Entrega el prompt implementando chain-of-thought.

```
Analiza este código Python, identifica el error línea por línea y explícame por qué el error ocurre.
Después, proporciona el código corregido con comentarios que expliquen la solución.
```

**Paso 3.** Compara la calidad de las respuestas de los tres servicios.

## Resultado esperado
Se espera obtener la cadena de pensamiento de cada servicio (Copilot, ChatGPT y DeepSeek) para compararla con el análisis del Paso 1.

<img width="512" height="691" alt="P1_T3_2" src="https://github.com/user-attachments/assets/1d6c21ce-e4cf-4bb8-b66d-0af98921d292" />

<img width="353" height="1013" alt="P1_T3_1" src="https://github.com/user-attachments/assets/5ec3bf4a-b82f-4a28-97ca-e60bc9ffe140" />

<img width="367" height="1058" alt="P1_T3_3" src="https://github.com/user-attachments/assets/7cea20f7-c87e-4101-8e09-56831e5ba752" />

<img width="288" height="1075" alt="P1_T3_4" src="https://github.com/user-attachments/assets/594ff148-7ff9-4387-8335-0548d0d67703" />


### Tarea 4. Análisis de errores y advertencias en archivo de Logs
## Objetivo visual 
Con ayuda de ChatGPT y DeepSeek, crea una tabla que resuma los errores que hay en el archivo de logs, un ejemplo es la siguiente imagen. 

<img width="404" height="271" alt="p1_1" src="https://github.com/user-attachments/assets/5e7d4bca-0c5d-47b7-b17e-1caa3af2c2ea" />

**Paso 1.** Descarga el archivo con el que se trabajará que contiene errores de un servidor:
[server_logs.xlsx](https://github.com/user-attachments/files/21859833/server_logs.xlsx)

**Paso 2.** Formula un prompt inicial para que el modelo analice el archivo; debe ser deliberadamente vago.

Ejemplo de prompt:
```
¿Qué errores hay?
```

**Paso 3.** Aplica los criterios de ingeniería de prompts.
Mejora el prompt inicial aplicando los siguientes criterios de ingeniería de prompts tanto en ChatGPT como en DeepSeek:

- Especificidad: indica al modelo la actividad que desea que realice, el formato de salida y el archivo sobre el cuál se requiere que trabaje.

- Envía el prompt y analiza la respuesta generada por cada servicio.

- Instrucción: genera una tabla con las columnas: 'Error', 'Frecuencia', y 'Hora'.

- Envía el prompt y analiza la respuesta generada por cada servicio.

- Contexto: proporciona información adicional sobre el sistema para ayudar al modelo a entender los datos. En este caso, se trata de errores en un servidor web Apache.

- Envía el prompt y analiza la respuesta generada por cada servicio.
  
- Limitaciones: establece restricciones para la respuesta. Por ejemplo, pedir que resuma los errores en un máximo de 5 categorías principales.

- Envía el prompt y analiza la respuesta generada por cada servicio.

**Paso 4.** Compara los resultados.
- ¿Qué modelo resumió mejor la información?
- ¿Cómo influyó la claridad y la estructura del prompt?

## Resultado esperado
Tablas de errores

<img width="436" height="209" alt="p1_2" src="https://github.com/user-attachments/assets/2d75cfdc-f716-4c37-9a59-f3e7023002c4" />

<img width="441" height="193" alt="p1_3" src="https://github.com/user-attachments/assets/9ce3edac-b091-45c9-a526-38967193eb5a" />

### Tarea 5. Sesgos en la IA
Detecta sesgos en las respuestas generadas con DeepSeek.

## Objetivo visual 
<img width="511" height="621" alt="P1_T5_1" src="https://github.com/user-attachments/assets/0a0eab7c-1de2-4f8e-b539-73e9dbe189a6" />

**Paso 1.** Proporciona este prompt a DeepSeek:
```
Describe los beneficios de la IA en procesos de selección de personal.
```

**Paso 2.** Analiza:
- ¿Menciona género, edad, nacionalidad?
- ¿Qué lenguaje usa?
- ¿Hay estereotipos?

**Paso 3.** Proporciona este prompt a DeepSeek: 
```
¿Para qué negocios aplican esos beneficios y en qué países?
```

**Paso 4.** Analiza:
- ¿Menciona todos los países del mundo?
- ¿Identificas a tu país?
- ¿Tu organización forma parte de los negocios que pueden beneficiarse?
- ¿Identificas algún sector que no se beneficie?

**Paso 5.** Proporciona este prompt a DeepSeek:
```
Mi negocio no opera en esos contextos. ¿Podríamos decir que los beneficios de la IA están sesgados a países que sí tienen Internet?
```

**Paso 6.** Analiza:
- ¿El modelo te dio la razón o hizo lo posible por ocultar la verdad?
- ¿El modelo te ofreció alguna ayuda o una solución?
- ¿Consideras que todos los modelos son conscientes del sesgo que está incluido en sus datos de entrenamiento?

## Resultado esperado
Esta es una sección del análisis final que generó DeepSeek.

<img width="512" height="841" alt="P1_T5_2" src="https://github.com/user-attachments/assets/77727722-14d4-4dd0-9463-a4acf110bee9" />
