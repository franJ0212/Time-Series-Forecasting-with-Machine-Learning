# Time Series Forecasting with Machine Learning

Análisis comparativo de métodos de Machine Learning y Deep Learning aplicados al pronóstico de series de tiempo. El proyecto evalúa el rendimiento de diferentes algoritmos en escenarios con características temporales distintas.

## Modelos Implementados

- **ARIMA** - Modelos autoregresivos de medias móviles integrados
- **SVR** - Support Vector Regression con kernels RBF
- **MLP** - Perceptrón Multicapa
- **LSTM** - Redes de memoria a corto y largo plazo
- **GRU** - Gated Recurrent Units
- **ESN** - Echo State Networks
- **Ensemble Methods** - Combinación de predicciones mediante técnicas de ensamble

## Datasets

### AirPassengers
Serie temporal clásica con 144 observaciones mensuales (1949-1960) de pasajeros de aerolíneas internacionales. Presenta tendencia creciente y estacionalidad multiplicativa bien definida.

### NVIDIA (NVDA)
Precios de cierre históricos de acciones de NVIDIA. Serie caracterizada por alta volatilidad, cambios abruptos de tendencia y comportamiento no estacionario.

## Estructura del Repositorio

```
.
├── FranciscoHernandez_OscarPerez_Proyecto.ipynb    # Notebook con implementación completa
├── FranciscoHernandez_OscarPerez_Proyecto.pdf      # Documento técnico detallado
├── AirPassengers.csv                                # Dataset de pasajeros aéreos
├── NVDA.csv                                         # Dataset de precios NVIDIA
└── Contribuciones.txt                               # Distribución del trabajo
```

## Notebook Principal

[FranciscoHernandez_OscarPerez_Proyecto.ipynb](FranciscoHernandez_OscarPerez_Proyecto.ipynb)

El notebook incluye:

- Carga y preprocesamiento de datos temporales
- Análisis exploratorio con descomposición de series
- Transformación de datos (FFT, medias móviles, feature engineering)
- Implementación de modelos tradicionales y redes neuronales
- Evaluación mediante métricas RMSE, MAE y MAPE
- Comparativa de rendimiento entre algoritmos
- Visualizaciones de predicciones vs valores reales

## Documento Técnico

El archivo PDF contiene la fundamentación teórica completa, incluyendo:

- Conceptos de series de tiempo (tendencia, estacionalidad, ciclicidad)
- Métodos de preparación y transformación de datos
- Arquitecturas de redes neuronales para secuencias temporales
- Estrategias de validación temporal
- Análisis comparativo de resultados
- Conclusiones sobre aplicabilidad de cada método

## Métricas de Evaluación

- **RMSE** (Root Mean Squared Error)
- **MAE** (Mean Absolute Error)
- **MAPE** (Mean Absolute Percentage Error)

## Tecnologías

- Python 3.x
- NumPy, Pandas
- Scikit-learn
- TensorFlow/Keras
- Statsmodels
- Matplotlib, Seaborn

## Resultados Principales

Los modelos tradicionales como ARIMA muestran buen desempeño en series estacionarias con patrones regulares (AirPassengers: MAPE ~2.8%), mientras que las redes neuronales recurrentes (LSTM, GRU) demuestran mayor robustez en series volátiles y no estacionarias (NVDA).

Los métodos de ensamble combinan las fortalezas de múltiples predictores, mejorando la estabilidad de las predicciones en diferentes escenarios.

## Autores

Francisco Hernández | Oscar Pérez
