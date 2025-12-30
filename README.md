# Kaggle-Playground-Series-Season-5-Episode-12

## 🎯 Project Goal  
### **Diabetes Prediction Challenge**  
The primary objective of this project is to develop a classification model that predicts the probability of a patient being diagnosed with diabetes. The project was developed using data from the "Kaggle Playground Series" Season 5, Episode 12. The dataset is designed for diabetes risk prediction, analysis, and machine learning applications.

## 📦 Methodology and Steps
The project was structured following an end-to-end data science workflow:

1.  **Data Analysis and Visualization:**

    - Checked for unique values and missing data
    - Examine the target distribution to see whether there is any class imbalance and what techniques to use.
    - Analysed the relationship between the numerical features and the target variable to identify multicollinearity and highlight features with strong correlation with the target.
    - Analysed the feature distribution using KDE plots to identify skewed distribution amongst the features and compare with the train and test datasets.
    - To conduct further investigation into skewed plots, we used boxplots to look for actual outliers and figure out the next strategy.
    - Plotted skewed features with their non-linear transformation to see if there is any difference between the plots and if the non-linear transformation leads to a normal distribution.

- **Optuna Study:** Find the best hyperparameters for the XGBoost model
  
## Libraries and Tools Used
-   Python
-   Pandas & NumPy
-   Scikit-learn (`train_test_split`, `StratifiedKFold`, `metrics`)
-   **XGBoost**
-   Jupyter Notebook
