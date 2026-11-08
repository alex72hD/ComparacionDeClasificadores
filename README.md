# Comparación de clasificadores

Proyecto de aprendizaje computacional para comparar clasificadores que predicen si un cliente suscribe un depósito a plazo tras una campaña de marketing telefónico.

## Dataset

- **Enlace original:** [Bank Marketing Dataset en Kaggle](https://www.kaggle.com/datasets/janiobachmann/bank-marketing-dataset).
- **Procedencia:** publicado en Kaggle por Janio Martinez Bachmann. La descripción de Kaggle cita el trabajo de S. Moro, P. Cortez y P. Rita, “A Data-Driven Approach to Predict the Success of Bank Telemarketing”, *Decision Support Systems*, 62:22–31, 2014.
- **Descarga/carga:** se incluye una copia del CSV en `data/bank.csv`. El notebook busca el archivo con una ruta relativa al proyecto; si no está, descarga el dataset público desde Kaggle con `kagglehub`. No se requieren rutas absolutas ni archivos de credenciales para usar la copia incluida.
- **Registros y variables:** 11.162 registros, 16 variables de entrada y una variable objetivo.
- **Objetivo:** `deposit` (se asigna a `y` en el notebook), que indica si el cliente suscribió un depósito a plazo.
- **Clases:** `no` — 5.873 (52,62 %); `yes` — 5.289 (47,38 %).

Las variables y una carga verificable del dataset se describen en [`notebooks/Clasificadores.ipynb`](notebooks/Clasificadores.ipynb).

## Ejecución

Desde la carpeta del proyecto, instala las dependencias y abre el notebook:

```bash
pip install -r requirements.txt
jupyter notebook notebooks/Clasificadores.ipynb
```

La copia de `data/bank.csv` permite ejecutar la carga sin conexión a Kaggle. Si se elimina esa copia, la descarga de respaldo requiere conexión a internet.
