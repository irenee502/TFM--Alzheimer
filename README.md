# TFM--Alzheimer
Master´s thesis 🧠 TFM - Detección Temprana de Deterioro Cognitivo Leve mediante Inteligencia Artificial

Este repositorio contiene todo el código, scripts y documentación utilizados en el Trabajo de Fin de Máster (TFM), cuyo objetivo es desarrollar un sistema de diagnóstico temprano del **Deterioro Cognitivo Leve (DCL)** mediante modelos de **Machine Learning** y **Deep Learning** aplicados a datos clínicos, neuropsicológicos y de neuroimagen funcional (fMRI).

La base de datos utilizada es:   Dallas LifeSpan BrainStudy" disponible en la plataforma OpenNeuro      https://openneuro.org/datasets/ds004856/versions/1.0.0

A continuación se describe brevemente el contenido de cada uno de los archivos y carpetas del repositorio:

1. `Descarga_DATABASE_TFM.ipynb`

Notebook inicial que permite al usuario descargar los datos necesarios para ejecutar el resto del pipeline. Incluye rutas, estructuras y comprobación básica de integridad de los archivos descargados.

---

2. `EDA_ML_TFM.ipynb` (Exploratory Data Analysis -MACHINE LEARNING )

Este notebook contiene un análisis exploratorio de los datos clínicos y neuropsicológicos. Se incluyen visualizaciones de distribuciones, análisis de correlaciones, detección de valores atípicos y primeras inferencias útiles para orientar los modelos de ML.

---

3.`EDA_DL_TFM.ipynb` (Exploratory Data Analysis -DEEP LEARNING )

Este notebook contiene un análisis exploratorio de las imágenes RMI, fRMI, PET. Incluye histogramas de intensidad, inspección de regiones cerebrales activadas, visualización de ejemplos concretos y comprobación del equilibrio de clases y calidad de las muestras funcionales.


---
4. `Prep_DL_TFM.ipynb`

Notebook dedicado al preprocesamiento de los datos funcionales (fMRI) que se utilizarán en Deep Learning. Se realizan tareas como normalización, segmentación, filtrado por tipo de tarea (por ejemplo, VentralVisual), y construcción de datasets personalizados para PyTorch.


---
5.`ML_TFM.ipynb` (MACHINE LEARNING)

Aquí se implementan y comparan diferentes algoritmos de Machine Learning (Random Forest, Gradient Boosting, SVM, etc.) aplicados a los datos tabulares. Incluye selección de características, evaluación de métricas como AUROC y precisión, así como validación cruzada.


---
6. `DL_TFM.ipynb`

Entrenamiento de modelos de Deep Learning con arquitecturas CNN, RNN y Transformers. Se exploran distintas configuraciones de hiperparámetros (dropout, learning rate, regularización, etc.), técnicas de optimización (Adam, ReduceLROnPlateau) y estrategias de mejora como autocast y batch normalization. También se evalúan modelos preentrenados mediante Transfer Learning.


---

7. `Ensamblado_TFM.ipynb`

Este script combina los modelos entrenados (tanto de ML como de DL) mediante técnicas de ensemble: soft averaging, hard voting y stacking. Se comparan los resultados y se selecciona la mejor combinación basada en métricas como AUROC, accuracy y recall.

---

8. `Interpretabilidad_TFM.ipynb`

Notebook dedicado a la interpretación de los modelos de Deep Learning mediante técnicas como Grad-CAM, Occlusion Sensitivity, LIME y SHAP. Se analizan visualmente las zonas cerebrales que más influyen en las decisiones del modelo y se comparan con el conocimiento clínico existente.

---

Documentación adicional

* `TFM.pdf`: Documento oficial del Trabajo de Fin de Máster en formato pdf, con resultados, figuras, interpretaciones y bibliografía.
* `README.md`: Este archivo, que explica la estructura y propósito del repositorio.


---

Contribuciones y contacto

Este proyecto ha sido desarrollado como parte del TFM del Máster en Inteligencia Artificial. Para más información o colaboración, puedes contactar al autor a través de aquí.

