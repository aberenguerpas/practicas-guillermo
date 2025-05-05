### Prácticas Guillermo

## **Contexto del Proyecto**

Acceder a la información sobre contratos públicos en España es, hoy en día, una tarea complicada, sobre todo para personas sin experiencia. El principal problema es que las herramientas actuales, como el[portal de contrataciones del estado](https://contrataciondelestado.es/wps/portal/!ut/p/b1/04_SjzSyMDAzsDAwt9CP0I_KSyzLTE8syczPS8wB8aPM4k1c_Z2d3TyMDCyCjV0MjHxcQkPNPIBcd1OggkigAlNjZ5Mwr7AAs2BPdwMDTw83F59QQ1MDdyMz4vQb4ACOBoT0h-tH4VdiBFWAz4lgBXjc4OeRn5uqnxuV42bpmWUCAKOwtvs!/dl4/d5/L2dBISEvZ0FBIS9nQSEh/pw/Z7_AVEQAI930OBRD02JPMTPG21004/act/id=0/p=javax.servlet.include.path_info=QCPjspQCPbusquedaQCPMainBusqueda.jsp/607687264348/-/), no están pensadas para facilitar la búsqueda a usuarios nuevos.

Por ejemplo, no se puede buscar fácilmente usando palabras clave como en Google. En lugar de eso, hay que usar códigos técnicos o identificadores, lo que resulta poco intuitivo y muy tedioso.

Para solucionar esto, queremos desarrollar una herramienta que permita buscar contratos públicos por palabras clave como “obras”, “reparación de cableado” o “desarrollo web”. Así, el usuario recibiría resultados que realmente se ajusten a lo que busca.

El problema es que la información más útil para este tipo de búsquedas no está en los metadatos, sino dentro de los documentos PDF que acompañan a cada contrato. En concreto, hay dos documentos importantes:

- Pliego técnico: Describe en detalle el trabajo que hay que hacer.
- Pliego administrativo: Explica las reglas legales y económicas del contrato.

Para poder usar esta información en nuestra herramienta, necesitamos leer y extraer ciertos datos clave de esos PDFs. Esa es una parte central de este proyecto.

##### Qué información hay que extraer de los PDFs?

* Del pliego técnico:
  * Resumen del contrato: Un texto de entre 100 y 200 palabras que explique claramente cuál es el trabajo que se va a hacer.
  * Requisitos técnicos: Normas de calidad, certificaciones necesarias, características técnicas, metodologías, materiales a usar, etc. En caso de servicios: qué perfiles profesionales se necesitan, cómo debe realizarse el trabajo, entregables y plazos.

- Del pliego administrativo:
  - Solvencia técnica y económica: Es decir, los requisitos mínimos que debe cumplir una empresa para poder presentarse (por ejemplo, experiencia previa, facturación mínima, número de empleados, etc.).
  - Criterios de adjudicación: Qué aspectos se tendrán en cuenta para decidir qué empresa gana el contrato (precio, calidad técnica de la propuesta, mejoras ofrecidas, etc.).

## Objetivos de la práctica

A partir del contexto anterior, estas prácticas tienen como objetivo introducirte en un problema real relacionado con la extracción de información de documentos públicos. Los pasos que seguirás son los siguientes:

* **Entender bien el problema:** Comprender por qué es difícil buscar contratos públicos y qué papel juegan los documentos PDF (pliegos) en este problema.
* **Investigar posibles soluciones**: Buscar ideas y métodos que se puedan usar para leer y extraer datos automáticamente de estos PDFs.
* **Proponer herramientas o modelos de inteligencia artificial (IA):** Pensar qué técnicas o modelos de IA podrían ayudar a identificar y extraer la información relevante.
* **Evaluar las propuestas:** Evaluación de esas propuestas en cuanto a tiempo, efectividad y coste.
* **Aplicación de técnicas RAG:** Usar técnicas de búsqueda y recuperación de información ( *Retrieval-Augmented Generation* ) para trabajar con los datos extraídos, de forma que puedan usarse en sistemas como chatbots o buscadores inteligentes.
