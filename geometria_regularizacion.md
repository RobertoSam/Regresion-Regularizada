# 📐 Geometría de la Regularización

La regularización en regresión consiste en restringir el tamaño de los coeficientes para evitar sobreajuste. Cada tipo de regularización impone una **región geométrica distinta** sobre la cual se optimiza el error.

## 📊 Tabla comparativa

| Método         | Penalización               | Región geométrica      | Efecto típico                               |
|----------------|----------------------------|-------------------------|---------------------------------------------|
| **Ridge**      | $\sum_j \beta_j^2$       | Círculo / Esfera        | Coeficientes pequeños, ninguno exactamente cero |
| **Lasso**      | $\sum_j |\beta_j|$       | Rombos / Poliedros      | Algunos coeficientes exactamente cero       |
| **Elastic Net**| $\alpha L1 + (1 - \alpha) L2$ | Región intermedia | Combinación de selección y estabilidad      |

---

## 🧭 Explicación geométrica

Durante la estimación, el modelo minimiza el **error cuadrático** sujeto a una restricción. Esa restricción define una **región de búsqueda**. El punto óptimo se encuentra donde la elipse de error (líneas de nivel del MSE) **toca** esta región:

- 🔵 Ridge: al ser una esfera, penaliza uniformemente → reduce varianza sin eliminar variables.
- 🔷 Lasso: el rombo fuerza algunos coeficientes a ser cero → útil para selección de variables.
- 🌀 Elastic Net: combina ambas propiedades → útil cuando hay muchas variables correlacionadas.

### 📎 Imagen explicativa

![Geometría Ridge, Lasso y Elastic Net](graficos_regularizacion/A_2D_digital_illustration_features_three_geometric.png)

---

## 📚 Bibliografía recomendada

- Hastie, T., Tibshirani, R., & Friedman, J. (2009). **The Elements of Statistical Learning**. Springer.
- James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). **An Introduction to Statistical Learning**. Springer.
- Zou, H., & Hastie, T. (2005). **Regularization and variable selection via the elastic net**. *Journal of the Royal Statistical Society: Series B*, 67(2), 301–320.
- Tibshirani, R. (1996). **Regression Shrinkage and Selection via the Lasso**. *Journal of the Royal Statistical Society: Series B*, 58(1), 267–288.

---

