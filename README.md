# 🧪 MLflow Experiment Tracking

A hands-on repository demonstrating how to use **MLflow** for experiment tracking, model logging, and end-to-end ML pipelines with scikit-learn. Projects span foundational concepts to real-world prediction tasks including house price and wine quality prediction.

---

## 📁 Repository Structure

```
ML-Flow/
├── basics/
│   └── basics.ipynb                  # Introduction to MLflow core concepts
├── House Price Prediction/           # House price regression with MLflow tracking
├── Wine Quality Prediction/          # Wine quality classification with MLflow tracking
├── requirements.txt                  # Python dependencies
├── .gitignore
└── README.md
```

---

## 📌 What This Repository Covers

- **Experiment Tracking** – Log parameters, metrics, and artifacts across runs
- **Model Logging & Registry** – Save, version, and reload trained scikit-learn models
- **MLflow UI** – Visualize and compare runs via the built-in dashboard
- **End-to-End Pipelines** – Full ML workflows from data prep to tracked inference
- **Real-World Projects** – Applied examples on housing and wine quality datasets

---

## 🧩 Projects

### `basics/basics.ipynb`
A guided introduction to MLflow fundamentals:
- Creating and managing experiments
- Logging hyperparameters with `mlflow.log_param()`
- Logging evaluation metrics with `mlflow.log_metric()`
- Saving and loading models with `mlflow.sklearn.log_model()` / `mlflow.sklearn.load_model()`
- Navigating the MLflow Tracking UI

---

### `House Price Prediction/`
An end-to-end regression pipeline for predicting house prices:
- Data preprocessing with **pandas** and **NumPy**
- Model training with **scikit-learn** regression models
- Full MLflow experiment tracking (parameters, metrics, artifacts)
- Model loading and inference from the MLflow model registry

---

### `Wine Quality Prediction/`
A classification pipeline for predicting wine quality scores:
- Feature engineering 
- Model training with scikit-learn classifiers
- MLflow run tracking with metrics comparison across experiments
- Model versioning and prediction from the MLflow registry

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

### Dependencies

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

2. Open and run notebooks in order:
   - `basics/basics.ipynb` — Start here for a guided MLflow introduction
   - `House Price Prediction/` — Regression pipeline with full tracking
   - `Wine Quality Prediction/` — Classification pipeline with run comparison

---

## 📊 Launching the MLflow UI

After running any notebook, visualize logged experiments in the browser:

```bash
mlflow ui
```

Open: [http://localhost:5000](http://localhost:5000)

---

## 🛠️ Key MLflow API Reference

| Function | Description |
|---|---|
| `mlflow.start_run()` | Starts a new experiment run |
| `mlflow.log_param()` | Logs a single hyperparameter |
| `mlflow.log_metric()` | Logs an evaluation metric |
| `mlflow.sklearn.log_model()` | Saves a scikit-learn model as an artifact |
| `mlflow.sklearn.load_model()` | Loads a saved model for inference |
| `mlflow.set_experiment()` | Sets the active experiment by name |

---

## 👤 Author

**Somesh Salunkhe**  
[GitHub](https://github.com/Somesh-Salunkhe)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
