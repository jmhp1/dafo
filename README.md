# Data Analysis and Visualization for Oceanographers

¡Hola! Si estás leyendo esto, es porque vas a cursar **Data Analysis for Oceanographers**. La idea y propósito de este curso es que puedas aprender no solo a procesar tus datos, sino también a encontrar la mejor manera de representarlos de forma autónoma. Este curso surge de las necesidades que encontré al ser estudiante de Ciencias del Mar. Al terminar el grado, o incluso haciendo el TFG, veía que procesar datos era algo en lo que me sentía cómodo y me gustaba, pero no tenía las herramientas correctas. A la vez, se me exigía escribir, representar, analizar e interpretar los datos. Por eso, tras mucho tiempo planeándolo, he creado este curso, el **DAFO**.

Al llegar a tercero de carrera, me di cuenta de que lo que me apasionaba era la física. Además, me apasionaba el proceso por el cual nuestros datos se transforman de meros números a ideas, conclusiones, hipótesis, e incluso, con suerte, alguna contribución inteligente. Por ello, me centré y obsesioné con aprender sobre eso. En mi TFG no sabía ni hacer una regresión en MatLab, ahora la puedo hacer en al menos cinco lenguajes. Porque sí, no hay una solución única a un mismo problema; cada persona debe encontrar las herramientas que mejor se ajusten a su proyecto y a sus necesidades en cada momento. Utilizamos estos lenguajes porque queremos procesar datos, no somos, aún, desarrolladores de software.

Por otro lado, creo que este curso es ideal para todas aquellas personas que estén cursando tercero o cuarto de CCDM o que estén realizando el MSc. ¿Por qué? Porque en tu vida laboral, si tienes que presentar datos, debes hacerlo de la mejor manera, de forma asertiva, útil y que permita al grupo que te esté escuchando centrarse en lo que explicas, para poder ponerlo en duda. Para ello, nos guiaremos por la idea del "menos es más" para construir nuestros gráficos, mapas o videos. Las gráficas deben acompañar a tus palabras.

## El curso está dividido en tres grandes bloques:

### 1. Instalación de todo el software que vamos a utilizar

Ya sea con un Mac, una máquina virtual o un ordenador prestado, vamos a hacer que todo funcione. Para ello, debéis seguir los pasos que os indico a continuación:

- Descargar Python.
- Descargar VSCode.
- Abrir VSCode e instalar las siguientes extensiones, que son como apps dentro del programa.
- Comandos básicos de Unix/Bash + uso de terminal.
- Crear y activar tu entorno virtual.
- Crear una carpeta-proyecto general, que te servirá como esqueleto en cualquier proyecto futuro.

### Project Structure

```plaintext
README.md          <- The top-level README for developers.
├── conf            <- Space for credentials (for secure storage of sensitive information).
│
├── data            <- Contains all data for the project.
│   ├── 01_raw      <- Immutable input data (data collected or received in raw form).
│   ├── 02_intermediate <- Cleaned version of raw data (pre-processed and ready for analysis).
│   ├── 03_processed <- Data used to develop models (cleaned and transformed).
│   ├── 04_models   <- Trained models (after the model training step).
│   ├── 05_model_output <- Model output (predictions made by the trained models).
│   └── 06_reporting <- Reports and input to frontend (final outputs for reporting purposes).
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

### 2. Python como herramienta de **análisis de datos**

- Instalación de todos los requirements. (2h)
- ¿Por qué Python? (1h)
- Módulos interesantes: xarray, cartopy, pandas, matplotlib, seaborn. (1h)
- Cómo organizar mi proyecto: ejemplo de una carpeta que contenga todos los elementos necesarios para que el proyecto sea replicable.
- Cómo podemos descargar nuestros datos? (1h)
- Abrir archivos netCDF (1h)

### 3. Python como herramienta de **visualización de datos**

- A quién presento condiciona cómo presento.
- Lo que digo tiene que ser claro y conciso.
- ¿Por qué debemos representar bien nuestros datos?

*Todo el material estará disponible y es replicable* a través del repositorio en GitHub **plan**.
