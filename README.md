# 🏠 Task 3: Linear Regression – Housing Price Prediction

## 🎯 Objective
To implement and understand **Simple and Multiple Linear Regression** using a housing dataset, and evaluate model performance using appropriate metrics.

---

## 🧰 Tools & Libraries Used
- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Seaborn**

---

## 📁 Dataset

We use a housing price dataset that includes 13 features such as:
- Area
- Bedrooms
- Bathrooms
- Parking
- Air conditioning
- Furnishing status, etc.

📥 (https://www.kaggle.com/datasets/harishkumardatalab/housing-price-prediction)

---

## 🔍 Steps Followed

### 1. **Import & Explore Data**
- Loaded dataset using `pandas`
- Displayed shape, info, and statistics using `.info()`, `.describe()`, `.isnull()`

### 2. **Preprocessing**
- Applied **Label Encoding** to categorical features like `mainroad`, `furnishingstatus`, etc.
- Checked and removed **outliers** in `price` and `area` columns using **IQR method** and **boxplots**

### 3. **Splitting the Dataset**
- Separated independent (`x`) and dependent (`y`) variables
- Performed **train-test split** using `train_test_split()` (80% train / 20% test)

### 4. **Feature Scaling**
- Standardized the feature set using **StandardScaler** from `sklearn.preprocessing`

### 5. **Model Building**
- Trained a **Linear Regression model** using `LinearRegression()` from `sklearn.linear_model`
- Fitted on training data and made predictions on test data

### 6. **Evaluation**
Used the following regression metrics:
- **MAE** (Mean Absolute Error)
- **MSE** (Mean Squared Error)
- **RMSE** (Root Mean Squared Error)
- **R² Score** (Coefficient of Determination)

---

## 📊 Model Evaluation Metrics

| Metric | Value |
|--------|--------|
| MAE    | ₹742,678.29 |
| MSE    | ₹977,664,860,283.97 |
| RMSE   | ₹988,769.37 |
| R²     | 0.6668 |

> Interpretation: The model explains ~66.7% of the variance in prices, with an average error of ~₹7.4 Lakhs.

---

## 📉 Visualization

- Used **boxplots** to visualize outliers in `price` and `area`
- Plotted **regression line** (optional extension)
  
---

## 💡 What You’ll Learn

- How to preprocess data for regression models
- How to apply and evaluate **Linear Regression**
- Importance of **scaling**, **encoding**, and **outlier removal**
- Interpreting model performance using **MAE, MSE, RMSE, R²**

---



## 📎 Future Improvements (Optional)
- Apply **log transformation** to `price` for better model fit
- Try **Ridge** or **Lasso Regression**
- Include more features like house age or location score
- Perform **k-fold cross-validation** for better generalization

---

## 📂 Folder Structure

