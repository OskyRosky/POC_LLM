# POC_LLM

Cómo implementar un LLM local o en un servidor a través de Ollama.

Informe Detallado: Implementación de un Modelo LLM con OpenWeb UI y Alternativas de Ollama

## 1. Introducción al Proyecto

La División de Fiscalización Operativa y Evaluativa desarrolló una Prueba de Concepto (PoC) con el objetivo de evaluar la viabilidad de implementar un modelo de lenguaje (LLM) para asistir a los abogados de la Entidad de Fiscalización Superior. El proyecto se inscribe dentro de un marco de transformación digital, buscando optimizar el acceso a criterios legales y normativos mediante inteligencia artificial generativa.

##  2. Justificación Técnica y Metodológica

El equipo eligió un enfoque iterativo, comenzando con una investigación de los modelos existentes (SLM y LLM), para luego definir herramientas, entrenar el modelo, probarlo y desplegarlo. Se utilizó el modelo Llama3, cargado a través de Ollama, y se usó OpenWeb UI como la interfaz para interactuar con el modelo. La metodología siguió cinco pasos clave:

definir los objetivos técnicos,

seleccionar las herramientas adecuadas,

alimentar el modelo con criterios legales,

realizar pruebas continuas,

desplegarlo en un entorno visual e interactivo.

##  3. Resultados Principales

El modelo respondió adecuadamente a las consultas legales, ofreciendo respuestas rápidas y contextualizadas. Sin embargo, el equipo identificó que se requieren mejoras en dos frentes: la alimentación del modelo con información más estructurada y actualizada, y el fortalecimiento de la infraestructura computacional para soportar una futura versión en producción.

##  4. Plataforma OpenWeb UI: Ventajas y Alternativas

OpenWeb UI fue seleccionado por su facilidad de uso y compatibilidad con modelos cargados por Ollama. Sus principales ventajas son:

- Interfaz intuitiva basada en navegador,

- Personalización del modelo vía comandos simples (open-webui server),

- Integración directa con Ollama.

Sin embargo, existen otras interfaces o entornos visuales compatibles o similares, que pueden ser consideradas para escalar el proyecto:

LM Studio: interfaz gráfica para cargar y probar LLMs de manera local, ideal para pruebas rápidas.

Text Generation WebUI: altamente configurable, permite múltiples backends como Hugging Face, GPTQ o llama.cpp.

Chatbot UI: clon de ChatGPT de código abierto, ideal para proyectos de front-end integrados.

Langflow: interfaz visual tipo “node-based” para construir flujos LLM con herramientas como LangChain.

Flowise: alternativa ligera para construir aplicaciones LLM sin necesidad de programar.

LiteLLM Playground: interfaz simple pero efectiva que funciona con múltiples proveedores de LLM.

PrivateGPT Web UI: interfaz centrada en privacidad para el despliegue de modelos locales.

AutoGen Studio: diseñada para crear agentes LLM colaborativos, con interfaz integrada.

Dust: entorno de desarrollo que integra modelos abiertos y permite gestionar el historial de conversaciones.

BerriAI Playground: útil para prototipado de flujos de chat y pruebas de prompts con retroalimentación visual.

##  5. Modelos de Lenguaje en Ollama: 10 Opciones Recomendadas

Además de Llama3, Ollama permite cargar fácilmente modelos listos para usar o personalizados. A continuación, se presentan 10 modelos compatibles, junto con sus características destacadas:

Llama3
modelo de Meta. Muy balanceado en precisión, rapidez y adaptabilidad. Recomendado para tareas generales.

Mistral-7B
modelo liviano y rápido. Excelente para ambientes locales con menor capacidad de cómputo.

Gemma
modelo de Google. Altamente optimizado para tareas de lenguaje natural y generación coherente.

Neural Chat
modelo basado en Intel, ideal para asistentes conversacionales.

Phi-2
pequeño pero potente. Entrenado con enfoque en razonamiento matemático y comprensión semántica.

OpenChat
versión abierta similar a ChatGPT. Muy capaz en tareas de interacción natural.

Command R+
modelo de tipo instructivo con fuerte orientación a seguir órdenes precisas.

Deepseek-Coder
especializado en generación de código y tareas de programación.

Code LLaMA
ideal para desarrolladores. Entiende y genera múltiples lenguajes de programación.

Nous Hermes 2 Mistral
modelo de tipo instructivo con excelentes resultados en benchmarks de comprensión.

##  6. Próximos pasos

El equipo deberá avanzar hacia el uso de Retrieval-Augmented Generation (RAG) o métodos de tuning para mejorar la calidad de las respuestas. Asimismo, será necesario contar con infraestructura basada en la nube (como AWS, Azure o GCP) que permita escalar la solución sin depender de recursos locales limitados.

##  7. Conclusión

La PoC demostró que es factible construir un sistema tipo ChatGPT para apoyo legal, utilizando herramientas de código abierto como Llama3, Ollama y OpenWeb UI. Aún quedan tareas importantes por ejecutar: optimizar la alimentación del modelo, mejorar la calidad de las respuestas mediante técnicas más avanzadas y garantizar una infraestructura capaz de soportar la demanda real. Este proyecto sienta las bases para una transformación tecnológica profunda en los procesos institucionales.
