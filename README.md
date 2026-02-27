# 📞 Challenge TelecomX - Análisis de Deserción (Churn)

### **📖 Descripción**
**Telecom X Latam** enfrenta una tasa de deserción significativa. Este proyecto, desarrollado en el marco del **Challenge de Data Science de Alura**, aborda el problema mediante un flujo de ingeniería de datos y un análisis exploratorio exhaustivo sobre una base de **7,032 clientes**.

---

## 🎯 Objetivos Estratégicos
* **Detectar causas:** Identificar los factores clave que impulsan la deserción.
* **Cuantificar impacto:** Medir el peso de cada variable en la tasa de abandono.
* **Proponer soluciones:** Definir recomendaciones estratégicas fundamentadas en datos.

---

## 📊 Principales Hallazgos (Insights)

### **📈 Métrica Global**
* **Tasa de Deserción:** **25.7%** de la base total de clientes muestra una clara intención de abandono.

### **⏰ El Factor Tiempo (Momento Crítico)**
* **Punto de Quiebre:** La densidad de abandono es máxima en los **primeros meses** de contrato. Superar el primer semestre incrementa drásticamente la lealtad.

### 👤 Perfil de Alto Riesgo
| Factor de Riesgo | Tasa de Deserción / Impacto |
| :--- | :--- |
| **Contrato Mensual** | **42.7%** de deserción |
| **Uso de Fibra Óptica** | **41.9%** de deserción |
| **Adultos Mayores** | **41.7%** de deserción |
| **Pago con Cheque Electrónico** | **45.3%** de deserción |
| **Sin Soporte Técnico** | Riesgo **2.7 veces mayor** |

### 💰 Impacto Financiero
* **Clientes Premium en Riesgo:** La fuga afecta desproporcionadamente a clientes con cargos mensuales elevados.
* **Comparativa de Cargos:** La mediana de pago de los desertores es de **$80**, mientras que la de los clientes leales es de **$63**.
* **Riesgo de Ingresos:** El abandono temprano de clientes con facturas altas representa la mayor amenaza financiera.
---

## 📁 Estructura del Proyecto
```text
Challenge-TelecomX-Alura-One-DS/
│
├── /imgs/                      # Capturas de pantalla y gráficos de Churn.
├── TelecomX_ETL.ipynb          # Notebook principal con ETL y EDA.
├── TelecomX_Data_Cleaned.csv   # Dataset final procesado.
└── README.md                   # Documentación técnica.

## 📋 Descripción de archivos principales 

### 📄 TelecomX_LATAM.ipynb
Análisis de Extremo a Extremo: Es el núcleo técnico del proyecto. Incluye todo el flujo de trabajo: desde la carga y desanidación de archivos JSON complejos, hasta la limpieza profunda de datos y la generación de los hallazgos estratégicos de negocio.

### 📂 data/
Gestión de Datos: Carpeta que aloja el dataset original de la compañía. Se documenta un proceso de transformación donde se inicia con 7,267 registros y, tras la limpieza de valores nulos y normalización, se obtienen 7,032 registros limpios listos para el análisis estadístico.

### 📂 Gráficos/
Evidencia Visual: Repositorio de las gráficas generadas (utilizando Seaborn y Matplotlib). Estas visualizaciones sirven como soporte para validar los puntos críticos de deserción, como el impacto del contrato mensual y la antigüedad del cliente.

### 📄 requirements.txt
Reproducibilidad Técnica: Archivo que especifica las librerías necesarias para ejecutar el proyecto. Garantiza que cualquier colaborador pueda recrear el entorno de análisis con las versiones exactas de las herramientas utilizadas.

## 🖼️ Ejemplos de Visualización

### ### **1. Distribución Global de Evasión**
**Estado actual:** Visualización de la proporción de clientes que permanecen vs. los que se van.
![Churn Global](churn_global.png)

---

### ### **2. Análisis de Contratos y Pagos**
**Segmentos críticos:** Se evidencia que el contrato mensual es el principal motor de fuga.
![Análisis de Contratos](analisis_contratos.png)

---

### ### **3. Permanencia y Cargos Mensuales**
**Impacto económico:** Gráficos de densidad que muestran el riesgo en clientes nuevos y de alta facturación.
![Distribución de Gastos](distribucion_gastos.png)

---

## 📌 Conclusión Clave
> **La deserción no es aleatoria:** Responde a patrones claros de experiencia temprana y tipo de contrato. Resolver el problema requiere un enfoque preventivo en los primeros 6 meses de vida del cliente.


## 🚀 Cómo ejecutar el proyecto

### **📍 Opción 1: Google Colab (Recomendado — No requiere instalación)**

Esta es la forma más rápida y sencilla de visualizar el análisis completo, el proceso de **ETL** y las gráficas interactivas sin necesidad de configurar un entorno local en tu computadora.

#### **1. Acceso directo**
Haz clic en el siguiente botón para abrir el proyecto directamente en la nube:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/18ubUeVDWU3q-xufZlcwcUsfqjFJrDEUf#scrollTo=mZj6Po-1JIpG)

#### **2. Ejecución**
Una vez que el notebook cargue en tu navegador, sigue estos pasos:
* Ve al menú superior y selecciona **Entorno de ejecución** (Runtime).
* Haz clic en **Ejecutar todo** (Run all).
* *Alternativa rápida:* Presiona `Ctrl + F9`.

#### **3. Resultados**
El sistema realizará automáticamente las siguientes tareas:
* 📥 **Carga y desanidación** del dataset original en formato JSON.
* 🧹 **Limpieza y transformación (ETL)** de las 7,032 filas de datos.
* 📊 **Generación de visualizaciones** de Churn, correlaciones y perfiles de riesgo.

---

### **✨ Ventajas de esta opción**
* **✅ Sin instalaciones:** No necesitas Python ni librerías en tu PC.
* **✅ Multiplataforma:** Funciona desde cualquier dispositivo con navegador.
* **✅ Procesamiento gratuito:** Utiliza los recursos de Google para ejecutar el análisis al instante.


### **📦 Dependencias principales**

Para asegurar la reproducibilidad del análisis, se requieren las siguientes librerías:

| Librería | Versión | Función |
| :--- | :--- | :--- |
| **Pandas** | `2.0.3` | Manipulación y limpieza de datos (ETL) |
| **NumPy** | `1.24.3` | Operaciones numéricas y vectores |
| **Matplotlib** | `3.7.2` | Generación de gráficos base |
| **Seaborn** | `0.12.2` | Visualizaciones estadísticas avanzadas |
| **SciPy** | `1.11.0` | Pruebas de correlación y estadística |
| **Requests** | `2.31.0` | Consumo de datos desde fuentes externas |

#### **💻 Instalación manual de dependencias:**
```bash
pip install pandas numpy matplotlib seaborn jupyter requests chardet scipy


