## Ley de grandes números

<p>Es un teorema fundamental en la probabilidad y la estadística que describe el comportamiento de una muestra a medida que aumenta su tamaño. Explica que, bajo ciertas condiciones, la media de los resultados obtenidos de un gran número de experimentos repetidos se aproximará a la media esperada o teórica.</p>

### Tipos de la Ley de los Grandes Números
Existen dos tipos principales de la Ley de los Grandes Números:
1. **Ley de los Grandes Números Débil**: Establece que, para un número suficientemente grande de observaciones, la media muestral convergerá en probabilidad hacia la media poblacional.
2. **Ley de los Grandes Números Fuerte**: Declara que, al aumentar indefinidamente el número de observaciones, la media muestral converge casi con certeza (probabilidad 1) a la media poblacional.

### Explicación
Si \( X_1, X_2, \ldots, X_n \) son variables aleatorias independientes e idénticamente distribuidas con media esperada \( \mu \), entonces la media muestral:
\[
\bar{X}_n = \frac{1}{n} \sum_{i=1}^n X_i
\]
se aproximará a \( \mu \) a medida que \( n \) tiende a infinito. Esto es:
\[
\lim_{{n \to \infty}} \bar{X}_n = \mu
\]

### Fórmulas y Notación
| Notación                | Descripción                                                                                |
|-------------------------|--------------------------------------------------------------------------------------------|
| \( X_1, X_2, \ldots, X_n \) | Variables aleatorias independientes con distribución idéntica y media esperada \( \mu \). |
| \( \bar{X}_n \)              | Media muestral calculada como \( \bar{X}_n = \frac{1}{n} \sum_{i=1}^n X_i \).          |
| \( \lim_{{n \to \infty}} \bar{X}_n = \mu \) | Convergencia de la media muestral hacia la media poblacional \( \mu \) a medida que \( n \) crece. |

### Ejemplo
Consideremos un experimento en el que lanzamos una moneda equilibrada. La probabilidad de obtener **cara** o **cruz** es 0.5. Según la Ley de los Grandes Números:
- Si lanzamos la moneda solo 10 veces, la proporción de caras podría no ser exactamente 0.5 debido a la pequeña muestra.
- Sin embargo, si lanzamos la moneda 1,000 o 10,000 veces, la proporción de caras tenderá a acercarse cada vez más a 0.5.

### Importancia
La Ley de los Grandes Números es esencial para la estadística inferencial, ya que garantiza que las muestras grandes proporcionan estimaciones más precisas de los parámetros poblacionales.

---

Este teorema nos permite confiar en los resultados de experimentos de gran tamaño, y en cómo las medias muestrales tienden a representar mejor la media poblacional conforme aumenta el tamaño de la muestra.