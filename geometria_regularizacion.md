# 📐 Geometría de la Regularización

La regularización en regresión lineal introduce restricciones sobre los coeficientes del modelo mediante **penalizaciones**, que pueden interpretarse como **formas geométricas** en el espacio de parámetros. Estas formas afectan directamente cómo se obtiene la solución óptima.

---

## 🔍 Intuición geométrica

Imaginemos que minimizamos el error cuadrático bajo una restricción en los coeficientes β. Cada tipo de regularización define una "región" alrededor del origen dentro de la cual buscamos la mejor solución.

### 🟦 Ridge: Penalización L2

- **Región geométrica**: **Círculo** o **esfera** en dimensiones mayores.
- **Penalización**: `||β||²₂ ≤ t`
- **Efecto**: Empuja los coeficientes hacia cero, pero raramente exactamente cero.
- **Visualización**: Las curvas de error (óvalos) intersectan el círculo suavemente → todos los coeficientes son pequeños.

### ◼️ Lasso: Penalización L1

- **Región geométrica**: **Rombo** o **octaedro** en alta dimensión.
- **Penalización**: `||β||₁ ≤ t`
- **Efecto**: Favorece soluciones esparsas → muchos coeficientes exactamente cero.
- **Visualización**: Los vértices del rombo aumentan la probabilidad de "chocar" en el borde → selección de variables.

### 🔷 Elastic Net: Combinación L1 + L2

- **Región geométrica**: Forma **curva intermedia** entre círculo y rombo.
- **Penalización**: `α||β||₁ + (1 - α)||β||²₂`
- **Efecto**: Control balanceado entre reducción de coeficientes y esparsidad.
- **Visualización**: Superficie de intersección que combina los efectos anteriores.

---

## 🖼️ Representación visual

![Geometría de Ridge, Lasso y Elastic Net](graficos_regularizacion/A_2D_digital_illustration_features_three_geometric.png)

La imagen compara visualmente las regiones de penalización para cada técnica. El punto óptimo del modelo (mínimo del error cuadrático) se proyecta dentro de estas regiones:

- En **Ridge**, la solución suaviza todos los coeficientes.
- En **Lasso**, algunos coeficientes se hacen cero.
- En **Elastic Net**, hay un compromiso entre ambos extremos.

---

## 📚 Lecturas recomendadas

- T. Hastie, R. Tibshirani, J. Friedman — *The Elements of Statistical Learning*.
- G. James et al. — *An Introduction to Statistical Learning*.
- Zou & Hastie (2005) — *Regularization and variable selection via the elastic net*.

---

Esta geometría explica **por qué** Lasso selecciona variables, Ridge estabiliza soluciones, y Elastic Net combina lo mejor de ambos.
