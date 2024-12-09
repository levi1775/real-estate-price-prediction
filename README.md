# 🏠 Real Estate Price Prediction

This project focuses on predicting real estate prices using machine learning techniques. The workflow includes detailed **data preprocessing**, **exploratory data analysis (EDA)**, and **model building** to achieve accurate predictions.

---

## 🌟 Project Overview

The dataset consists of approximately **3000 rows** and **274 columns**, capturing a wide range of features. The target variable is **SalePrice**, representing the price of real estate properties. This project leverages advanced preprocessing techniques and Elastic Net regularization to build a robust predictive model.

---

## 🔑 Key Steps

### 1. Data Preprocessing

#### a. **Dealing with Missing Data**
- Identified missing values and categorized them as:
  - **Missing Completely at Random (MCAR)**
  - **Missing Not at Random (MNAR)**
- Used:
  - **Median imputation** for numerical values.
  - **Mode imputation** for categorical values.
- Handled significant missing values (e.g., absence of features like a basement or garage).

#### b. **Dealing with Categorical Data**
- Encoded categorical variables using:
  - **One-Hot Encoding**: For nominal categories.
  - **Ordinal Encoding**: For ordered categories (e.g., quality ratings).
- Ensured compatibility with machine learning by converting all categorical data into numeric format.

#### c. **Dealing with Outliers**
- Identified outliers using statistical methods like **Interquartile Range (IQR)** and visualizations (box plots).
- Applied strategies like capping or removal based on domain knowledge.

---

### 2. Exploratory Data Analysis (EDA)
- Visualized relationships between features and the target variable.
- Detected multicollinearity using heatmaps and correlation matrices.
- Examined numerical feature distributions and applied transformations where necessary.

---

### 3. Feature Engineering
- Added new features to improve model accuracy.
- Removed redundant or highly correlated features to simplify the dataset.

---

### 4. 🤖 Model Building

#### a.  **Scaling**
- Standardized features using **StandardScaler**.

#### b.  **Train-Test Split**
- Divided the dataset into **90% training** and **10% testing** subsets.

#### c.  **Elastic Net Regularization**
- Used Elastic Net, combining Lasso (L1) and Ridge (L2) regression.
- Hyperparameter tuning with **GridSearchCV**:
  - Explored multiple `alpha` (regularization strength) and `l1_ratio` (balance between Lasso and Ridge) values.
  - Used 5-fold cross-validation.

#### d.  **Performance Evaluation**
- **Metrics Used**:
  - **Mean Absolute Error (MAE)**: Average prediction error.
  - **Root Mean Squared Error (RMSE)**: Highlights larger errors.
- Achieved errors within 10% of the average sale price, validating the model's accuracy.

---

### 5. 🎯 Prediction and Insights
- Generated predictions for test data and compared them to actual prices.
- Extracted feature importance using Lasso coefficients to identify significant features.
- Recommended dataset simplification by removing non-significant features.

---

## 🛠️ Tools and Libraries
- **Python**: Core programming language.
- **Pandas & NumPy**: Data manipulation.
- **Matplotlib & Seaborn**: Data visualization.
- **scikit-learn**: Machine learning and evaluation.

---

## 📊 Results
- Achieved:
  - **Mean Absolute Error (MAE)**: ~$14,000.
  - **Root Mean Squared Error (RMSE)**: ~$20,000.
- Highlighted key features driving property prices, optimizing accuracy.

---

## 🚀 Future Scope
- Experiment with advanced models like **Random Forests** or **Gradient Boosted Machines**.
- Implement dimensionality reduction techniques for simplification.
- Deploy the model as a **web application** for real-time predictions.

---

## 🤝 Contributions
Contributions are welcome! If you have ideas to improve the project, feel free to open a pull request or raise an issue.

---

## 📬 Contact Me
**Vedant Pimple**  
💼 [LinkedIn](https://www.linkedin.com/in/your-linkedin-profile)  
📧 Email: vedant.pimple@example.com  

---

🎉 Thank you for checking out this project! If you liked it, don’t forget to give it a ⭐ on GitHub!
