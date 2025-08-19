# Práctica 1. Optimización de prompts según el contexto

## Objetivo de la práctica:
Al finalizar la práctica, serás capaz de:
- Aplicar los fundamentos de la ingeniería de prompts.
- Identificar las diferencias entre Zero-Shot, Few-Shot y Chain-of-Thought.

## Tabla de ayuda:
Para que puedas replicar las prácticas, se recomienda crear una cuenta en las siguientes plataformas:

| Sitio web | Enlace |
| --- | --- | 
| ChatGPT | https://auth.openai.com/create-account | 
| Copilot | https://copilot.microsoft.com/login |
| DeepSeek | https://www.deepseek.com/en |

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.

### Tarea 1. Análisis de errores y advertencias en archivo de Logs
#### Objetivo Visual 
Crear una tabla que resuma los errores que hay en el archivo de logs, un ejemplo es la siguiente imagen. 

<img width="581" height="361" alt="p1_1" src="https://github.com/user-attachments/assets/5e7d4bca-0c5d-47b7-b17e-1caa3af2c2ea" />


#### Duración aproximada:
- 12 minutos.

#### Paso 1: Preparación del Log
Descarga el archivo llamado [server_logs.xlsx](https://github.com/user-attachments/files/21859833/server_logs.xlsx) que contiene errores de un servidor.

#### Paso 2: Formula un Prompt Inicial (Vago)
Formula un prompt inicial para que el modelo analice el archivo. Este prompt debe ser deliberadamente vago.

Ejemplo de prompt:
```
Explica qué errores hay en este log.
```

#### Paso 3: Aplica Criterios de Ingeniería de Prompts
Ahora, mejora tu prompt inicial aplicando los siguientes criterios de ingeniería de prompts:

- Especificidad: Indica al modelo el formato de salida que deseas.

- Instrucción: Genera una tabla con las columnas: 'error', 'frecuencia', y 'hora'.

- Contexto: Proporciona información adicional sobre el sistema para ayudar al modelo a entender los datos. En este caso, se trata de errores en un servidor web Apache.

- Limitaciones: Establece restricciones para la respuesta. Por ejemplo, se le puede pedir que resuma los errores en un máximo de 5 categorías principales.

#### Paso 4: Compara los Resultados
Utiliza tus prompts optimizados en ChatGPT y DeepSeek y compara los resultados.
¿Qué modelo resumió mejor la información? ¿Cómo influyó la claridad y la estructura del prompt?

#### Resultado esperado
Tabla comparativa de errores.


<img width="520" height="278" alt="p1_2" src="https://github.com/user-attachments/assets/2d75cfdc-f716-4c37-9a59-f3e7023002c4" />

<img width="588" height="257" alt="p1_3" src="https://github.com/user-attachments/assets/9ce3edac-b091-45c9-a526-38967193eb5a" />





### Tarea 1. Descripción de la tarea a realizar.
Paso 1. Debe de relatar el instructor en verbo infinito, claro y conciso cada actividad para ir construyendo paso a paso en el objetivo de la tarea.

Paso 2. <!-- Añadir instrucción -->

Paso 3. <!-- Añadir instrucción -->

### Tarea 2. Descripción de la tarea a realizar.
Paso 1. Debe de relatar el instructor en verbo infinito, claro y conciso cada actividad para ir construyendo paso a paso en el objetivo de la tarea.

Paso 2. <!-- Añadir instrucción -->

Paso 3. <!-- Añadir instrucción -->

### Resultado esperado
En esta sección se debe mostrar el resultado esperado de nuestro laboratorio
![imagen resultado](../images/img3.png)
