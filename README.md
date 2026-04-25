# 🧪 MLflow Experiment Tracking

A hands-on repository demonstrating how to use **MLflow** for experiment tracking, model logging, and end-to-end ML pipelines. Projects span foundational concepts to real-world prediction tasks including house price regression and wine quality prediction using a deep learning model.

---

## 📁 Repository Structure

```
ML-Flow/
├── basics/
│   └── basics.ipynb                             # Introduction to MLflow core concepts
├── House Price Prediction/                      # House price regression with MLflow tracking
├── Wine Quality Prediction/
│   └── Wine_Quality_Prediction_With_ANN.ipynb   # ANN-based wine quality prediction with MLflow
├── requirements.txt                             # Python dependencies
├── .gitignore
└── README.md
```

---

## 📌 What This Repository Covers

- **Experiment Tracking** – Log parameters, metrics, and artifacts across runs
- **Model Logging & Registry** – Save, version, and reload trained models
- **MLflow UI** – Visualize and compare runs via the built-in dashboard
- **End-to-End Pipelines** – Full ML workflows from data preparation to tracked inference
- **Deep Learning Integration** – MLflow tracking with Keras/TensorFlow ANN models

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
A deep learning pipeline for predicting wine quality scores using an **Artificial Neural Network (ANN)**:
- Data preprocessing 
- ANN model built with **Keras (TensorFlow backend)**
- MLflow run tracking for epochs, loss, and evaluation metrics
- Model versioning and reloading via the MLflow registry

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
| `scikit-learn` | ML model training (house price) |
| `tensorflow` / `keras` | ANN model for wine quality prediction |
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
   - `Wine Quality Prediction/Wine_Quality_Prediction_With_ANN.ipynb` — ANN pipeline with Keras and MLflow

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
| `mlflow.tensorflow.log_model()` | Saves a Keras/TensorFlow model as an artifact |
| `mlflow.set_experiment()` | Sets the active experiment by name |

---

## 👤 Author

**Somesh Salunkhe**  
[GitHub](https://github.com/Somesh-Salunkhe)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
