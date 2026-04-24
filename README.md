# MLflow Experiment Tracking

A hands-on repository demonstrating how to use **MLflow** for experiment tracking, model logging, and prediction workflows with scikit-learn. This project covers MLflow basics as well as an end-to-end prediction pipeline with experiment management.

---

## 📁 Repository Structure

```
ML-Flow/
├── basics/
│   └── basics.ipynb              # Introduction to MLflow core concepts
├── Prediction_With_MLFlow.ipynb  # End-to-end ML pipeline with MLflow tracking
├── requirements.txt              # Python dependencies
├── .gitignore
└── README.md
```

---

## 📌 Overview

This repository explores key MLflow capabilities:

- **Experiment Tracking** – Log parameters, metrics, and artifacts per run
- **Model Logging** – Save and version trained scikit-learn models
- **MLflow UI** – Visualize and compare runs via the built-in dashboard
- **Prediction Pipeline** – Load logged models and run inference

---

## 🧪 Notebooks

### `basics/basics.ipynb`
Covers the fundamentals of MLflow:
- Creating and managing experiments
- Logging parameters and metrics with `mlflow.log_param()` / `mlflow.log_metric()`
- Logging and loading models using `mlflow.sklearn.log_model()`
- Navigating the MLflow tracking UI

### `Prediction_With_MLFlow.ipynb`
An end-to-end machine learning workflow:
- Data preparation using **pandas** and **NumPy**
- Model training with **scikit-learn**
- Full MLflow run tracking (params, metrics, model artifacts)
- Loading a logged model from the MLflow registry for prediction

---

## ⚙️ Setup & Installation

### Prerequisites
- Python 3.8+
- pip

### Install Dependencies

```bash
git clone https://github.com/Somesh-Salunkhe/ML-Flow.git
cd ML-Flow
pip install -r requirements.txt
```

### Dependencies (`requirements.txt`)
| Package | Purpose |
|---|---|
| `mlflow` | Experiment tracking & model registry |
| `scikit-learn` | ML model training |
| `pandas` | Data manipulation |
| `numpy` | Numerical computing |

---

## 🚀 Running the Notebooks

1. Launch Jupyter Notebook or JupyterLab:
   ```bash
   jupyter notebook
   ```

2. Open and run either notebook:
   - Start with `basics/basics.ipynb` for a guided introduction
   - Proceed to `Prediction_With_MLFlow.ipynb` for a full pipeline walkthrough

---

## 📊 Launching the MLflow UI

After running any notebook, start the MLflow tracking UI to visualize logged experiments:

```bash
mlflow ui
```

Then open your browser at: [http://localhost:5000](http://localhost:5000)

---

## 🛠️ Key MLflow Concepts Used

| Concept | Description |
|---|---|
| `mlflow.start_run()` | Starts a new experiment run |
| `mlflow.log_param()` | Logs a single hyperparameter |
| `mlflow.log_metric()` | Logs an evaluation metric |
| `mlflow.sklearn.log_model()` | Saves a scikit-learn model as an artifact |
| `mlflow.sklearn.load_model()` | Loads a saved model for inference |

---

## 👤 Author

**Somesh Salunkhe**  
[GitHub](https://github.com/Somesh-Salunkhe)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
