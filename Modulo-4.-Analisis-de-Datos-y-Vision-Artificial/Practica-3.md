# Práctica 3. Digitalizar información desde medios físicos
## Objetivos
Implementar herramientas de IA multimodal para automatizar la extracción de datos desde documentos físicos o imágenes, optimizando procesos de digitalización y gestión de información.

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
Formas parte del área de Control de Inventarios en una empresa que gestiona activos físicos en almacenes y puntos de operación.

Actualmente, parte del inventario se registra de manera manual o mediante evidencia visual (fotografías de productos, etiquetas, códigos QR y anotaciones a mano). Esto genera retrasos, errores de captura y falta de visibilidad en tiempo real.

La empresa quiere utilizar Inteligencia Artificial para extraer información desde imágenes, convertirla en datos estructurados, integrarla con el inventario base del sistema e identificar diferencias y riesgos operativos.

### Parte 1. Análisis de imagen (visión artificial)
En esta etapa analizarás visualmente productos e información de inventario.

1. Ingresa a Gemini y crea una nueva conversación
2. Descarga el contenido de esta carpeta: [inventario](../images/M4/P3/) y selecciona una imagen (la que prefieras).
3. Selecciona una de las imágenes disponibles de la carpeta.
4. Carga la imagen en la herramienta y escribe el siguiente prompt:

```text
Actúa como un sistema de visión artificial aplicado a inventarios.
Analiza la imagen e identifica:
- Productos visibles
- Cantidad estimada
- Etiquetas, códigos o números de serie
- Estado físico del producto (correcto, dañado, incompleto)

Responde de forma estructurada.
```

5. Analiza la respuesta:
- ¿La IA identifica correctamente los elementos?
- ¿Existen ambigüedades en la interpretación?
- ¿Qué tan confiable parece la estimación de cantidades?

6. Repite el paso 4 con las imágenes restantes.

### Parte 2. Extracción de datos estructurados
Ahora convertirás el análisis visual en datos organizados.

1. Utiliza el siguiente prompt:

```text
Convierte el análisis anterior de las 3 imágenes en datos estructurados.
Genera una tabla con:
- id_producto (si es visible o inferido)
- nombre_producto
- cantidad_detectada
- codigo_detectado (si aplica)
- estado
- ubicacion_estimada

Considera un formato tipo Excel.
```

2. Analiza la respuesta:
- ¿La tabla es clara y utilizable?
- ¿Los datos son consistentes?
- ¿Existen campos incompletos o inferidos?

### Parte 3. Normalización de datos
En esta etapa prepararás los datos para integrarlos con sistemas reales.

1. Utiliza el siguiente prompt:

```text
Normaliza los datos extraídos para que sean compatibles con un sistema de inventario.

Asegúrate de:
- Usar nombres consistentes
- Estandarizar estados (Correcto, Dañado, Faltante)
- Evitar duplicados

Devuelve la información ordenada en formato de tabla.
```

2. Observa la respuesta:
- ¿Los nombres están estandarizados?
- ¿Los estados son comparables?
- ¿Se eliminaron inconsistencias?

### Parte 4. Cruce con inventario base
Ahora integrarás los datos visuales con el sistema de inventario.

1. Utiliza el siguiente prompt y agrega el archivo inventario_base.xlsx:

```text
Actúa como auditor de inventarios.
Trabajarás con dos fuentes:

1. Datos del Excel "inventario_base.xlsx" (stock_sistema)
2. Inventario detectado en imágenes anteriores (cantidad_detectada)

IMPORTANTE:
- No inventes información.
- Usa únicamente los datos disponibles.

Tu tarea es:
1. Alinear los productos entre ambas fuentes.
2. Comparar cantidades.
3. Identificar diferencias.

Detecta:
- Diferencias de stock
- Productos faltantes
- Posibles errores de registro
- Riesgos operativos

Devuelve:
- Tabla comparativa:
  id_producto | nombre_producto | stock_sistema | cantidad_detectada | diferencia

- Lista de inconsistencias clara y basada en datos.
```

2. Analiza la respuesta:
- ¿Las diferencias son coherentes?
- ¿Se detectan faltantes o excedentes?
- ¿La IA evitó inventar datos?

### Parte 5. Generación de reporte de inventario
En esta etapa transformarás el análisis en un reporte ejecutivo.

1. Utiliza el siguiente prompt:

```text
Actúa como responsable de control de activos.

Genera un informe con:

1. Estado general del inventario
2. Diferencias detectadas
3. Productos con incidencias
4. Riesgos operativos
5. Recomendaciones para control y mejora

Incluye indicadores como:
- % exactitud inventario físico vs sistema
- % productos con incidencias
- Diferencia promedio de stock
- Nivel de riesgo operativo

Formato ejecutivo, claro y accionable.
```

2. Analiza la respuesta:
- ¿El reporte es claro y útil?
- ¿Los KPIs son relevantes?
- ¿Las recomendaciones son aplicables?

### Reflexión
-  ¿Qué valor aporta digitalizar información a partir de imágenes frente a capturar datos manualmente?
-  ¿Qué desafíos identificas al extraer datos desde medios físicos (calidad de imagen, escritura manual, ambigüedad)?
- ¿Qué riesgos existen si los datos extraídos no son precisos?

### Resultado esperado
Al finalizar la práctica, el participante será capaz de:
-  Utilizar herramientas de IA multimodal para analizar imágenes de inventario.
- Extraer información relevante y convertirla en datos estructurados.
- Integrar datos visuales con información estructurada mediante cruces analíticos.