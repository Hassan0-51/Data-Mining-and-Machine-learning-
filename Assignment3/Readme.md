
# Assignment 3

## Overview
This assignment focuses on car price prediction using machine learning techniques. It involves data preprocessing, model training, and evaluation to identify the best-performing model for predicting car prices.

## Dataset Description
The dataset used in this assignment is **car_price_prediction_.csv**. It consists of **2,500 entries** and **10 columns** related to car attributes. The key features include:
- **Car ID**: Unique identifier (removed during preprocessing)
- **Brand**: The car's manufacturer (e.g., Tesla, BMW, Audi)
- **Year**: Manufacturing year
- **Engine Size**: Size of the engine in liters
- **Fuel Type**: Type of fuel (Petrol, Diesel, Electric)
- **Transmission**: Type of transmission (Manual, Automatic)
- **Mileage**: Total distance traveled by the car (in km)
- **Condition**: Car condition (New, Used, Like New)
- **Model**: Specific model of the car
- **Price**: Target variable (car price in dollars)

## Tasks Performed
- **Task 1: Data Loading and Preprocessing**  
  - Loaded the dataset using pandas.  
  - Removed irrelevant features (e.g., Car ID).  
  - Encoded categorical variables using one-hot encoding.  
  - Split the data into training and testing sets (80-20 split).

- **Task 2: Model Implementation and Training**  
  - Implemented multiple regression models, including:
    - **Linear Regression (all features included).**  
    - **Backward Elimination (feature selection based on p-values).**  
  - Used `sklearn` and `statsmodels` for training and evaluation.

- **Task 3: Model Evaluation and Performance Analysis**  
  - Measured model accuracy using R² score.  
  - Compared models to determine the impact of feature selection.  
  - Evaluated feature significance using p-values from OLS regression.

## Results and Output
The results of the assignment include:
- The **Linear Regression model** with all features achieved an R² score of **0.85**.
- The **Backward Elimination model** achieved an R² score of **0.83**.
- The most significant features (with the lowest p-values) were **0.0001, 0.0023, 0.0156, 0.0489, 0.0521**.
- Feature selection helped in identifying the most influential variables affecting car prices.

## Conclusion
From this assignment, we conclude that:
- **Feature selection** (Backward Elimination) helps in improving model interpretability without significantly reducing accuracy.
- **Data preprocessing**, including encoding categorical variables, plays a crucial role in achieving better predictions.
- **Linear Regression** provides a good baseline for car price prediction, and further improvements can be made with feature engineering and advanced models.

## Requirements
- Python 3.x
- Jupyter Notebook
- Libraries: pandas, numpy, sklearn, statsmodels, matplotlib

## How to Run
1. Open the notebook in Jupyter:
   ```bash
   jupyter notebook assignment3.ipynb
   ```
2. Run each cell sequentially to execute the assignment steps.

## Author
 Hassan Ali

