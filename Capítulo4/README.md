# Práctica 4. Creación de un agente

## Objetivo de la práctica
Al finalizar la práctica, serás capaz de:
- Diseñar un agente conversacional básico en Copilot Studio, desde la definición del propósito hasta las pruebas iniciales.


## Tabla de ayuda
Para que puedas replicar las prácticas, se recomienda crear una cuenta **gratuita** con tu **cuenta empresarial** en la siguiente plataforma.

| Sitio web | Enlace |
| --- | --- | 
| Copilot Studio | https://www.microsoft.com/es-es/microsoft-copilot/microsoft-copilot-studio | 

## Duración aproximada
- 60 minutos.

## Instrucciones 
Sigue los pasos a continuación para completar cada tarea que conforma la práctica.

### Tarea 1. Crear un agente usando plantillas preconstruidas en Copilot Studio
Ingresa a Copilot Studio para desarrollar la práctica e inicia sesión con tu cuenta empresarial.

**Paso 1.** Explora agentes a partir de plantillas.
- En la página _Inicio_, selecciona _Crear_ y explora los agentes de la sección _Empezar con una plantilla de agente_.
- Selecciona una plantilla de agente que se ajuste a tu caso, por ejemplo _Viajes seguros_.

  <img width="1067" height="569" alt="P4_T1_1" src="https://github.com/user-attachments/assets/80d92a14-9a8a-4fc1-9166-d163a16a5e7a" />

**Paso 2.** Personaliza el agente.
- Revisa y explora la documentación de la plantilla _Viajes seguros_.
- Cambia el _Nombre del agente_, _Descripción_, _Instrucciones_ e _Icono del agente_:

| Elemento | Original | Personalizado |
| --- | --- | --- |
| Nombre del agente | Viajes seguros | Asistente de viajes corporativos |
| Descripción | Ayuda a los usuarios a planificar viajes seguros. | Brinda recomendaciones de viaje, políticas de empresa y asistencia en tiempo real para empleados que viajan por trabajo. |
| Instrucciones | Responde preguntas sobre viajes. | Usa un tono profesional y claro. Prioriza la seguridad, cumplimiento de políticas y eficiencia. |
| Icono | <img width="58" height="57" alt="P4_T1_2" src="https://github.com/user-attachments/assets/002a5427-97c4-4249-b097-1f7d1cf56e4d" /> | <img width="60" height="60" alt="travel-bag" src="https://github.com/user-attachments/assets/1d65f748-9c15-4076-90ca-1081ae6f7bdc" /> |

- Dirígete a la sección de _Conocimiento_ y visita _Sitio web de viajes de EE.UU._
- Da clic en _Crear_.

<img width="908" height="568" alt="P4_T1_3" src="https://github.com/user-attachments/assets/d0d5e640-5d92-4fc6-adc3-da64268dc6b0" />

**Paso 2.** Probar el _Agente_.
- Da clic en _Probar_ <img width="68" height="52" alt="P4_T1_4" src="https://github.com/user-attachments/assets/e136086f-9338-40a9-8d5d-27c399060aac" />
 (sección superior derecha) y empieza a interactuar con el agente. Verifica y comprueba la veracidad de las respuestas.
```
How can I get a U.S. passport?
```
- Envía el prompt y comprueba la veracidad de la respuesta.

```
What should I do if I lose my passport during an international trip?
```
- Envía el prompt y comprueba la veracidad de la respuesta.

```
What are the travel recommendations for China?
```
- Envía el prompt y comprueba la veracidad de la respuesta.

- ¿Qué respuesta obtendrías si haces una pregunta que no se relaciona con el contenido de la página web ni con las instrucciones del _Agente_?

```
What's the name of the last book you read?
```
- Envía el prompt y verifica la respuesta.

```
How much does a train ticket cost from Paris to Rome?
```
- Envía el prompt y verifica la respuesta.
- ¿A partir de qué información generó esa respuesta? 


**Paso 3.** Modificar parámetros.

**Búsqueda web**

- En la pestaña _Información general_, dirígete a la sección _Conocimientos_ y habilita la _Búsqueda web_
    <img width="108" height="34" alt="P4_T1_5" src="https://github.com/user-attachments/assets/7a7122d9-838b-4d16-b4b7-6ed05c645a16" />
- Para probar el _Agente_ con los cambios aplicados, da clic en el botón de _Refresh_ que se encuentra en la sección superior derecha, debajo del botón de _Probar_ <img width="86" height="85" alt="P4_T1_6" src="https://github.com/user-attachments/assets/34083041-cc80-4511-90b8-eddeb58c8793" />

- Ingresa el siguiente prompt en la sección del chat.
```
What are the best local dishes to try in Thailand?
```
- Envía el prompt y verifica la respuesta.
- ¿De dónde se extrajo la información para generar la respuesta?

##### Temas
- En la pestaña _Información general_, dirígete a la sección _Temas_ y da clic en _Ver todo_. Explora los distintos temas.
- Da clic en Agregar un tema y seleccionar "Agregar a partir de una descripción con Copilot" 
- Ingresa la siguiente información.
  - Asigna un nombre al tema: _Requisitos de vacunación_.
  - Crea un tema para: _Informar sobre vacunas obligatorias o recomendadas para viajar a ciertos países_.
  - Da clic en _Crear_.
  - La página te redirigirá a la definición del tema. Analiza el contenido y la estructura lógica.
  - Da clic en _Guardar_.
  - Da clic en _Refresh_ para probar los cambios en el _Agente_.
  - ¿Crees que Copilot sea capaz de comprender el contenido de ese _Tema_ aunque no se encuentre en el mismo idioma que definimos para el _Agente_?
  - Ingresa el siguiente prompt.
    ```
    Do I need vaccines to travel to India?
    ```
  - Envía el prompt y verifica la respuesta.
- Da clic en el botón _Atrás_ para añadir nuevos _Temas_.
- Repite el proceso con la siguiente información.
  - Asigna un nombre al tema: _Currency exchange_.
  - Crea un tema para: _Provide information on exchange rates, where to exchange money, and tips_.
  - Da clic en _Crear_
  - Asigna un nombre al tema: _Customs and etiquette_.
  - Crea un tema para: _Inform about cultural norms, greetings, dress, and behavior_.
  - Da clic en _Crear_.
- Ingresa los siguientes prompts.
    ```
    Where can I exchange dollars in Japan?
    ```

    ```
    What customs should I respect in Saudi Arabia?
    ```
- Modifica la sección [country] acorde al país de tu preferencia.
  
    ```
    What is the current exchange rate in [country]?
    ```

    ```
    What clothing is appropriate for visiting temples in [country]?
    ```

- Envía los prompts y verifica las respuestas.

#### Resultado esperado
Al explorar los resultados generados con Copilot y ChatGPT, se obtendrán resultados similares a los siguientes.

<img width="437" height="616" alt="P4_T1_7 (1)" src="https://github.com/user-attachments/assets/e9178840-0513-4882-8ae7-af1b8dc540b4" />

<img width="446" height="635" alt="P4_T1_7 (2)" src="https://github.com/user-attachments/assets/3e593126-69c2-48eb-9c51-9d2c9d1df876" />

<img width="415" height="405" alt="P4_T1_7 (3)" src="https://github.com/user-attachments/assets/06b8801b-d679-47f9-bb01-4aa3083822e7" />

<img width="624" height="654" alt="P4_T1_7 (4)" src="https://github.com/user-attachments/assets/4050e8d2-9aea-41be-b830-ef3db2807696" />

