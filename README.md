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

2. **Optuna Study:** Find the best hyperparameters for the XGBoost model

3. **Feature Engineering and XGBoost Model:**
   - Applied target encoding using the original dataset and the global mean of the train dataset.
   - Categorical features were converted to a numerical format using count encoding
   - Applied non-linear transformation such as <code>sqrt</code> and <code>log1p</code> to the skewed variables as a feature engineering techniques
   - The train dataset was split using the <code>OOF</code> technique for better generalization and <code>StratifiedKFold</code> for addressing the imbalance target distribution.
   - <code>XGBoostClassifier</code> was selected as the model for this project and used the best parameters achieved from the Optuna study.
  
4. **Results**
   - The model achieved an overall OOF AUC score of <code>0.7295</code>.
   
  
## Libraries and Tools Used
-   Jupyter Notebook
-   Python
-   Pandas & NumPy
-   Seaborn & Matplotlib
-   Scikit-learn (`train_test_split`, `StratifiedKFold`, `metrics`)
-   Optuna
-   **XGBoost**