## 🔧 Solución de problemas comunes

* **❌ Problema:** `ModuleNotFoundError: No module named 'pandas'`  
  **✅ Solución:** Ejecuta `pip install pandas numpy matplotlib seaborn`

* **❌ Problema:** `Jupyter no se inicia`  
  **✅ Solución:** Verifica que el entorno virtual esté activado y ejecuta `pip install jupyter`

* **❌ Problema:** `Error al cargar el dataset`  
  **✅ Solución:** Verifica que el archivo `data/TelecomX_Data.json` exista en la ruta correcta.

* **❌ Problema:** `Error con scipy.stats`  
  **✅ Solución:** Instala la versión específica con `pip install scipy==1.11.0`

---

## 🚀 Tecnologías utilizadas

* 🐍 **Python 3.8+** – Lenguaje principal de análisis.
* 📊 **Pandas** – Manipulación y análisis de datos estructurados.
* 📈 **Matplotlib / Seaborn** – Visualización de datos y gráficos estadísticos.
* 🔢 **NumPy** – Operaciones numéricas y estadísticas.
* 📓 **Jupyter Notebook** – Desarrollo interactivo del análisis.
* ☁️ **Google Colab** – Ejecución en la nube sin instalación local.
* 💻 **Visual Studio Code** – Desarrollo y edición de código.
* 🌐 **Git / GitHub** – Control de versiones y colaboración.
* 📡 **Requests** – Obtención de datos desde APIs.
* 🔍 **Chardet** – Detección de codificación de archivos.
* 📊 **Scipy** – Análisis estadístico avanzado (correlación point-biserial).

---

## 💡 Recomendaciones estratégicas

### **🚀 Acciones de corto plazo (operativas)**
* **Programa de onboarding intensivo:** Acompañamiento en los primeros 90 días para mitigar el riesgo de deserción temprano.
* **Seguimiento proactivo:** Atención especializada a los segmentos más vulnerables: clientes de **Fibra Óptica** y adultos mayores.
* **Incentivos de contrato:** Implementar descuentos del **15-20%** para incentivar la migración de contrato mensual a anual.
* **Métodos de pago:** Promover la transición desde el **Cheque Electrónico** hacia métodos de pago automáticos.

### **🎯 Acciones de retención (mediano plazo)**
* **Sistema de alertas tempranas:** Implementar monitoreo automático para identificar clientes con antigüedad menor a 6 meses y cargos superiores a **$70**.
* **Programa personalizado:** Ofrecer upgrades gratuitos y atención mediante un ejecutivo dedicado para perfiles de alto valor.

## ✍️ Créditos y Autoría

Este proyecto fue desarrollado como parte del **Challenge Data Science** de **Alura Latam** en colaboración con el programa **Oracle Next Education (ONE)**.

**Desarrollado por:**
### **✨ [Idabel Coparropa]**
*Data Scientist Enthusiast*

---

### **📚 Agradecimientos**
* A **Alura Latam** y **Oracle** por los retos técnicos que impulsan el crecimiento profesional.
* A la comunidad de **Data Science** por las herramientas de código abierto que hicieron posible este análisis.

---
