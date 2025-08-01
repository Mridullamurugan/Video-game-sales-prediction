# 🎮 Video Game Sales Prediction 📊

This repository contains a Machine Learning project that predicts global sales of video games based on various features such as platform, genre, and publisher. The project is built using Python and is intended to showcase skills in data preprocessing, feature engineering, and supervised learning using regression techniques.

## 📁 Project Structure
├── data/
│ └── vgsales.csv # Dataset used for training and testing
├── notebooks/
│ └── EDA_and_Modeling.ipynb # Jupyter notebook with full workflow
├── models/
│ └── trained_model.pkl # Serialized model (optional)
├── README.md # Project documentation
├── requirements.txt # Python dependencies
└── main.py # Script to load model and make predictions

## 📌 Objective

To build a regression model that can accurately predict the **Global Sales** of a video game using features such as:

- Name
- Platform
- Year of Release
- Genre
- Publisher
- NA Sales, EU Sales, JP Sales, and Other Sales (for feature engineering)

## 📊 Dataset

The dataset used is sourced from [Kaggle's Video Game Sales dataset](https://www.kaggle.com/datasets/gregorut/videogame-sales-with-ratings) and contains over 16,000 entries of video game records.

## 🔍 Features Used

- Categorical encoding for `Platform`, `Genre`, and `Publisher`
- Imputation for missing values (e.g., `Year`, `Publisher`)
- Log transformation and scaling for numerical features
- Train-test split and performance evaluation using metrics like R² and RMSE

## 🧠 Machine Learning Algorithms

- Linear Regression
- Random Forest Regressor
- XGBoost Regressor (optional)
- Cross-validation for performance tuning

## ⚙️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/video-game-sales-prediction.git
   cd video-game-sales-prediction
2. Install dependencies:
  ```bash
  pip install -r requirements.txt
  ```
3. Run the notebook:
  ```bash
  jupyter notebook notebooks/EDA_and_Modeling.ipynb
  ```
4. Or run the main prediction script:
  ```bash
  python main.py
  ```
✅ Results
Model performance (example):

R² Score: 0.89

RMSE: 0.47 (in millions of global units sold)
