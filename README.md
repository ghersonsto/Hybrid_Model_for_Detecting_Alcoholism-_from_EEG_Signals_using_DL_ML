# 🧠 Hybrid Model for Detecting Alcoholism from EEG Signals Using Deep Learning and Machine Learning 🤖
### *Deep Learning & Machine Learning Integration for Clinical Diagnosis*

Este repositorio alberga el desarrollo de un **modelo híbrido** de inteligencia artificial para la detección objetiva del alcoholismo mediante señales de **electroencefalografía (EEG)**. El proyecto fue desarrollado bajo la modalidad de **artículo científico** para optar por el título profesional de **Ingeniero de Software**.

---

## 🚀 Performance Destacado (Benchmark Final)
Tras un riguroso proceso de experimentación con 6 arquitecturas de Deep Learning y 3 clasificadores, la combinación **Vision Transformer (ViT) + Support Vector Machine (SVM)** se consolidó como la solución óptima.

| Métrica | Resultado | Significado Clínico |
| :--- | :--- | :--- |
| **Exactitud (Accuracy)** | **98.38%** | Alta fiabilidad en el diagnóstico general. |
| **Sensibilidad (Recall)** | **100%** | **Cero falsos negativos:** No se omite ningún paciente enfermo. |
| **F1-Score** | **98.43%** | Equilibrio perfecto entre precisión y sensibilidad. |
| **AUC-ROC** | **0.9996** | Capacidad de discriminación casi perfecta. |



---

## 🛠️ Arquitectura del Sistema
El modelo utiliza un enfoque de **Feature Extraction** donde la red neuronal extrae la esencia de la señal y el clasificador tradicional toma la decisión final.

1.  **Procesamiento Wavelet (CWT):** Las señales crudas de **Kaggle (UCI)** se transforman en escalogramas (imágenes 2D de tiempo-frecuencia) de 224x224 píxeles.
2.  **Extractor de Características:** Se utiliza un **Vision Transformer (ViT)** que emplea mecanismos de auto-atención para capturar dependencias globales en la señal cerebral.
3.  **Clasificador Robusto:** Un **SVM** con optimización de hiperparámetros para definir el hiperplano óptimo de separación entre clases (Alcohólico vs. Control).



---

## 📂 Organización del Repositorio
Para facilitar la replicabilidad y el despliegue, el proyecto se estructura de la siguiente manera:

* `📁 notebooks/`: Flujo completo desde la limpieza de datos hasta el entrenamiento (CWT, Normalización, Training).
* `📁 src/`: Implementación modular de las arquitecturas (ViT, CNN, MobileNetV2, BotNet).
* `📁 models/`: Pesos entrenados y serialización del modelo ganador para inferencia inmediata.
* `📁 docs/`: Documentación técnica, artículo científico y presentación de tesis.*
* `📁 results/`: Resultados, Matrices de confusion y Curva ROC.

---

## 🔧 Stack Tecnológico
* **Lenguaje:** Python 3.x
* **Deep Learning:** TensorFlow / Keras
* **Machine Learning:** Scikit-Learn
* **Procesamiento de Señales:** PyWavelets / NumPy
* **Visualización:** Matplotlib / Seaborn

---

## 👤 Autor y Créditos
**Investigador:** Gherson Steven Torres Otrera  
**Asesor:** Mg. Ing. Wilfredo Mamani Ticona  
**Institución:** Universidad Tecnológica del Perú (UTP)

---
> *Este proyecto demuestra cómo la ingeniería de software y la inteligencia artificial pueden proporcionar herramientas diagnósticas no invasivas, precisas y de bajo costo para la salud pública.*
