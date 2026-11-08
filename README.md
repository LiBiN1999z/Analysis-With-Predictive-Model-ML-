# 🏡 Housing Price Prediction Using Machine Learning

## 📌 Overview

This project focuses on analyzing and predicting house prices using Machine Learning techniques.

The **California Housing Dataset** is used to explore different factors affecting house prices, such as median income, geographical location, housing age, population, and ocean proximity.

The project uses Python for data cleaning, Exploratory Data Analysis (EDA), data visualization, preprocessing, and Machine Learning model development.

A **Linear Regression** algorithm is implemented to predict median house values.

## 🎯 Objectives

- Understand and analyze the California Housing Dataset.
- Identify important factors influencing house prices.
- Perform data cleaning and handle missing values.
- Conduct Exploratory Data Analysis (EDA).
- Visualize relationships between housing features.
- Apply categorical encoding and feature scaling.
- Build a Machine Learning model using Linear Regression.
- Predict median house prices.
- Evaluate model performance using regression metrics.

## 📊 Dataset Information

**Dataset:** California Housing Dataset

- Total Records: 20,640
- Original Columns: 10
- Target Variable: `median_house_value`

### Dataset Features

| Feature | Description |
|---|---|
| longitude | Geographic longitude |
| latitude | Geographic latitude |
| housing_median_age | Median age of houses |
| total_rooms | Total number of rooms |
| total_bedrooms | Total number of bedrooms |
| population | Population of the area |
| households | Number of households |
| median_income | Median income |
| median_house_value | Median house value (Target) |
| ocean_proximity | Proximity to the ocean |

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## ⚙️ Workflow

### 1. Data Understanding
- Loaded the California Housing Dataset.
- Examined dataset structure and dimensions.
- Identified numerical and categorical features.
- Generated descriptive statistics.

### 2. Data Cleaning
- Checked for missing values.
- Handled missing values in `total_bedrooms` using median imputation.
- Checked duplicate records.

### 3. Exploratory Data Analysis (EDA)

Performed statistical analysis and data visualization to understand:

- Distribution of house prices.
- Relationship between median income and house prices.
- Ocean proximity and average house prices.
- House price distribution by ocean proximity.
- Correlation between numerical variables.
- Geographical distribution of house prices.

### 4. Data Preprocessing

- Separated independent and dependent variables.
- Applied One-Hot Encoding to the `ocean_proximity` column.
- Applied StandardScaler for feature scaling.
- Prepared the dataset for Machine Learning.

After encoding, the dataset contained 13 features.

### 5. Train-Test Split

The dataset was divided into:

- Training Data: 80% (16,512 records)
- Testing Data: 20% (4,128 records)

The `random_state=42` parameter was used for reproducibility.

### 6. Machine Learning Model

**Algorithm:** Linear Regression

The model was trained using the training dataset and used to predict median house prices on the testing dataset.

### 7. Model Evaluation

The model was evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

## 📈 Model Performance

The Linear Regression model achieved the following results:

| Evaluation Metric | Result |
|---|---:|
| MAE | 50,670.74 |
| MSE | 4,908,476,721.16 |
| RMSE | 70,060.52 |
| R² Score | 0.6254 |

**Model Interpretation:**

The model achieved an R² score of approximately 62.54%, meaning it explains 62.54% of the variation in median house prices in the testing dataset.

## 🔍 Key Findings

1. Median income has a strong positive correlation (0.688) with median house value.
2. House prices generally increase as median income increases.
3. Inland areas have lower average house prices compared to coastal areas.
4. Island locations show the highest average house prices, but the category contains only five records.
5. Total rooms and total bedrooms have a strong positive correlation (0.927).
6. Population and households have a strong positive correlation (0.907).
7. Population and median house value have a very weak negative correlation (-0.025).
8. Geographical location plays an important role in house price variations.
9. The dataset contains a noticeable concentration of house values at the $500,001 upper limit.

## 📉 Actual vs Predicted Prices

The project compares actual house prices with predicted house prices using visualizations.

The comparison helps understand:

- How accurately the model predicts house prices.
- Differences between actual and predicted values.
- The general prediction trend.
- Outliers and prediction errors.

## ⚠️ Project Limitations

- The dataset contains limited information about housing features.
- Linear Regression may not capture complex relationships between variables.
- Some factors affecting house prices are not included.
- Outliers may affect prediction accuracy.
- The model achieved an R² score of 62.54%, so some price variations remain unexplained.

## 💡 Conclusion

This project demonstrates how Machine Learning can be used to analyze housing data and predict house prices.

Through Exploratory Data Analysis, important relationships were identified between median income, geographical location, ocean proximity, and house prices.

A Linear Regression model was developed and achieved an R² score of 0.6254 (62.54%).

Overall, this project helped develop practical knowledge of Python, data cleaning, data visualization, feature engineering, Machine Learning, and model evaluation.

## 🚀 How to Run This Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Housing-Price-Prediction.git
```

### 2. Navigate to the Project Folder

```bash
cd Housing-Price-Prediction
```

### 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

### 5. Run the Notebook

Open `machine learning .ipynb` and execute the cells.

Aspiring Data Analyst | Machine Learning Enthusiast

## ⭐ Acknowledgement

This project was completed as part of my learning journey in Data Analytics and Machine Learning.
