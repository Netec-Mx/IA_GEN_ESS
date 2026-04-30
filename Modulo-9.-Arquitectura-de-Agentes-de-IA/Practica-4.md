# Práctica 4. Definir manejo de excepciones (Manual de Crisis)
## Objetivos
Establecer reglas y estrategias para que un agente responda adecuadamente ante solicitudes fuera de alcance, conflictos de información o situaciones críticas.

## Duración aproximada
- 10 minutos.

## Tabla de ayuda
Para que puedas replicar esta práctica no necesitas ninguna herramienta mas que tu propia capacidad de análisis.

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.


## Contexto de la práctica
Ya diseñaste un agente en la práctica anterior.

Ahora debes prepararlo para lo más importante: ¿Qué hace cuando algo sale mal?

Ejemplos reales:
- El usuario pide algo que el agente no puede hacer
- Hay datos contradictorios
- El usuario pide información sensible
- El agente no tiene suficiente información

Aquí es donde muchos agentes fallan.

### Parte 1. Definir límites del agente

1. Con base en la información que redactaste en las prácticas anteriores, responde:

- ¿Qué cosas NO puede hacer tu agente?
- ¿Qué temas están fuera de su alcance?

Por ejemplo:
- No puede aprobar pagos
- No puede dar asesoría legal
- No puede acceder a datos personales

2. Manejo de solicitudes fuera de alcance:

Define:

- ¿Cómo debe responder cuando el usuario pide algo que no puede hacer?
- ¿Qué debe decir el agente?
- ¿Qué alternativas ofrece?

Por ejemplo:

```text
“No puedo realizar esa acción, pero puedo orientarte sobre cómo hacerlo”
```

3. Manejo de información contradictoria:

- ¿Qué hace el agente si encuentra información inconsistente?

Por ejemplo, debería:
- Reconocer la inconsistencia
- No asumir
- Pedir validación

4. Manejo de preguntas sensibles o éticas:

- Define cómo responde el agente ante:
    - Datos personales
    - Temas sensibles
    - Información confidencial

Por ejemplo, debería:
- Evitar responder directamente
- Redirigir
- Mantener neutralidad

5. Manejo de incertidumbre

- ¿Qué debe hacer el agente cuando no sabe la respuesta?

Por ejemplo, debería:
- No inventar información
- Reconocer qie tiene un límite
- Ofrecer un siguiente paso

6. Para construir el Manual de Crisis, integra todo en este formato:

```text
MANUAL DE CRISIS DEL AGENTE

1. Límites del agente:
- ...

2. Solicitudes fuera de alcance:
- Respuesta:
- Alternativa:

3. Información contradictoria:
- ...

4. Preguntas sensibles:
- ...

5. Incertidumbre:
- ...
```

### Reflexión

- ¿Qué riesgo existe si el agente no tiene límites claros?
- ¿Qué tipo de errores serían más graves?
- ¿Qué situación sería crítica en tu contexto?

### Resultado esperado
El participante debe generar:
- Un manual claro
- Reglas de excepción bien definidas
- Estrategias de respuesta
- Control del comportamiento del agente
