# Proyecto DATATON - Equipo 21

## Resumen del Proyecto
Este proyecto tiene como objetivo predecir la ubicación óptima para la apertura de nuevas farmacias en México, enfocándose en identificar municipios con alto potencial. Utilizando una red neuronal y diversos indicadores económicos, se proporcionan recomendaciones basadas en datos regionales y variables estratégicas.

## Miembros del Equipo
- **Eduardo García** - Lic. en Ciencia de Datos, Ganador de beca ERASMUS
- **Diego Méndez** - Lic. en Ciencia de Datos, Pasante en DiDi
- **Harry Gomar** - Ing. en Negocios, Coordinador de Makers ITAM
- **Mauricia Peña** - Lic. en Matemáticas Aplicadas, Pasante en Business Data Evolution
- **Diego Cottin** - Faculty en 4Geeks Academy España, Lic. en Matemáticas Aplicadas

## Contexto
- El proyecto utiliza una red neuronal entrenada con datos de farmacias de alto rendimiento.
- Se realizó un análisis comparativo para interpretar indicadores económicos regionales.
- La selección estratégica de 200 municipios para la apertura de nuevas farmacias se hizo analizando datos abiertos del INEGI y considerando variables económicas y demográficas.

## Resultados Principales
- Se analizaron **1,156 municipios**, identificando **441 como de alto rendimiento**.
- Se recomendaron **46 municipios** en **20 estados** para la apertura de farmacias, representando un valor de mercado potencial de **1330 millones de pesos**.
- Se agruparon y evaluaron los municipios con base en indicadores económicos y demográficos como ROE, ROA, rentabilidad, ingresos, gastos y eficiencia.

## Modelo de Predicción
- El modelo de predicción se entrenó con **1,375 datos** y **45 variables de entrada** para predecir el número de farmacias necesarias en cada municipio.
- Las variables clave que influyeron en las predicciones incluyeron los ingresos por farmacia, eficiencia, similitud con municipios comparables y diferencias entre los resultados del modelo y la realidad.
- El modelo alcanzó los siguientes resultados:
  - **RMSE**: 23.2862
  - **R² Score**: 0.9677
  - Optimizado utilizando XGBoost.

## Mejoras Futuras
- Análisis adicional sobre la optimización de la localización de farmacias utilizando datos de cobertura de farmacias existentes.
- Integración de nuevos datos independientes sobre infraestructura, enfermedades, crimen y censos actualizados para refinar las predicciones.

## Ejemplos de Recomendaciones por Municipio
| Municipio             | Farmacias Recomendadas |
|-----------------------|------------------------|
| Xalapa                | 17                     |
| Cadereyta Jiménez      | 5                      |
| Piedras Negras         | 8                      |
| Celaya                | 1                      |
| Puebla                | 42                     |
| Toluca                | 28                     |
| Monterrey             | 2                      |
| Veracruz              | 9                      |
| San Pedro Tlaquepaque | 13                     |

# Archivos 
## Codigo
### Procesamiento 
PREP_PreprocesamientoDatos.ipynb
PREP_TopFarmacias.ipynb
PREP_Clusters.ipynb
### Red Neuronal
RN_EntrenamientoRedNeuronalFarmacias.ipynb
RN_PrediccionesRNF.ipynb
### Interpretacion
INTER_RankingResultados.ipynb
INTER_DistanciaEuclidiana.ipynb