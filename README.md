# house_price_prediction
First project, predicts the House price
<br>

## Objective
The goal of this project is to build predictive models that can accurately estimate house prices based on various features like size, location, quality, garage type, etc. The key focus is on:
- Learning how different regression techniques work
- Understanding regularization (Ridge and Lasso)
- Comparing model performance using evaluation metrics
- Interpreting model coefficients to understand feature importance
---
## Model used
- **Linear Regression** => Base model to fit data without regularization
- **Ridge Regression** => Regularized linear regression (L2 penalty) to handle multicollinearity
- **Lasso Regression** => Regularized linear regression (L1 penalty) to perform feature selection
- **Decision Tree Regressor** => Non-linear model that splits data hierarchically
---
## Evaluation Matrics
- **R² Score** (Accuracy)
- **RMSE** (Root Mean Squared Error)
---
## Tools
- Python
- Numpy , Pandas
- Scikit-learn
- Jupyter Notebook
---
## Dataset
- Dataset: **Ames Housing Dataset** from kaggle
- Features: 80+ features(numeric & categorical)
- Target: `SalePrice` (house price)
---
## Key Steps
1) **Data Cleaning & Preprocessing**
   - Removed columns with too many nulls
   - Handled missing values
   - Encoded categorical variables using One-Hot Encoding
   - Feature scaling (if needed)
2) **Model Training**
   - Split into train/test using `train_test_split`
   - Trained all 4 models
   - Compared R² scores and RMSE
3) **Coefficient Analysis**
    - Visualized top features from Linear, Ridge, and Lasso
    - Observed how Lasso reduces less important features' coefficients to zero
4) **Feature Importance (Decision Tree)**
   - Extracted and plotted top 10 features based on impurity reduction
---
# Results
  | Model              | R² Score        |
  |--------------------|-----------------|
  | Linear Regression  |    0.9092       |
  | Ridge Regression   |    0.8823       |
  | Lasso Regression   |    0.9092       |
  | Decision Tree      |    0.8079       |

  >Lasso performed similar to Linear, while Ridge slightly underperformed. Decision Tree was bad to overfitting on deeper depths.
## Learnings
  - How different regression models behave on real-world data
  - How to interpret and visualize model coefficients
  - Decision Trees can overfit if not properly tuned
  - Importance of regularization in model generalization

## 🧑‍💻 Author
  Atharva Joshi  
  *2nd year B.Tech in Chemical Engineering*  
  *IIT Hyderabad*
