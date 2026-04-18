# california-housing-regression
Regression analysis on the California Housing dataset using Linear Regression and Decision Tree Regressor with preprocessing, feature scaling, and model evaluation using MSE, MAE and R² metrics. Built with Python and Scikit-learn.
# Objective
To evaluate understanding of regression techniques in supervised learning by applying them to the California Housing dataset.
# Dataset
* Source: California Housing Dataset from sklearn.datasets
* Size: 20,640 samples, 8 features
* Target: Median House Value (in $100,000s)
  
# Features
| Feature    | Description                 |
|------------|-----------------------------|
| MedInc     | Median income of households |
| HouseAge   | Median age of houses        |
| AveRooms   | Average number of rooms     |
| AveBedrms  | Average number of bedrooms  |
| Population | Block population            |
| AveOccup   | Average house occupancy     |
| Latitude   | Geographic latitude         |
| Longitude  | Geographic longitude        |

# Libraries Used
numpy, pandas, matplotlib, seaborn, scikit-learn

# Project Structute
```
├── Regression_Assignment.ipynb   # Main notebook
└── README.md                     # Project description
```
# Steps Performed
**1. Loading & Preprocessing**

* Loaded dataset using fetch_california_housing()
* Converted to pandas DataFrame
* Checked and confirmed zero missing values
* Applied StandardScaler for feature standardization
* Split data into 80% train and 20% test sets

**2. Models Implemented**

* Linear Regression — baseline model using equation y = m₁x₁ + m₂x₂ + ... + m₈x₈ + c
* Decision Tree Regressor — captures non-linear relationships using yes/no splits

**3. Evaluation Metrics**

* Mean Squared Error (MSE)
* Mean Absolute Error (MAE)
* R² Score

# Results
|Model            | MSE    | MAE    | R²     |
|-----------------|--------|--------|--------|
|Linear Regression| 0.5559 | 0.5332 | 0.5758 |
|Decision Tree    | 0.4940 | 0.4539 | 0.6230 |

# Conclusion
Decision Tree outperformed Linear Regression across all metrics with a higher R² of 0.6230, as it captures non-linear relationships in housing data. Linear Regression struggled due to its assumption of a straight line relationship between features and prices.

# How to Run
1. Clone the repository
2. Open Regression_Assignment.ipynb in Jupyter Notebook
3. Run all cells sequentially
