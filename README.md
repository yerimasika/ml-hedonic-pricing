# Aircraft Price Prediction

This repository presents an applied **data science and machine learning project** focused on predicting aircraft prices based on their technical and performance characteristics.  
The project follows a structured, end-to-end approach combining exploratory data analysis, preprocessing, and multiple regression models.

It was developed as part of a **Master’s degree in Data Science and Economics** at Université Paris Nanterre.

---

## Project Objective

Aircraft prices are influenced by a wide range of technical attributes such as engine power, speed, range, weight, and operational performance.  
The goal of this project is to **model and predict aircraft prices** using these characteristics, while balancing **predictive performance and interpretability**, in line with the economic theory of **hedonic pricing**.

---

## Dataset

- **Observations**: 517 aircraft  
- **Target variable**: Aircraft price (USD)  
- **Features**:
  - Engine characteristics (type, power)
  - Speeds (max, cruise, stall)
  - Operational performance (takeoff & landing distances, climb rates)
  - Structural variables (length, wingspan, empty weight)
  - Fuel capacity and range

Some aircraft prices are missing and are later predicted using the trained models.

---

## Methodology

### 1. Exploratory Data Analysis
- Distribution analysis
- Detection of asymmetries and outliers
- Identification of structural heterogeneity across aircraft categories

### 2. Data Preprocessing
- Log-transformations for highly skewed variables
- Standardization of numerical features
- Categorical encoding for engine type
- Pipeline-based preprocessing to avoid data leakage

### 3. Models Implemented
- Linear Regression (baseline)
- Ridge Regression (L2 regularization)
- Lasso Regression (L1 regularization & feature selection)
- Polynomial Regression
- Neural Network (MLP)

### 4. Evaluation
Models are compared using:
- Mean Squared Error (MSE)
- R² score  
on a held-out test set (80/20 split).

---

## Key Results

- Linear and penalized regression models perform strongly, with **R² ≈ 0.8**
- Regularization improves stability in the presence of multicollinearity
- More complex models (high-degree polynomial, neural network) do not significantly outperform simpler approaches
- Operational performance variables (range, climb rate, cruise speed) are the most influential price drivers

---

## Technologies Used

- Python
- Pandas / NumPy
- Scikit-learn
- Matplotlib / Seaborn
- TensorFlow / Keras
- Jupyter Notebook

---

## Repository Structure
```
├── code/aircraft.ipynb        # Main notebook (EDA, modeling, evaluation)
├── report.pdf            # Full project report
├── data/                 # Dataset (if included)
└── README.md
```


---

## Why This Project Matters

This project demonstrates:
- A rigorous **end-to-end ML workflow**
- The ability to connect **economic theory** with **machine learning**
- Strong emphasis on **interpretability, robustness, and practical relevance**

It reflects my interest in applying data science to real-world valuation and decision-making problems.

---

## Author

**Sika**  
Data Scientist | Applied Machine Learning  

You can find more of my work on my GitHub profile.

---

## Notes

This repository is shared for educational and portfolio purposes.  
Feedback and discussions are welcome.
