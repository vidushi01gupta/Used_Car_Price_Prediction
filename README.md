# 🚗 Used Car Price Prediction

A machine learning project that predicts the **selling price of used cars** based on features such as brand, model, model year, mileage, fuel type, engine type, transmission, colors, accident history, and clean-title status.

The project uses **Multiple Linear Regression** to estimate the expected market price of a used vehicle.

---

## 📌 Project Overview

Buying or selling a used car can be difficult because the price depends on many factors.

This project aims to build a regression model that can predict a car's price using historical used-car data.

### Business Objective

> Predict the expected market price of a used car based on its specifications and condition.

---

## 📊 Dataset

The dataset contains approximately **4,000 used-car records**.

### Features

| Feature            | Description                           |
| ------------------ | ------------------------------------- |
| `Brand`            | Manufacturer of the vehicle           |
| `Model`            | Vehicle model                         |
| `Model_Year`       | Manufacturing/model year              |
| `Milage`           | Vehicle mileage in miles              |
| `Fuel_Type`        | Type of fuel used                     |
| `Engine_Type`      | Engine specification                  |
| `Transmission`     | Transmission type                     |
| `Exterior_Color`   | Exterior color                        |
| `Interior_Color`   | Interior color                        |
| `Accident_History` | Accident/damage history               |
| `Clean_Title`      | Whether the vehicle has a clean title |
| `Price`            | Target variable — vehicle price       |

---

## 🔍 Exploratory Data Analysis

The following EDA steps were performed:

* Dataset shape and structure
* Statistical summary
* Data types
* Missing-value analysis
* Duplicate-value analysis
* Unique-value analysis
* Categorical feature analysis
* Target variable distribution
* Outlier analysis
* Relationship between numerical features and price

---

## 🧹 Data Preprocessing

The following preprocessing techniques were applied:

* Renamed columns for consistency
* Handled missing values
* Converted mileage from string format to numeric
* Cleaned the price column
* Replaced missing categorical values with `Unknown`
* Handled inconsistent categorical values
* Grouped rare vehicle models into an `Other` category
* Converted categorical variables using **One-Hot Encoding**
* Split the dataset into training and testing sets

### Train-Test Split

The dataset was divided into:

* **80% Training Data**
* **20% Testing Data**

---

## 🤖 Machine Learning Model

### Multiple Linear Regression

The primary model used in this project is:

**Multiple Linear Regression**

The model attempts to learn the relationship between the input features and the vehicle price.

---

## 📈 Model Evaluation

The regression model was evaluated using:

### Mean Absolute Error (MAE)

Measures the average absolute difference between actual and predicted prices.

### Mean Squared Error (MSE)

Measures the average squared difference between actual and predicted prices.

### Root Mean Squared Error (RMSE)

The square root of MSE. It gives the error in the same units as the target variable.

### R² Score

Measures how much of the variation in vehicle prices is explained by the model.

---

## 📊 Results

The model achieved an R² score of approximately:

```text
R² ≈ 0.73
```

The relatively low R² indicates that a simple Multiple Linear Regression model does not capture all the complexity of used-car pricing.

Possible reasons include:

* Highly skewed vehicle prices
* Luxury and high-performance vehicles
* Large variation between vehicle brands and models
* High-cardinality categorical variables
* Non-linear relationships between features and price
* Outliers in the target variable
* Limited number of observations for some vehicle categories

The project focuses on understanding the complete **regression workflow**, including preprocessing, feature engineering, model training, evaluation, residual analysis, and regression assumptions.

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**
* **uv**
* **Git**
* **GitHub**

---

## 📁 Project Structure

```text
Used_Car_Price_Prediction/
│
├── used_car_price_prediction.ipynb
├── used_cars.csv
├── README.md
├── requirements.txt
├── pyproject.toml
├── uv.lock
├── .python-version
└── .gitignore
```

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/vidushi01gupta/Used_Car_Price_Prediction.git
```

### 2. Navigate to the project

```bash
cd Used_Car_Price_Prediction
```

### 3. Create/activate the environment

If you are using `uv`:

```bash
uv sync
```

Then activate the environment:

### Windows

```bash
.venv\Scripts\activate
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Run the notebook

Open:

```text
used_car_price_prediction.ipynb
```

Select the appropriate Python kernel and run the notebook cells from top to bottom.

---

## 🔄 Machine Learning Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Understanding
   ↓
Exploratory Data Analysis
   ↓
Data Cleaning
   ↓
Missing Value Handling
   ↓
Outlier Analysis
   ↓
Feature Engineering
   ↓
Categorical Encoding
   ↓
Train-Test Split
   ↓
Multiple Linear Regression
   ↓
Predictions
   ↓
Model Evaluation
   ↓
Residual Analysis
   ↓
Regression Assumption Analysis
```

---

## 👩‍💻 Author

**Vidushi Gupta**

B.Tech Computer Science Engineering

GitHub:
https://github.com/vidushi01gupta

---

## ⭐ Project

If you find this project useful, consider giving the repository a ⭐ on GitHub.
