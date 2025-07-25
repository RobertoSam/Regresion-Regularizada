# Regresión Regularizada: Ridge, Lasso y Elastic Net

Este repositorio contiene un notebook interactivo con teoría y práctica de tres técnicas de regresión regularizada:
- **Ridge** (penalización L2)
- **Lasso** (penalización L1)
- **Elastic Net** (combinación L1 + L2)

## 📘 Objetivos del notebook

- Comprender la motivación de la regularización en modelos lineales.
- Comparar matemáticamente y gráficamente Ridge, Lasso y Elastic Net.
- Aplicar cada técnica a un conjunto de datos reales (`Diabetes` de sklearn).
- Visualizar las diferencias en los coeficientes estimados.
- Evaluar rendimiento usando RMSE y R².

## 📁 Archivos

- `Regresion_Regularizada_Detallada.ipynb`: Notebook completo listo para ejecutar.
- `trayectorias_regularizadas.ipynb`: Visualización de cómo los coeficientes cambian con alpha.

## 🧪 Requisitos

- Python ≥ 3.8
- scikit-learn
- matplotlib
- numpy

Instalación rápida:

```bash
pip install -r requirements.txt
```

## 🚀 Ejecutar en Google Colab

[Haz clic aquí para abrir el notebook en Colab](https://colab.research.google.com/github/RobertoSam/Regresion-Regularizada/blob/main/Regresion_Regularizada_Detallada.ipynb)

## 📊 Ejemplo de uso

```python
from sklearn.linear_model import Ridge
model = Ridge(alpha=1.0)
model.fit(X_train, y_train)
```

## 🤝 Autor

Este material fue desarrollado como apoyo didáctico para estudiantes de la Maestría en Modelización Matemática y Computacional de la UNI (Perú).

---
