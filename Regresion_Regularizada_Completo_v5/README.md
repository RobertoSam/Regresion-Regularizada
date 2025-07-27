# 📊 Regresiones Regularizadas: Ridge, Lasso y Elastic Net

Este repositorio contiene una unidad completa sobre regresión regularizada en modelos lineales, orientada a estudiantes de maestría y profesionales en ciencia de datos y modelación matemática.

---

## 📁 Contenido del repositorio

| Archivo | Descripción |
|--------|-------------|
| `regresion_regularizada_completa.ipynb` | Notebook integral con teoría, aplicación y comparación de Ridge, Lasso y Elastic Net |
| `ridge_regression.ipynb` | Teoría, visualización e implementación completa de **Regresión Ridge** |
| `lasso_regression.ipynb` | Teoría e implementación de **Regresión Lasso**, con enfoque en selección de variables |
| `elasticnet_regression.ipynb` | Análisis de **Elastic Net**, mostrando cómo combina Ridge y Lasso |
| `comparacion_modelos_regularizados.ipynb` | Comparación práctica y gráfica entre los tres modelos |
| `graficos_regularizacion/` | Imágenes explicativas sobre las regiones geométricas de cada modelo |

---

## 🎯 Objetivos de aprendizaje

- Comprender las limitaciones de la regresión OLS y cómo la regularización las mitiga.
- Conocer el fundamento teórico y geométrico de Ridge, Lasso y Elastic Net.
- Aplicar cada técnica en un ejemplo real, analizar sus coeficientes y evaluar su rendimiento.
- Validar los supuestos del modelo usando análisis de residuos.
- Comparar los tres métodos y justificar su elección en problemas reales.

---

## 🧠 Geometría de la regularización

![Geometría de Ridge, Lasso y Elastic Net](graficos_regularizacion/A_2D_digital_illustration_displays_geometric_repre.png)

> Este gráfico representa cómo la elección de la penalización impone distintas **regiones geométricas de solución**:
> - **Ridge**: región circular → todos los coeficientes pequeños
> - **Lasso**: región romboidal → muchos coeficientes exactamente cero
> - **Elastic Net**: región curva intermedia → mezcla entre Ridge y Lasso

---

## ⚙️ Tecnologías utilizadas

- Python 3.11
- Scikit-learn
- Numpy, Matplotlib, Seaborn
- Statsmodels, Scipy

---

## 🚀 Ejecutar en línea

- [Notebook completo en Colab](https://colab.research.google.com/github/RobertoSam/Regresion-Regularizada/blob/main/regresion_regularizada_completa.ipynb)
- [Abrir Ridge en Google Colab](https://colab.research.google.com/github/RobertoSam/Regresion-Regularizada/blob/main/ridge_regression.ipynb)
- [Abrir Lasso en Colab](https://colab.research.google.com/github/RobertoSam/Regresion-Regularizada/blob/main/lasso_regression.ipynb)
- [Abrir Elastic Net en Colab](https://colab.research.google.com/github/RobertoSam/Regresion-Regularizada/blob/main/elasticnet_regression.ipynb)
- [Comparación en Colab](https://colab.research.google.com/github/RobertoSam/Regresion-Regularizada/blob/main/comparacion_modelos_regularizados.ipynb)

---

## 🛠 Instalación local rápida

1. Clona este repositorio:
```bash
git clone https://github.com/RobertoSam/Regresion-Regularizada.git
cd Regresion-Regularizada
```

2. Crea un entorno virtual (opcional pero recomendado):
```bash
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
```

3. Instala las dependencias:
```bash
pip install -r requirements.txt
```

4. Abre los notebooks:
```bash
jupyter notebook
```

---

## 📚 Aplicaciones actuales

Las técnicas de regresión regularizada se usan ampliamente en:

- Genómica y biología computacional
- Marketing predictivo
- Selección de variables en modelos con alta dimensionalidad
- Modelos de series temporales con múltiples covariables

---

## 👨‍🏫 Autor

Material desarrollado por **Roberto Sam** para la Maestría en Modelización Matemática y Computacional – Universidad Nacional de Ingeniería (UNI), Perú.  
Asistencia técnica y didáctica desarrollada con ayuda de un asistente académico especializado en matemáticas aplicadas y ciencia de datos.


---

## 🚀 Ejecutar en Google Colab

Puedes ejecutar el notebook directamente en [Google Colab](https://colab.research.google.com/) sin instalar nada localmente.

### 📂 Desde Google Drive

1. Guarda `regresion_regularizada_completa.ipynb` en tu Google Drive.
2. Abre [https://colab.research.google.com](https://colab.research.google.com)
3. Selecciona el archivo desde la pestaña **Google Drive**
4. Ejecuta normalmente por celdas.

---

### 🔗 Desde GitHub

Si tienes el repositorio en GitHub (`RobertoSam/Regresion-Regularizada`), puedes abrirlo así:

```bash
https://colab.research.google.com/github/RobertoSam/Regresion-Regularizada/blob/main/Regresion_Regularizada_Completo/regresion_regularizada_completa.ipynb
```

### ▶️ Enlaces rápidos por técnica (si el notebook tiene títulos apropiados):

| Técnica         | Fragmento Colab (#scrollTo=...) |
|----------------|----------------------------------|
| **Ridge**       | `#scrollTo=ridge`               |
| **Lasso**       | `#scrollTo=lasso`               |
| **Elastic Net** | `#scrollTo=elasticnet`          |

> Puedes combinar el enlace base con estos fragmentos para llegar directamente a cada sección.
