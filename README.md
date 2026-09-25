Markdown
# 🏭 Automatización de POEs con IA bajo Normativa ISO 9001

## 🎯 Objetivo del Proyecto
Desarrollar una Prueba de Concepto (POC) en Python y Jupyter Notebook para transformar notas informales de planta, audios transcritos o descripciones desestructuradas en **Procedimientos Operativos Estándar (POE)** formales, profesionales y estructurados bajo los lineamientos de la norma **ISO 9001**.

## 🛠️ Stack Tecnológico y Herramientas
* **Lenguaje:** Python
* **Entorno:** Jupyter Notebook / Google Colab
* **Modelo de IA:** Groq API (`openai/gpt-oss-120b`)
* **Librerías principales:** `groq`, `requests`

## ⚙️ Diseño del Prompt Maestro
El sistema implementa una estrategia de estructuración basada en roles (*Role Prompting*), asignando a la IA la perspectiva de un **Ingeniero Industrial Senior experto en gestión de calidad**. 

El prompt fuerza al modelo a entregar un formato estricto en Markdown que incluye:
1. **Encabezado del Procedimiento:** Código alfanumérico, título y área/departamento.
2. **Objetivo y Alcance:** Propósito claro del proceso y sector de aplicación.
3. **Responsables:** Roles involucrados en la ejecución.
4. **Paso a Paso Operativo:** Instrucciones secuenciales detalladas.
5. **Criterios de Control y Calidad:** Puntos críticos de control.

## 🚀 Guía de Instalación y Uso
1. Clona este repositorio o descarga el archivo `.ipynb`.
2. Instala la librería oficial de Groq en tu entorno:
   ```bash
   pip install groq
