# Multiple Disease Prediction System

A machine learning-based web application that predicts the likelihood of diabetes and heart disease using user input and displays results interactively via a Streamlit frontend.

## Features

- **Diabetes Prediction**: Uses Support Vector Machine (SVM) on the PIMA Indian Diabetes dataset.
- **Heart Disease Prediction**: Uses Logistic Regression on the Cleveland Heart Disease dataset.
- **Interactive Web UI**: Built with Streamlit and streamlit-option-menu.
- **Robust Input Validation**: Prevents calculation on incomplete or invalid input.
- **Modular Design**: Easily extendable to include more diseases.

## Project Structure
multiple-disease-prediction-system/
│
├── colab_files_to_train_models/ # Not included in Git (see .gitignore)
├── dataset/
│ ├── diabetes.csv
│ └── heart.csv
├── MDPredict.py # Main Streamlit UI and prediction logic
├── multiple disease predict.py # Alternative main file (if present)
├── Multiple-disease-prediction-system-diabetes.ipynb # Model training notebook
├── Multiple-disease-prediction-system-heart.ipynb # Model training notebook
├── .gitignore

## Installation

### 1. Clone the Repo
git clone https://github.com/izharisnia/multiple-disease-prediction-system.git
cd multiple-disease-prediction-system


### 2. Install Required Packages
If `requirements.txt` is missing, install manually:
pip install streamlit streamlit-option-menu scikit-learn pandas numpy


## Usage

### 1. Train Models (if `.sav` files not present)
Use the Jupyter notebooks or Python scripts to train and save the models as `diabetes_model.sav` and `heart_disease_model.sav` in the project directory.

### 2. Run the Streamlit Frontend
streamlit run MDPredict.py
Then open your browser and go to [http://localhost:8501](http://localhost:8501).

## How It Works
- Enter values in the web form for diabetes or heart disease prediction.
- The app validates input and uses the trained ML model to predict risk.
- The result is displayed on the page.

## Datasets
- **Diabetes**: [PIMA Indian Diabetes Dataset](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)
- **Heart Disease**: [Cleveland Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+Disease)

## Customization
To add new diseases:
1. Train a new model (with a notebook or script).
2. Save the model file.
3. Add UI elements and prediction code to `MDPredict.py`.

## License
MIT License

## Authors
- Isnia Izhar





