# COVID-19 Image Classification with CNN

An educational project that trains convolutional neural networks (CNNs) to classify images labeled **Covid** or **Normal**. It includes a Jupyter notebook, a NumPy image array, and a CSV of image labels.

> **Disclaimer:** This project is for learning purposes only. It is not a medical device and must not be used to diagnose or guide treatment.

## Dataset

- **251 color images**, each with shape `128 × 128 × 3` (RGB).
- **111** images labeled `Covid` and **140** labeled `Normal`.
- `CovidImages .npy` contains the images.
- `CovidLabels (1).csv` contains the corresponding labels in a `Label` column.
- Labels are mapped to `Covid = 1` and `Normal = 0` in the notebook.

The notebook uses a stratified split of 70% training, 15% validation, and 15% testing, then normalizes image pixel values to the range 0–1. It builds and evaluates CNN models and reports metrics including accuracy and COVID recall.

## Repository contents

| File | Description |
|---|---|
| `Covid-19(CNN).ipynb` | Data exploration, preprocessing, CNN training, and evaluation |
| `CovidImages .npy` | Image data array |
| `CovidLabels (1).csv` | Image labels |

## Requirements

Python 3 and Jupyter Notebook are required. Install the notebook dependencies with:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow jupyter
```

## Run the notebook

1. Clone or download this repository.
2. Install the requirements above.
3. Open `Covid-19(CNN).ipynb` in Jupyter Notebook or JupyterLab.
4. Update the image and label file paths in the notebook to point to the files in your local repository. The notebook currently contains machine-specific absolute paths.
5. Run the notebook cells in order.

Training time and model results depend on your hardware and software environment; see the notebook outputs for the results from a particular run.
