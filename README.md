# 🌐 Federated Learning on Weather Station Data

This project implements a **Federated Learning** approach to predict temperature using data collected from multiple weather stations (e.g., station 7790 and 7761). The main goal is to collaboratively train models across decentralized datasets **without sharing raw data**, thus preserving data **privacy** and **locality**.

---

## 🚀 Features

- 🔐 **Federated Learning Setup**  
  Simulated client environments where data remains local; only model updates are exchanged.

- 📊 **Regression Task**  
  Target: Predict **temperature (Température °C)** using various environmental features.

- 🤖 **Local Model Training**  
  Linear Regression used per client. Can be extended to **XGBoost**, **Neural Networks**, etc.

- 🔁 **Model Aggregation**  
  A central server performs **FedAvg (Federated Averaging)** to combine client model parameters.

- 📈 **Evaluation Metrics**  
  - MAE (Mean Absolute Error)  
  - RMSE (Root Mean Squared Error)  
  - R² (Coefficient of Determination)  
  - MAPE (Mean Absolute Percentage Error)  
  - EVS (Explained Variance Score)

- 🧹 **Data Handling**  
  - Missing value imputation  
  - Normalization with `MinMaxScaler`  
  - Separate train/validation/test splits per station

---

## 🏗️ Tech Stack

- **Python**: Core language for logic and modeling  
- **Libraries**:
  - `pandas`, `numpy`, `scikit-learn` for data manipulation and ML
  - `matplotlib`, `seaborn` for visualization
- **Development Tools**:
  - Jupyter Notebook / Python scripts

### Extensions
- `xgboost`, `tensorflow`, or `pytorch`
- **Federated frameworks**: Flower, TensorFlow Federated for real-world FL setups



## 📌 How to Run
### Clone the repository:

```bash
git clone https://github.com/AlperErd0gan/Federated-Learning-on-Weather-Station-Data.git
cd Federated-Learning-on-Weather-Station-Data
```
### (Optional) Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

```
### Install dependencies:
```bash
pip install -r requirements.txt
```




## 📬 Contributing
Feel free to fork the repo, open issues, or submit pull requests if you'd like to contribute or improve this project!