# Assignment 3 – Federated Learning Design Principles

This repository contains the implementation and experimentation for **Assignment 3** in a course or project focused on **Federated Learning (FL) Design Principles**. The notebook focuses on temperature prediction using a graph-based approach and federated learning setup.

## 📁 Files

- `Assignment_3_FLDesignPrinciple.ipynb`: Main Jupyter notebook with all code, data processing, model training, and results.
- `FMI_data_2025.csv`: Dataset containing weather station data used in the project.

## 📊 Dataset Description

The dataset includes weather data for different stations across six days. Each row in the dataset includes:

- `Name`: Name of the weather station
- `Latitude`, `Longitude`: Geographical coordinates of the station
- `Tmax`, `Tmin`: Max/min temperatures over the past five days (used as features)
- `y_Tmax`: Max temperature on the sixth day (target label)
- `y_Tmin`: Min temperature on the sixth day (can be used optionally)

Each station acts as a **node in a graph**, and the task is to predict `y_Tmax` using previous `Tmax` and `Tmin` values.

## 🧠 Objective

The goal is to apply federated learning techniques to:

- Process spatial weather data
- Build a graph of weather stations based on location
- Train models in a federated setup without sharing raw data
- Compare performance with centralized learning approaches

## ⚙️ Technologies Used

- Python
- Jupyter Notebook
- NumPy & Pandas
- PyTorch / TensorFlow
- NetworkX (for graph construction)
- Federated Learning frameworks (TFF, PySyft, or custom code)

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

# 2. Install required packages
pip install -r requirements.txt

# 3. Launch Jupyter Notebook
jupyter notebook

# 4. Open the notebook and run all cells
# Open 'Assignment_3_FLDesignPrinciple.ipynb' and execute cells in order



