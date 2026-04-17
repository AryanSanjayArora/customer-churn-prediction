# Customer Churn Prediction Project

## Overview
This project focuses on developing a machine learning model to predict customer churn. The goal is to identify customers who are likely to stop using a service, enabling proactive retention efforts. The workflow, from data exploration to model evaluation, is implemented in a Jupyter Notebook using Python and popular data science libraries.

## Motivation
Retaining existing customers is often more cost-effective than acquiring new ones. By building an accurate churn prediction model, businesses can:

* Identify at-risk customers.
* Implement targeted retention strategies.
* Reduce customer attrition.
* Improve overall business profitability.
  
## Jupyter Notebook (`Customer_Churn_Prediction.ipynb`)

The notebook covers the following stages:

1. **Data Loading and Exploration**  
   - Load dataset and perform initial exploratory analysis.  
   - Visualize churn distribution and check missing values.  

2. **Data Preprocessing**  
   - Handle missing values (e.g., imputation for `TotalCharges`).  
   - Encode categorical features using Label Encoding and One-Hot Encoding.  
   - Scale numerical features with StandardScaler.  

3. **Feature Engineering**  
   - Group customer tenure into categories.  
   - Create new features to improve model performance.  

4. **Exploratory Data Analysis (EDA)**  
   - Churn distribution across gender, contract type, monthly charges.  
   - Correlation heatmap of numerical features.  

5. **Model Selection and Training**  
   - Logistic Regression  
   - Random Forest Classifier  
   - Gradient Boosting Classifier  

6. **Model Evaluation**  
   - Accuracy, Precision, Recall, F1-Score  
   - Confusion Matrix (visualized as heatmaps)  
   - Feature Importance (tree-based models)  

7. **Model Comparison Table**  
   - Summarizes performance metrics of all models in one place.  

8. **Hyperparameter Tuning**  
   - GridSearchCV applied to Random Forest for optimization.  

9. **Cross-Validation**  
   - Validates model stability with k-fold CV.  

10. **Visualization of Results**  
    - Confusion matrices, feature importance plots, correlation heatmap, EDA charts.
   
## Key Findings
* The **Gradient Boosting Classifier** achieved the highest accuracy (~85%).  
* Key features influencing churn include **contract type, tenure, and monthly charges**.  
* The comparison table clearly shows differences in model performance.  

## Technical Skills Demonstrated
* Python, Pandas, NumPy  
* Scikit-learn (ML algorithms, preprocessing, evaluation)  
* Matplotlib, Seaborn (visualizations)  
* Jupyter Notebook  
* Feature Engineering  
* Model Selection & Training  
* Model Evaluation (Classification Metrics, Confusion Matrix, F1-Score)  
* Hyperparameter Tuning & Cross-Validation  

## How to Run the Code
1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/customer-churn-prediction.git

## Create a virtual environment and install dependencies:
python -m venv venv
source venv/bin/activate   # macOS/Linux
venv\Scripts\activate      # Windows
pip install -r requirements.txt

Run the notebook:
jupyter notebook Customer_Churn_Prediction.ipynb


---

### ✂️ Step 5: Dataset Description
```markdown
## Dataset

This project uses the **Customer_churn** (commonly available on Kaggle).  
It contains information about customer demographics, contract details, billing, and service usage.  

- **Target Variable:** `Churn` (Yes/No)  
- **Key Features:**  
  - `gender` – Male/Female  
  - `tenure` – Number of months the customer has stayed  
  - `Contract` – Type of contract (Month-to-month, One year, Two year)  
  - `MonthlyCharges` – Amount charged per month  
  - `TotalCharges` – Total amount charged  
  - `PaymentMethod` – Payment type (Electronic check, Credit card, etc.)  

These features are used to train machine learning models that predict whether a customer is likely to churn.


