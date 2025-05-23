# 🏠 Housing Price Prediction

This is my **very first machine learning project**, where I predict house prices based on input features using supervised regression models. I followed a project-based and self-learning approach to study AI. Although I'm not yet well-versed in ML theory, I aimed to create a complete and functional end-to-end workflow. ❤️

---

## 🧠 Problem Definition

The goal of this project is to:

- Predict housing prices based on features (area, bedrooms, parking, etc.).
- Apply a real-world machine learning pipeline.
- (Optionally in the future) infer which features most impact housing prices — useful for real estate and business decisions.

---

## 📊 Dataset

- Source: [Kaggle](https://www.kaggle.com/code/ashydv/housing-price-prediction-linear-regression)
- Format: `.zip` containing a `.csv` file
- Features:
  - **Numerical:** `area`, `bedrooms`, `bathrooms`, `stories`, `parking`, `price`
  - **Categorical (binary):** `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `prefarea`
  - **Categorical (nominal):** `furnishingstatus` (furnished/semi/unfurnished)

---

## 🔁 Project Workflow

1. **Data Collection & Reading**
2. **Data Cleaning**
   - Removed 15 outliers using IQR
   - No missing or duplicate values
3. **Data Preprocessing**
   - One-hot encoding for categorical features
   - Feature scaling with `StandardScaler`
4. **Exploratory Data Analysis (EDA)**
   - Distribution of `price`
   - Correlation and boxplots
   - Multicollinearity check
5. **Feature Engineering**
   - Created `sum_area = area × stories`
   - Created `amenities_count` = count of all "yes" binary features
   - One-hot encoded `stories`
6. **Modeling**
   - Baseline: `LinearRegression`
   - Final: `XGBoostRegressor`
7. **Evaluation & Tuning**
   - Used RMSE, R²
   - GridSearchCV and RandomSearchCV for tuning
   - Visualized predicted vs actual values

---

## ✅ Final Results

- **Model:** XGBoostRegressor
- **RMSE:** 1,093,408
- **R² Score:** 0.653

---

## 📈 Actual vs Predicted Plot

![Actual vs Predicted](https://github.com/user-attachments/assets/7e4e5793-a4ba-43c6-9fc7-f762895c3f55)

---

## 🛠 Technologies Used

- Python
- Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn
- XGBoost
- Google Colab

---

## 🧑‍💻 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/Housing-price-prediction.git

# 2. Upload the zip dataset from Kaggle

# 3. Open and run the notebook in Google Colab or Jupyter




  
   


