
# ⚡ Electric Vehicle Population Analysis & Forecasting

This project analyzes and forecasts the adoption of electric vehicles (EVs) using a dataset from Kaggle. It includes exploratory data analysis (EDA), machine learning classification to predict CAFV eligibility, and time series forecasting using Facebook Prophet.

## 📦 Dataset

- **Source**: [Kaggle - Electric Vehicle Population Data](https://www.kaggle.com/datasets/ratikkakkar/electric-vehicle-population-data)
- **File**: `Electric_Vehicle_Population_Data.csv`

The dataset contains information on EV models, types, manufacturers, electric range, and CAFV (Clean Alternative Fuel Vehicle) eligibility status.

## 🧪 Environment & Libraries

The project uses the following Python libraries:

- pandas, numpy, matplotlib, seaborn
- scikit-learn (for ML models and evaluation)
- xgboost
- prophet
- kagglehub

Ensure all dependencies are installed using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost prophet kagglehub
```

## 📊 Project Workflow

### 1. Data Loading & Cleaning
- Downloads the dataset using `kagglehub`
- Removes rows with missing critical information
- Focuses on two key eligibility categories

### 2. Exploratory Data Analysis (EDA)
- Plots distribution of CAFV eligibility
- Shows correlations between `Model Year` and `Electric Range`

### 3. Data Preprocessing
- Label encoding of categorical features
- Standard scaling of numerical inputs
- Train/test split (80/20)

### 4. Classification Models
Four machine learning models were evaluated:

- Random Forest
- Decision Tree
- Support Vector Machine (SVM)
- XGBoost

Each model was assessed based on:
- Accuracy
- Precision
- Recall
- F1 Score

Confusion matrices and metric comparisons were visualized.

### 5. Forecasting EV Adoption (Prophet)
- Aggregates eligible EVs by model year
- Trains Prophet on historical data
- Forecasts future EV adoption for 5 years
- Visualizes trends and components

## 📈 Sample Output

- CAFV eligibility bar charts
- Model performance bar plots
- Confusion matrices
- EV adoption forecast through 2030

## 📁 File Structure

```
EV.ipynb                # Main notebook
Electric_Vehicle_Population_Data.csv  # Dataset (downloaded from Kaggle)
README.md               # This file
```

## 🧠 Key Insights

- Random Forest and XGBoost had the best performance for predicting CAFV eligibility.
- Positive trend in EV adoption is expected to continue in coming years.

