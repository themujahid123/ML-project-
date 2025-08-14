# ML-project-  
## 📄 Project: Classification Model Comparison  

-**Objective:** Predict the target variable using multiple models, compare their performance, and identify the best approach.  

##Data Preparation

-Import libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`.  
-Load dataset → checked data types, missing values, and class distribution.  
-Encoding: Applied label encoding / one-hot encoding where needed.  
-Train-test split: 80% training, 20% testing using `train_test_split(random_state=42)`.  

### Model Comparison Conclusion   

We trained and compared three classification models — Logistic Regression, Decision Tree, and Dummy Classifier — to predict the target variable.

- **Logistic Regression (C=1)** delivered the highest test accuracy (**85%**), with balanced precision, recall, and F1-scores across classes.
- **Decision Tree** achieved 79% accuracy but showed signs of overfitting (100% train accuracy vs. lower test accuracy).
- **Dummy Classifier** served as a baseline (53% accuracy), confirming that both main models significantly outperformed random/majority prediction.

**Key Takeaway:** Logistic Regression with proper regularization provided the best trade-off between accuracy and generalization, making it the recommended model for deployment.
