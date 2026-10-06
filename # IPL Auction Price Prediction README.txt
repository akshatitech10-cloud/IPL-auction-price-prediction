# IPL Auction Price Prediction

A machine learning regression project to predict IPL player auction prices using player performance and career statistics.

## 📌 Project Overview

This project uses historical IPL player data to predict the auction price of players based on their batting, bowling, experience, and other performance-related attributes.

## 📊 Dataset

- **Records:** 130 IPL players
- **Target Variable:** `SOLD PRICE`
- **Features:** Player age, playing role, batting and bowling statistics, international experience, captaincy experience, and other performance indicators.

The dataset contains player statistics and auction-related information from IPL auctions.

## 🔍 Exploratory Data Analysis

- Analyzed the distribution of IPL auction prices.
- Studied the relationship between player performance and auction price.
- Compared average auction prices across different playing roles.
- Examined batting and bowling statistics in relation to auction prices.

## ⚙️ Data Preprocessing

- Inspected the dataset for missing values and data inconsistencies.
- Removed identifier and potentially irrelevant columns.
- Applied categorical encoding to player-related categorical variables.
- Handled numerical outliers using IQR-based capping.
- Applied log transformation to the target variable to reduce skewness.
- Standardized numerical features using `StandardScaler`.
- Used an **80:20 train-test split** for model evaluation.

## 🤖 Models Used

- Linear Regression
- Ridge Regression

Ridge Regression was further optimized using cross-validation to select the best regularization parameter.

## 📈 Model Evaluation

Models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Ridge Regression Results

- **MAE:** 164,881.56
- **RMSE:** 227,371.47
- **R²:** 0.620
- **Best Alpha:** 100

Ridge Regression outperformed the baseline Linear Regression model on the test set.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## 📁 Files

- `IPL_Auction_Price_Prediction.ipynb` — Complete data analysis, preprocessing, model training, and evaluation
- `README.md` — Project documentation
- `requirements.txt` — Required Python libraries

## ▶️ How to Run

1. Download or clone this repository.
2. Install the required libraries:

```bash
pip install -r requirements.txt