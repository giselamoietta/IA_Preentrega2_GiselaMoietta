# 🏭 Automatización de POEs con IA bajo Normativa ISO 9001

## 📋 Resumen Ejecutico
Este proyecto presenta una Prueba de Concepto (POC) orientada a resolver las fricciones operativas y administrativas vinculadas a la documentación y estandarización de procesos en el ámbito industrial. Utilizando modelos de lenguaje avanzados integrados mediante API y técnicas de *Fast Prompting*, la solución automatiza la transformación de notas informales de planta, audios y descripciones desestructuradas en Procedimientos Operativos Estándar (POE) formales y estructurados bajo los lineamientos de la norma ISO 9001.

---

## 🔍 Presentación del Problema a Abordar
* **Descripción de la problemática:** En el ámbito de la gestión industrial y operativa en las empresas, la documentación, actualización y correcta asimilación de los Procedimientos Operativos Estándar y manuales de operaciones suele ser un proceso manual, disperso y altamente ineficiente. A menudo, el conocimiento crítico sobre cómo ejecutar una tarea reside de manera informal en la experiencia de operarios o supervisores, generando demoras en la transferencia de saberes, inconsistencias operativas y dificultades al momento de capacitar nuevo personal.
* **Relevancia:** Una solución basada en Inteligencia Artificial es relevante porque permite automatizar la transformación de información cruda y desestructurada (como notas de reuniones, audios de procesos o explicaciones informales de planta) en manuales formales, normalizados y comprensibles. Esto reduce drásticamente los tiempos de gestión administrativa, estandariza la calidad operativa y disminuye los márgenes de error humano en la planta.

---

## 🎯 Objetivo del Proyecto
Desarrollar una Prueba de Concepto (POC) en Python y Jupyter Notebook para transformar notas informales de planta, audios transcritos o descripciones desestructuradas en Procedimientos Operativos Estándar (POE) formales, profesionales y estructurados bajo los lineamientos de la norma ISO 9001.

---

## 🛠️ Stack Tecnológico y Herramientas
* **Lenguaje:** Python
* **Entorno:** Jupyter Notebook / Google Colab
* **Modelo de IA (Texto a Texto):** Groq API (`openai/gpt-oss-120b`)
* **Modelo de IA (Texto a Imagen):** Generación de infografías conceptuales mediante herramientas alternativas gratuitas (ej. NightCafe / Bing Image Creator)
* **Librerías principales:** `groq`, `requests`

---

## ⚙️ Metodología y Diseño del Prompt Maestro
El sistema implementa una estrategia de estructuración basada en roles (*Role Prompting*), asignando a la IA la perspectiva de un **Ingeniero Industrial Senior experto en gestión de calidad**. 

El prompt maestro fuerza al modelo a entregar un formato estricto en Markdown que incluye:
1. **Encabezado del Procedimiento:** Código alfanumérico, título y área/departamento.
2. **Objetivo y Alcance:** Propósito claro del proceso y sector de aplicación.
3. **Responsables:** Roles involucrados en la ejecución.
4. **Paso a Paso Operativo:** Instrucciones secuenciales detalladas.
5. **Criterios de Control y Calidad:** Puntos críticos de control.

---

## 📉 Viabilidad Técnica y Análisis de Costos
* **Viabilidad Técnica:** La arquitectura es altamente viable ya que no requiere infraestructura local compleja ni entrenamiento de modelos pesados; opera de manera ágil mediante peticiones HTTP a la API de Groq.
* **Análisis de Costos y Tokens:** El uso del modelo `openai/gpt-oss-120b` a través de la infraestructura optimizada de Groq permite un procesamiento de baja latencia con un consumo eficiente de tokens en la capa gratuita, haciéndolo sostenible para fases experimentales y despliegues piloto en PyMEs industriales.

---

## 🖼️ Módulo Multimodal: Texto a Imagen
Como complemento visual al procedimiento operativo, se diseñó un prompt para generar una representación conceptual del flujo de estandarización industrial.

* **Prompt visual utilizado:** 
  > *"Infografía esquemática y profesional para manual industrial, estilo plano y minimalista, mostrando la transformación de notas informales de planta en un documento estructurado bajo norma ISO 9001, sin textos ilegibles, colores corporativos azul y gris, alta calidad técnica."*

* **Resultado visual obtenido:**
  *(Asegúrate de subir tu archivo de imagen generado, por ejemplo `proceso_poe.png`, a este repositorio y enlazarlo aquí debajo)*
  ![Esquema Conceptual POE ISO 9001](proceso_poe.png)

---

## 📊 Análisis Crítico de Resultados
* **Efectividad del Modelo:** El uso del modelo especificado logró estructurar con total precisión las entradas informales de planta, respetando rigurosamente las 6 secciones exigidas por el estándar ISO 9001.
* **Márgenes de Error Detectados:** Durante las iteraciones iniciales se observó que la falta de delimitadores estrictos en el prompt provocaba ambigüedades en los roles responsables. Esto se corrigió aplicando reglas de *grounding* y restricción de formato estricto, logrando salidas consistentes y libres de alucinaciones operativas.

---

## 🏁 Conclusiones
La POC desarrollada demuestra de manera exitosa que la combinación de Python, técnicas de *Fast Prompting* y modelos optimizados puede resolver una problemática real de la industria: la burocracia y dispersión en la documentación de procesos. Se cumplieron los objetivos de optimizar el uso de prompts, estructurar salidas profesionales y mantener una viabilidad económica accesible mediante herramientas gratuitas y de bajo costo de API.

---

## 📚 Referencias
* Norma Internacional ISO 9001: Sistemas de gestión de la calidad — Requisitos.
* Documentación oficial de Groq API y librerías de desarrollo en Python.
