# Customer Churn Prediction (ML/DL)

## Overview
Yeh project bank customers ka churn predict karta hai – yaani kaun se customers apni service chhor sakte hain. Business growth, retention aur marketing ke liye yeh insight bohot valuable hai [file:17].

## Objective
Machine Learning aur Deep Learning ka use kar ke binary prediction ki gayi hai: customer exited (churn) karega ya nahi. ANN use hua hai aur accuracy maximize karne ki koshish ki gayi hai [file:17].

## Dataset Description
- **File:** Churn_Modelling.csv
- **Features:** Customer demographics (Age, Gender, Geography), account info (Tenure, Balance, Products, HasCrCard, IsActiveMember), salary aur target label (Exited)
- Data ko pandas se load, explore aur visualize kiya gaya hai, initial EDA mein missing values, unuseful columns drop kiye gaye hain [file:17].

## Methodology

1. **Data Preprocessing**
   - Initial columns (RowNumber, CustomerId, Surname) drop kiye gaye
   - Categorical variables (Geography, Gender) ko One-Hot encoding se numeric banaya
   - Features scale kiye (Standard Scaler)
   - Train-test split (test size = 20%) [file:17]

2. **Model Architecture**
   - Keras Sequential ANN: 2 hidden layers (6 neurons, relu), output layer (1 neuron, sigmoid)
   - Optimizer: Adamax
   - Loss: Binary cross-entropy
   - Epochs: 100 tak train kiya gaya
   - Batch size: 10
   - Validation split: 33% [file:17]

3. **Training & Evaluation**
   - Accuracy aur loss per epoch plot kiye gaye
   - Confusion matrix aur accuracy score calculate kiye: Final accuracy approx **84.7%** on test data [file:17]
   - Metrics: Accuracy, confusion matrix, loss curve

## Results

| Metric         | Value      |
|----------------|------------|
| Test Accuracy  | 84.7% [file:17] |
| Confusion Matrix | [1521, 87], [219, 173] [file:17] |

Model ne achi prediction ki hai churn ke liye. ANN approach is project ke liye effective rahi hai [file:17].

## Project Structure


