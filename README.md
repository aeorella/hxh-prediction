# 📖 Hunter × Hunter — Predicción del regreso del manga

Este proyecto usa **modelos de Machine Learning** y análisis temporal para estimar la probabilidad de regreso del manga *Hunter × Hunter* en la revista *Weekly Shōnen Jump*.

## 🔍 Descripción

Desde 1998, *Hunter × Hunter* ha tenido múltiples pausas ("hiatus").  
El objetivo de este análisis es **predecir las semanas más probables de regreso futuro**,  
usando datos históricos de publicación y diferentes modelos de predicción.

## 🧠 Modelos utilizados

- **Hazard Model (Regresión logística temporal)** → Probabilidad base de regreso semanal.  
- **XGBoost** → Captura patrones no lineales, estacionales y de publicación.  
- **Modelo Final (Meta / Ensamble)** → Combina Hazard + XGBoost + estacionalidad.  
- (Opcional) **Simulación Monte Carlo** → Estimaciones estocásticas de futuros posibles.

## 📈 Resultados principales

- El modelo identifica patrones estacionales de publicación y hiatus prolongados.
- Las proyecciones trimestrales muestran alta probabilidad de regreso en los últimos trimestres de cada año.
- Predicciones generadas para 2025–2035 con probabilidad media y superior al 40% en octubre.

## 📊 Archivos incluidos

| Archivo | Descripción |
|:--|:--|
| `Prediccion_HxH_Modelos_Ensamble.ipynb` | Notebook completo con código, análisis y visualizaciones. |
| `predicciónregresohxh.py` | Script modular del modelo final. |
| `tabla_trimestral_modelos_promedio.csv` | Resumen trimestral de probabilidades 2025–2030. |
| `regresomanga.py` | Versiones previas de experimentos y modelos base. |

## 🧩 Librerías utilizadas

- Python 3.12  
- Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib  
- Opcional: TensorFlow (para prototipos de redes neuronales)

## 🚀 Autor

**Alejandro Emilio Orellana Urrea**  
[GitHub @aeorella](https://github.com/aeorella)  
Proyecto personal de portafolio — Ciencia de Datos aplicada a análisis cultural y predictivo.

---

