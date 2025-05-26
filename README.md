Solución Prueba Técnica - Científico de Datos

Este repositorio presenta la solución integral a una prueba técnica orientada al rol de científico de datos. Se incluyen tanto respuestas teóricas como el desarrollo completo de un análisis exploratorio y modelos predictivos con validación cruzada, aplicados a un conjunto de datos reales sobre muertes por intervención policial en EE. UU.

Archivos incluidos

* Prueba científico de datos (propuesta).pdf: Documento con preguntas teóricas y enunciados.
* puntos_7_8.html: Notebook HTML con el desarrollo completo de los puntos prácticos.

Contenidos


Parte 1: Teoría (desde el PDF)
Incluye respuestas a temas clave como:

* Diferencia entre aprendizaje supervisado y no supervisado
* Prevalencia y su impacto en la precisión y exactitud
* Interpretación de matriz de confusión y medidas como precisión, exactitud y cociente informativo
* Evaluación de estacionariedad en series temporales y modelo ARIMA
* Cálculo del valor esperado de Δxt para procesos autoregresivos
* Ventajas del RMSE frente al MSE

Parte 2: Desarrollo Práctico

Análisis Exploratorio

* Análisis sociodemográfico de variables como manner_of_death, armed, age, gender, race.
* Evolución temporal de muertes por estado (top 5).
* Análisis por estado de ingreso, educación, pobreza y distribución racial


Modelado Predictivo

Se implementaron modelos para predecir la raza de la víctima con base en variables del incidente y del entorno:

Modelos usados:
* LogisticRegression
* SVC
* DecisionTreeClassifier
* RandomForestClassifier
* XGBoost
Técnicas adicionales:
* Oversampling con RandomOverSampler (para mitigar desbalance de clases).
* Validación cruzada estratificada (StratifiedKFold) con métricas como Accuracy, F1-Score, y Recall.
* Evaluación detallada por clase con matriz de confusión y métricas por etiqueta

Resultados Destacados

* Mejor desempeño general observado en el modelo SVC (accuracy promedio ≈ 66%).
* Modelos con pobre precisión en clases minoritarias, resaltando la importancia del balance y ajuste de métricas.
* Visualización clara de métricas por clase que permite evaluar equidad en el desempeño.

Conclusiones

El desarrollo mostró la necesidad de:

* Evaluar métricas más allá del accuracy en problemas desbalanceados.
* Implementar estrategias de balanceo como el oversampling.
* Usar validación cruzada para una evaluación robusta.

Este trabajo permite evidenciar competencias tanto teóricas como prácticas requeridas para un rol de científico de datos.
