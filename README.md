# 🌤️ Seattle Weather Temperature Prediction

A clean and engaging weather forecasting project that predicts the mean temperature for Seattle using historical weather data and a machine learning model.

<p align="center">
  <img src="https://images.unsplash.com/photo-1504608524841-42fe6f032b4b?auto=format&fit=crop&w=1200&q=80" alt="Weather landscape" width="100%" />
</p>

## ✨ Overview

This project uses the `seattle-weather.csv` dataset to build a temperature prediction model. It analyzes weather patterns over time, engineers useful features, trains a `LinearRegression` model, and evaluates its performance using key metrics such as MAE and RMSE.

The notebook includes:
- Date feature extraction (`Year`, `Month`, `Day`)
- Mean temperature feature engineering
- Train/test splitting for time-based evaluation
- Model training and prediction
- Visualization of actual vs predicted temperatures
- Residual analysis and future temperature forecasting

---

## 📊 Dataset

The project uses a weather dataset containing the following fields:

- `date`
- `precipitation`
- `temp_max`
- `temp_min`
- `wind`

From this data, the notebook creates a new target variable:

- `meantemp = (temp_max + temp_min) / 2`

This allows the model to predict daily average temperature more effectively.

---

## 🧠 Model and Methodology

### Features Used
- `Year`
- `Month`
- `Day`
- `precipitation`
- `wind`

### Target
- `meantemp`

### Algorithm
- `LinearRegression`

### Evaluation Metrics
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

### Workflow
1. Load the dataset
2. Convert date fields into useful features
3. Create mean temperature
4. Split data into training and testing sets
5. Train the regression model
6. Predict on unseen test data
7. Visualize performance and residuals
8. Forecast future temperature values

---

## 📈 Visualizations Included

The notebook produces multiple useful charts:

- Temperature trend over time
- Actual vs predicted temperature plot
- Scatter plot of actual vs predicted values
- Residual error plot

These plots help you understand how the model performs and where it may be under- or over-predicting.

---

## 🗂️ Project Structure

```text
Weather-Temperature-Prediction/
├── README.md
├── seattle-weather.csv
├── Weather_Forecasting_Model.ipynb
└── .git/
```

---

## 🚀 Getting Started

### 1. Clone the project

```bash
git clone <repository-url>
cd Weather-Temperature-Prediction
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib scikit-learn
```

### 3. Open the notebook

Run the Jupyter notebook:

```bash
jupyter notebook Weather_Forecasting_Model.ipynb
```

> If you are using Google Colab, upload the dataset and run the notebook cells there.

---

## 🔎 Example Output

The notebook prints model performance such as:

```text
MODEL PERFORMANCE
Mean Absolute Error (MAE) : 2.75
Root Mean Squared Error (RMSE) : 3.41
```

It also forecasts future temperature values, for example:

```text
FUTURE PREDICTION
Date : 20-08-2026
Predicted Mean Temperature : 18.12 °C
```

---

## 🛠️ Requirements

- Python 3.x
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- scikit-learn

---

## 💡 Possible Improvements

- Use a time-series model such as Random Forest Regressor, XGBoost, or LSTM
- Add seasonal features and lag-based variables
- Improve forecasting by using long-term historical data
- Deploy the model as a small web app or REST API

---

## 🤝 Contributing

Contributions are welcome! If you want to improve the model, enhance the notebook visuals, or add a better forecasting pipeline, feel free to open a pull request.

---

## ✅ Summary

This project is a simple yet effective introduction to weather forecasting with machine learning. It demonstrates how historical data can be transformed into meaningful features, how regression models can learn patterns, and how predictions can be evaluated visually and numerically.

If you want, I can also help you make the README even more polished with:
- a project logo section
- badges for accuracy metrics
- a screenshot gallery
- a more professional technical documentation style
