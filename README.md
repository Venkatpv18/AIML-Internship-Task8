## Decision Tree: Bank Marketing Subscription Prediction

## Task Overview
This task focuses on building a **Decision Tree classification model** to predict whether a bank customer will subscribe to a **term deposit** based on demographic, financial, and campaign-related features.

The goal of this task is to gain hands-on experience with an **interpretable machine learning model** and understand customer subscription behavior.


##  Dataset Description
- **Dataset Name:** Bank Marketing Dataset  
- **Source:** Kaggle (UCI Bank Marketing – bank-full.csv)  
- **Total Records:** 45,211  
- **Features:** 16 input attributes (categorical and numerical)  
- **Target Variable:**  
  - `y` → Indicates whether the customer subscribed to the term deposit (`yes` / `no`)

## 🛠 Tools & Technologies Used
- Python  
- Google Colab  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  

---

## Methodology
The following steps were followed to complete the task:

1. **Dataset Loading**  
   The dataset was downloaded using KaggleHub and loaded into a Pandas DataFrame.

2. **Data Preprocessing**  
   - Replaced `unknown` values with missing values  
   - Filled missing categorical values using mode  
   - Renamed the target column for consistency  

3. **Feature Encoding**  
   - Categorical features were encoded using **OneHotEncoding**  
   - Numerical features were passed directly  

4. **Train–Test Split**  
   - Data was split into training and testing sets  
   - A fixed `random_state` was used for reproducibility  

5. **Model Training**  
   - A **Decision Tree Classifier** was trained  
   - Tree depth was limited using `max_depth` to avoid overfitting  

6. **Model Visualization**  
   - The trained decision tree was visualized for interpretability  

7. **Model Evaluation**  
   - Predictions were made on test data  
   - Classification report and accuracy scores were generated  
   - Training and testing accuracy were compared  

8. **Rule Extraction**  
   - Decision rules were extracted from the tree  

## Results & Observations
- **Call duration** was the most influential feature.  
- Customers with **successful previous campaigns** showed a higher subscription rate.  
- Very short call durations usually resulted in non-subscription.  
- Training and testing accuracy were close, indicating reduced overfitting.

---

## Key Decision Rules
1. Customers with **longer call durations** are more likely to subscribe.  
2. A **successful previous campaign outcome** increases subscription probability.  
3. Short call durations combined with unsuccessful past outcomes generally lead to non-subscription.

---

## Deliverables
- Google Colab Notebook  
- Decision Tree Visualization Image  
- Classification Report  
- Accuracy Comparison  
- Extracted Decision Rules  

---

## Learning Outcome
This task helped in understanding:
- Decision Tree classification  
- Handling categorical data  
- Model interpretability  
- Overfitting control using tree depth  

---

## Conclusion
This task demonstrates how **Decision Trees** can be effectively used for transparent and explainable predictions in real-world business problems such as customer marketing and subscription prediction.
