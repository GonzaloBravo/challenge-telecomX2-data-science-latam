# Challenge Telecom X - Parte 2: análisis de evasión de clientes para G8 - ONE de Alura Latam

## :brain: Objetivos del proyecto

- Comprender los factores que llevan a que la empresa "Telecom X" tenga una alta tasa de cancelaciones, lo que repercute en la pérdida de clientes
- Recopilar, procesar y analizar los datos, utilizando Python y sus principales bibliotecas 
- Extraer información detallada
- Realizar un análisis detallado para que el equipo de Data Science pueda avanzar en modelos predictivos y desarrollar estrategias para reducir la evasión
- Desarrollar modelos predictivos capaces de prever qué clientes tienen mayor probabilidad de cancelar sus servicios
- Preparar los datos para el modelado (tratamiento, codificación, normalización)
- Realizar análisis de correlación y selección de variables
- Entrenar dos o más modelos de clasificación
- Evaluar el rendimiento de los modelos con métricas
- Interpretar los resultados, incluyendo la importancia de las variables
- Crear una conclusión estratégica señalando los principales factores que influyen en la cancelación

## :hammer_and_wrench: Desarrollo del proyecto

- Importar y manipular datos desde una API de manera eficiente
- Aplicar los conceptos de ETL (Extracción, Transformación y Carga) en la preparación de los datos
- Crear visualizaciones estratégicas para identificar patrones y tendencias
- Realizar un Análisis Exploratorio de Datos (EDA) y generar un informe con insights relevantes
- Carga del archivo CSV que contiene los datos
- Eliminar columnas que no aportan valor al análisis o a los modelos predictivos, como identificadores únicos (por ejemplo, el ID del cliente). Estas columnas no ayudan en la predicción de la cancelación y pueden incluso perjudicar el desempeño de los modelos
- Transformación de las variables categóricas a formato numérico para hacerlas compatibles con los algoritmos de machine learning. Utilizando un método de codificación adecuado, como one-hot encoding
- Calcular la proporción de clientes que cancelaron en relación con los que permanecieron activos. Evaluando si existe un desbalance entre las clases, ya que esto puede impactar en los modelos predictivos y en el análisis de los resultados
- Profundizar en el análisis, aplicando técnicas de balanceo como undersampling o oversampling. En situaciones de fuerte desbalanceo, herramientas como SMOTE pueden ser útiles para generar ejemplos sintéticos de la clase minoritaria
- Normalización o estandarización de los datos, según los modelos que se aplicarán. Modelos basados en distancia, como KNN, SVM, Regresión Logística y Redes Neuronales, requieren este preprocesamiento. Por otro lado, modelos basados en árboles, como Decision Tree, Random Forest y XGBoost, no son sensibles a la escala de los datos.
  
## :memo: Extracción de datos

 - Para iniciar el análisis, necesitaremos importar los datos de la API de Telecom X. Estos datos están disponibles en formato JSON y contienen información esencial sobre los clientes, incluyendo datos          demográficos,   tipo de servicio contratado y estado de evasión
 - Cargar los datos directamente desde la API utilizando Python.
 - Convertir los datos a un DataFrame de Pandas para facilitar su manipulación
   
 ## :computer: Conjuntos y estructura de datos

 Para comprender la estructura del dataset y el significado de sus columnas, identificaremos qué variables son más relevantes para el análisis de evasión de clientes
 - Diccionario de datos con la descripción de cada columna
 - Explorar las columnas del dataset y verificar sus tipos de datos
 - Consultar el diccionario para comprender mejor el significado de las variables
 - Identificar las columnas más relevantes para el análisis de evasión
 - Creación de al menos dos modelos diferentes para predecir la cancelación de clientes
 - Evaluación de cada modelo utilizando las siguientes métricas: Exactitud (Acurácia) - Precisión - Recall - F1-score - Matriz de confusión

 
## :clipboard: Comprobación de incoherencias en los datos y manejo de inconsistencias

  - Verificación de problemas en los datos que puedan afectar el análisis
  - Atención a valores ausentes, duplicados, errores de formato e inconsistencias en las categorías
  - Identificación de inconsistencias y aplicación las correcciones necesarias.
  - Ajuste de datos para asegurar que estén completos y coherentes, preparándolos para las siguientes etapas del análisis
  - Separación de conjuntos de datos en entrenamiento y prueba para evaluar el rendimiento del modelo. 

##  :bar_chart: Carga y análisis(L - Load & Analysis)

-  Análisis descriptivo de los datos, calculando métricas como media, mediana, desviación estándar y otras medidas que ayuden a comprender mejor la distribución y el comportamiento de los clientes
-  Comprender cómo está distribuida la variable "churn" (evasión) entre los clientes. Utilización de gráficos para visualizar la proporción de clientes que permanecieron y los que se dieron de baja
-  Explorar cómo se distribuye la evasión según variables categóricas, como género, tipo de contrato, método de pago, entre otras, revelando patrones interesantes, por ejemplo, si los clientes de ciertos perfiles tienen una mayor tendencia a cancelar el servicio, lo que ayudará a orientar acciones estratégicas
- Explorar cómo las variables numéricas, como "total gastado" o "tiempo de contrato", se distribuyen entre los clientes que cancelaron (evasión) y los que no cancelaron, para entender si ciertos valores numéricos están más asociados con la evasión, proporcionando insights sobre los factores que influyen en el comportamiento de los clientes
- Visualización de la matriz de correlación para identificar relaciones entre las variables numéricas. Prestando especial atención a las variables que muestran una mayor correlación con la cancelación, ya que estas pueden ser fuertes candidatas para el modelo predictivo.
- Anáñisis dirigido de variables específicas que se relacionan con la cancelación, tales como: Tiempo de contrato × Cancelación y Gasto total × Cancelación. Utilizando gráficos como boxplots o scatter plots para visualizar patrones y posibles tendencias

## :white_check_mark: Informe Final

- Introducción: Explica el objetivo del análisis y el problema de evasión de clientes (Churn)
- Limpieza y Tratamiento de Datos: Describe los pasos realizados para importar, limpiar y procesar los datos
- Análisis Exploratorio de Datos: Presenta los análisis realizados, incluyendo gráficos y visualizaciones para identificar patrones
- Conclusiones e Insights: Resume los principales hallazgos y cómo estos datos pueden ayudar a reducir la evasión
- Informe detallado, destacando los factores que más influyen en la cancelación, basado en las variables seleccionadas y en el rendimiento de cada modelo
- Identificar los principales factores que afectan la cancelación de clientes y proponer estrategias de retención basadas en los resultados obtenidos

