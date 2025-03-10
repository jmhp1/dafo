# Data Analysis and Vizualisation for Oceanographers
Hola! Si estas leyendo esto es que vas a cursar el Data Analysis For Oceanographers. La idea y proposito de este curso es que puedas aprender no solo a procesar tus datos, sino que tambien puedas, de forma autonoma, encontrar la mejor manera de representarlos. En cierta forma, este curso surge de las necesidades que yo encontre al ser estudiante de Ciencias del Mar. Al terminar el grado, o incluso haciendo el TFG, veia que procesar datos era algo en lo que yo me sentia comodo, me gustaba, pero no tenia las herramientas correctas. A la vez, se me exigia: escribir, representar, analizar e interpretar los datos. Por eso, tras mucho tiempo planeandolo, he creado este curso, el DAFO. 

Al llegar a 3o de carrera me di cuenta que lo que me apasionaba era la fisica. Ademas, me apasionaba el proceso por el cual nuestros datos se transformaan en meros numeros a ideas, conclusiones, hipotesis, e incluso, con suerte, alguna contribucion inteligente. Por ello me centre, y obsesione, con aprender sobre eso. En mi TFG no sabia ni hacer una regresion en MatLab, ahora la puedo hacer en, al menos 5 lenguajes. Por que si, no hay una solucion unica a un mismo problema, cada persona debe encontrar las herramientas que mejor se ajusten a su proyecto y a sus necesidades en cada momento. Utilizamos estos lenguajes por que queremos procesar datos, no somos, aun, desarrolladores de software. 

Por otro lado, creo que este curso es ideal para todas aquellas personas que esten cursando 3o o 4o de CCDM o que esten realizando el MSc. Por que? Por que en tu vida laboral, si tienes que presentar datos, debes hacerlo de la mejor manera, de una forma acertiva, util y que permita al grupo que te este escuchando, centrarse en lo que explicas, para poder ponerlo en duda. Para ello, nos guiaremos por la idea del 'menos es mas' para construir nuestros graficos, mapas o videos. Las graficas deben acompanar a tus palabras.

#### El curso esta dividido en tres grandes bloques:
0. Instalacion de todo el software que vamos a utilizar.

Ya sea con un Mac, una maquina virtual o un ordenador prestado, vamos a hacer que todo funcione. Para ello debeis seguir los pasos que os indico a continuacion.

- Descargar pyhton.
- Descargar vsCode.
- Abrir vsCode e instalar las siguientes extensiones, son como apps dentro del programa.
- Comandos basicos de unix/bash + uso de terminal.
- Crear y activar tu virtual environment.
- Crear una carpeta-proyecto general, te servira como esqueleto en cualquier proyecto futuro.

## Project Structure

```plaintext
README.md          <- The top-level README for developers.
├── conf            <- Space for credentials (for secure storage of sensitive information).
│
├── data            <- Contains all data for the project.
│   ├── 01_raw      <- Immutable input data (data collected or received in raw form).
│   ├── 02_intermediate<- Cleaned version of raw data (pre-processed and ready for analysis).
│   ├── 03_processed<- Data used to develop models (cleaned and transformed).
│   ├── 04_models   <- Trained models (after the model training step).
│   ├── 05_model_output<- Model output (predictions made by the trained models).
│   └── 06_reporting<- Reports and input to frontend (final outputs for reporting purposes).
│
├── docs            <- Documentation generated with Sphinx (for project-specific documentation).
│
├── notebooks       <- Jupyter notebooks for exploring and experimenting with the data.
│   └── YYYYMMDD    <- Notebooks named by date (e.g., `20220315_AB-model-testing`).
│
├── references      <- Reference materials such as data dictionaries, manuals, etc.
│
├── results         <- Final analysis reports and documents for model evaluation and reporting.
│
├── requirements.txt <- Required Python packages for setting up the analysis environment.
│
├── .gitignore      <- Defines files and directories to be ignored by Git (e.g., data, credentials).
│
└── src             <- Source code for use in this project.
    ├── __init__.py <- Makes `src` a Python module.
    │
    ├── d00_utils   <- Utility functions used across the project.
    │   └── remove_accents.py <- Example of a utility script.
    │
    ├── d01_data    <- Scripts for reading and writing data (e.g., loading CSVs, processing).
    │   └── load_data.py <- Example script to load data into the system.
    │
    ├── d02_intermediate <- Data transformation scripts to turn raw data into intermediate form.
    │   └── create_int_payment_data.py <- Script to create cleaned intermediate data.
    │
    ├── d03_processing <- Scripts that process data into modeling-ready input.
    │   └── create_master_table.py <- Script to prepare master table for model input.
    │
    ├── d04_modelling  <- Scripts to train models and make predictions.
    │   └── train_model.py <- Example model training script.
    │
    ├── d05_model_evaluation <- Scripts that evaluate the performance of models.
    │   └── calculate_performance_metrics.py <- Script to calculate model evaluation metrics.
    │
    ├── d06_reporting <- Scripts that generate reports based on model output.
    │   └── create_rpt_payment_summary.py <- Example script to create reports.
    │
    └── d07_visualisation <- Scripts for visualizing data and results (plots, charts).
        └── visualise_patient_journey.py <- Example script for creating patient journey visualizations.
```

2. Python como erramienta de **analisis de datos**.

 - Instalacion de todos los requirements. (2h)
 - Por que python? (1h)
 - Modulos interesantes: xarray, cartopy, pandas, matplotlib, seaborn. (1h)
 - Como organizar mi proyecto: ejemplo de una carpeta que contenga todos los elementos necesarios para que el poryecto sea replicable.
 - Como podemos descargar nuestros datos? (1h)
 - Abrir archivos netCDF (1h)
 - 
   
2. Python como erramienta de **visualizacion de datos**.
 
 - A quien presento condiciona como presento.
 - Lo que digo tiene que
 - Por que debemos representar bien nuestros datos?

  *Todo el material estara disponible y es replicable* a traves del repositorio en GitHub **plan**.



