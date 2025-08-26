# 🧠 Machine Learning Tutorial for Beginners

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-green.svg)](https://scikit-learn.org)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Un tutorial completo de **Machine Learning** utilizando un dataset real de pacientes ortopédicos. Este proyecto cubre tanto **aprendizaje supervisado** como **no supervisado** con implementaciones prácticas en Python.

## 📊 Dataset

**Archivo:** `column_2C_weka.csv`
- **310 registros** de pacientes ortopédicos
- **6 características numéricas** relacionadas con medidas pélvicas y lumbares
- **Variable objetivo:** Clasificación binaria (Normal/Abnormal)

### 🔍 Variables del Dataset

| Variable | Descripción | Tipo |
|----------|-------------|------|
| `pelvic_incidence` | Incidencia pélvica | Float64 |
| `pelvic_tilt numeric` | Inclinación pélvica numérica | Float64 |
| `lumbar_lordosis_angle` | Ángulo de lordosis lumbar | Float64 |
| `sacral_slope` | Pendiente sacra | Float64 |
| `pelvic_radius` | Radio pélvico | Float64 |
| `degree_spondylolisthesis` | Grado de espondilolistesis | Float64 |
| `class` | Clase (Normal/Abnormal) | Object |

### 📈 Distribución de Clases

```
Abnormal: 210 casos (67.7%) ████████████████████
Normal:   100 casos (32.3%) ████████
```

## 🤖 Algoritmos Implementados

### 📚 Aprendizaje Supervisado

| Algoritmo | Accuracy/Score | Descripción |
|-----------|----------------|-------------|
| **K-Nearest Neighbors** | 88.17% | Clasificación basada en vecinos más cercanos |
| **Regresión Lineal** | R² = 0.646 | Modelo lineal para predicción continua |
| **Regresión Ridge** | Score: 0.561 | Regularización L2 para evitar overfitting |
| **Regresión Lasso** | Score: 0.964 | Regularización L1 con selección de características |
| **Random Forest** | 84% | Ensemble de árboles de decisión |
| **Regresión Logística** | - | Clasificación con curva ROC |

### 🔍 Aprendizaje No Supervisado

| Algoritmo | Descripción |
|-----------|-------------|
| **K-Means Clustering** | Agrupación en 2 clusters |
| **PCA** | Análisis de componentes principales |
| **T-SNE** | Visualización de datos en 2D |
| **Clustering Jerárquico** | Dendrogramas para análisis de clusters |

## 🛠️ Técnicas de Evaluación

- ✅ **Train-Test Split** (70%-30%)
- ✅ **Cross Validation** (5-fold)
- ✅ **Grid Search** para optimización de hiperparámetros
- ✅ **Matriz de Confusión**
- ✅ **Curva ROC** y métricas AUC
- ✅ **Métricas completas:** Accuracy, Precision, Recall, F1-score

## 🔧 Preprocesamiento

- **Estandarización** de datos numéricos
- **One-hot encoding** para variables categóricas
- **Pipeline** para automatizar procesos
- **Normalización** para algoritmos sensibles a escala

## 📋 Requisitos

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy
```

### Dependencias principales:
- `numpy` - Computación numérica
- `pandas` - Manipulación de datos
- `matplotlib` - Visualización básica
- `seaborn` - Visualización estadística
- `scikit-learn` - Algoritmos de ML
- `scipy` - Computación científica

## 🚀 Uso

1. **Clona el repositorio:**
   ```bash
   git clone https://github.com/IrvingMordo26/machine-learning-tutorial.git
   cd machine-learning-tutorial
   ```

2. **Instala las dependencias:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Abre el notebook:**
   ```bash
   jupyter notebook machine-learning-tutorial-for-beginners.ipynb
   ```

4. **Ejecuta las celdas** para reproducir todos los resultados

## 📊 Resultados Destacados

### 🏆 Mejores Resultados por Algoritmo:
- **🥇 Mejor Score General:** Lasso Regression (0.964)
- **🥈 Mejor Accuracy:** KNN con K=18 (88.17%)
- **🥉 Mejor Balance:** Random Forest (84% accuracy)

### 🔍 Características Más Importantes:
Según el análisis Lasso, las características más relevantes son:
1. `pelvic_incidence` (coeficiente: 0.825)
2. `pelvic_tilt numeric` (coeficiente: -0.721)

### 📈 Insights del Dataset:
- ✅ **Dataset balanceado** - No requiere técnicas especiales de balanceo
- ✅ **Sin valores faltantes** - Datos limpios y completos
- ✅ **Correlaciones moderadas** - Buenas para ML

## 📚 Conceptos Clave Aprendidos

### 🎯 Supervisado:
- Diferencia entre overfitting y underfitting
- Importancia de la validación cruzada
- Optimización de hiperparámetros
- Interpretación de métricas de evaluación

### 🔍 No Supervisado:
- Clustering y evaluación de clusters
- Reducción de dimensionalidad
- Visualización de datos multidimensionales

## 🎓 Preguntas de Examen

### Conceptuales:
- ¿Qué es el aprendizaje supervisado vs no supervisado?
- ¿Por qué es importante dividir los datos en train/test?
- ¿Qué es overfitting y cómo evitarlo?
- ¿Cuál es la diferencia entre Ridge y Lasso?

### Técnicas:
- ¿Cómo funciona el algoritmo KNN?
- ¿Qué mide el R² en regresión?
- ¿Cómo interpretar una matriz de confusión?
- ¿Para qué sirve PCA?

## 📁 Estructura del Proyecto

```
machine-learning-tutorial/
├── README.md                                    # Este archivo
├── machine-learning-tutorial-for-beginners.ipynb # Notebook principal
├── requirements.txt                             # Dependencias
└── data/                                       # Datos (si se agregan)
    └── column_2C_weka.csv
```

## 👨‍💻 Autor

**Irving Morales**  
📧 Email: 220732@utxicotepec.edu.mx  
🎓 Estudiante de Machine Learning  
🔗 GitHub: [@IrvingMordo26](https://github.com/IrvingMordo26)

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo [LICENSE](LICENSE) para más detalles.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📞 Contacto

Si tienes preguntas sobre este tutorial o quieres colaborar, no dudes en contactarme.

---

⭐ **¡No olvides darle una estrella al repositorio si te fue útil!** ⭐# Irving-Dataset-Ortopedia
