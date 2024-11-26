# VISUALIZACIÓN DE DATOS

Este proyecto explora diversas técnicas de visualización de datos aplicadas al dataset del Titanic (`titanic_limpio.csv`). Utilizando la biblioteca `matplotlib`, se analizan y representan gráficamente diferentes aspectos del dataset, desde distribuciones y relaciones hasta detección de valores atípicos.

## Contenido

### 1. **Carga del Dataset**
El dataset limpio es cargado utilizando `pandas` y se realiza una inspección inicial con `head()`.

### 2. **Visualizaciones**

#### 2.1. Histograma
Se crea un histograma de la columna `age` para observar la distribución de edades de los pasajeros:
- Se eliminan valores nulos con `dropna()`.
- Configuración personalizada del gráfico con `bins`, colores y cuadrículas.

#### 2.2. Gráfico de Barras
Se representa el número de pasajeros en cada clase (`class`) mediante un gráfico de barras:
- Se utiliza la función `value_counts()` para calcular las frecuencias.
- Personalización del color para cada barra.

#### 2.3. Gráfico de Torta (Pie)
Se visualiza el porcentaje de sobrevivientes y fallecidos (`survived`):
- Las proporciones se calculan con `value_counts()`.
- Configuración de etiquetas y colores específicos.

#### 2.4. Boxplot
Se analiza la columna `fare` para identificar valores atípicos (outliers):
- Uso de `boxplot()` para mostrar la dispersión y valores extremos.
- Personalización del diseño del gráfico.

#### 2.5. Matriz de Correlación
Se calcula y visualiza la matriz de correlación para variables numéricas:
- Se seleccionan columnas numéricas utilizando `select_dtypes()`.
- Representación con un mapa de calor (`imshow`), añadiendo valores dentro de las celdas.

## Requisitos

- Python 3.x
- Bibliotecas:
  - `pandas`
  - `numpy`
  - `matplotlib`

## Cómo Usar

1. Clona este repositorio en tu máquina local.
2. Asegúrate de tener el archivo `titanic_limpio.csv` en el mismo directorio.
3. Instala las dependencias necesarias:
   ```bash
   pip install pandas numpy matplotlib
