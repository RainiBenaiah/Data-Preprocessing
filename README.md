# Project Overview
This project focuses on predicting customer spending behavior based on transaction data, social engagement, and behavioral insights. We preprocessed, cleaned, and engineered features from multiple datasets, then trained Machine Learning models (Linear Regression and XGBoost) to predict purchase amounts.


# Project Structure
```
data_preprocessing/
├── datasets/
│   ├── copy_1.csv
│   ├── copy_2.csv
│   ├── customer_transactions_augmented.csv
│   ├── final_customer_data_pld14.csv
│   └── final_dataset_ready_pld14.csv
└── datapreprocessing_1.ipynb

models/
├── best_customer_spending_model.pkl
├── customer_spending_prediction.ipynb
└── sample_predictions.csv

README.md
```


# Setup Instructions

## 1. Install Dependencies
Ensure you have Python installed (>= 3.8). Install the required libraries.

## 2. Run Data Preprocessing
Open datapreprocessing_1.ipynb in Jupyter Notebook and run all cells. This will:
 - Merge transaction and social media data.
 - Clean, transform, and engineer features.
 - Save the final dataset as final_dataset_ready_pld14.csv.

## 3. Train the Machine Learning Model
Open customer_spending_prediction.ipynb and run all cells to:
 -  Load the preprocessed dataset.
 -  Train Linear Regression & XGBoost models.
 - Evaluate and compare performance.
 - Save the best model (best_customer_spending_model.pkl).

## 4. View Sample Predictions
After training, sample predictions are saved in sample_predictions.csv.
Run the visualization function inside customer_spending_prediction.ipynb to compare Actual vs. Predicted values.


# Model Performance Summary
| Model               | MAE   | MSE   | RMSE  | R² Score |
|---------------------|-------|-------|-------|----------|
| Linear Regression   | 0.0794| 0.0117| 0.1081| 0.8022   |
| XGBoost             | 0.0523| 0.0070| 0.0838| 0.8809   |

XGBoost performed better with an R² score of 88.09%, meaning it explains a larger variance in customer spending.


# Key Insights & Challenges

## What We Did
1. Merged transaction data with customer social profiles.
2. Engineered behavioral features like rolling averages, engagement scores, and sentiment analysis.
3. Handled missing values & inconsistencies.
4. Trained two models and selected the best.
5. Visualized actual vs. predicted spending patterns.

## Challenges Faced & Solutions
1. Complex Data Merging
Solution: Resolved duplicate IDs and inconsistent mappings by ensuring unique keys.

2. Parsing DateTime Errors
Solution: Standardized date formats and handled time inconsistencies.

3. Feature Selection Confusion
Solution: Used correlation analysis and feature importance techniques.


# Future Improvements
1. Hyperparameter tuning for better model performance.
2. Deep Learning models for improved predictions.
3. Deploy as an API or integrate into a business dashboard.


# Link to Report

# Link to Demo Video
