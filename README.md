# 🫀 Modelo Predictivo de Riesgo Cardiovascular

Este proyecto implementa un modelo de regresión logística para predecir el riesgo de un evento cardiovascular a 10 años, utilizando variables clínicas del estudio Framingham. Fue desarrollado como parte de un máster en Inteligencia Artificial Aplicada a la Salud.

---

## 📊 Dataset
- **Fuente:** Estudio Framingham (base pública)
- **Variables utilizadas:**
  - Edad, sexo, presión sistólica/diastólica, colesterol total, tabaquismo, diabetes, etc.
  - `TenYearCHD`: Evento cardiovascular en 10 años (variable objetivo binaria)

---

## 🛠️ Metodología

1. **Preprocesamiento:**
   - Imputación de valores faltantes (mediana/moda)
   - Normalización de variables clínicas
   - División de datos en entrenamiento (70%) y prueba (30%)

2. **Modelado:**
   - Regresión logística con `class_weight='balanced'` para manejar desbalance de clases
   - Evaluación con AUC-ROC, matriz de confusión, sensibilidad y precisión

3. **Visualización:**
   - Curva ROC
   - Coeficientes del modelo interpretados clínicamente

---

## 📈 Resultados

- **AUC-ROC:** 0.70
- **Mejora de sensibilidad** (recall) en pacientes con riesgo cardiovascular al aplicar balance de clases
- El modelo identifica correctamente a más del 60% de los pacientes con riesgo, siendo útil en contextos de salud preventiva

---

## ▶️ Cómo reproducir

1. Clona el repositorio o descarga los archivos
2. Asegúrate de tener Python 3 y las siguientes librerías instaladas:
   - `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`
3. Ejecuta el notebook `Modelo_Riesgo_Cardiovascular.ipynb`

```bash
pip install -r requirements.txt  # si agregas dependencias en el futuro
```

---

## 📌 Autor

Camila Pallalever  
📍 Concepción, Chile  
🔗 [LinkedIn] https://www.linkedin.com/in/camila-pallalever-mella-832b6810a/

---

**Nota:** Este proyecto fue realizado con fines académicos y de aprendizaje. No debe ser usado para toma de decisiones clínicas sin validación externa.
