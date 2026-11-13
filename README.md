# python- ML project

## Project Overview

This project focuses on analyzing white wine quality data and building a Machine Learning model to predict wine quality using its physicochemical properties.

The project uses data preprocessing, exploratory data analysis (EDA), feature transformation, and Linear Regression to understand and predict wine quality.

## Objectives

- Analyze the white wine dataset.
- Perform data cleaning and preprocessing.
- Explore relationships between wine properties and quality.
- Build a Machine Learning model using Linear Regression.
- Evaluate model performance using regression metrics.
- Understand the influence of different features on wine quality.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Dataset

The project uses a **White Wine Quality Dataset** (`whitewines.csv`).

The dataset contains physicochemical properties of white wine, including:

- Fixed acidity
- Citric acid
- Density
- pH
- Sulphates
- Alcohol
- Quality

## Project Workflow

### 1. Data Loading
Loaded the dataset using Pandas.

### 2. Exploratory Data Analysis
- Checked dataset dimensions.
- Examined data types and missing information.
- Generated descriptive statistics.
- Visualized the distribution of wine quality.
- Created a correlation heatmap.

### 3. Data Cleaning
- Removed duplicate records.
- Removed records with zero or negative alcohol, pH, and quality values.
- Filtered records with pH and quality values below 10.

### 4. Feature Transformation
- Applied logarithmic transformation to alcohol.
- Applied logarithmic transformation to the target variable (quality).

### 5. Model Building
Used a Scikit-learn Pipeline with:
- Data preprocessing.
- Linear Regression.

### 6. Model Evaluation

Evaluated the model using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R-squared (R²)
- R-squared on the log scale

A residual plot was also created to examine prediction errors.

### 7. Feature Analysis

Extracted and sorted Linear Regression coefficients to understand the contribution of different input features.

## How to Run the Project

1. Clone or download this repository.
2. Install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

3. Place the `whitewines.csv` dataset in the appropriate location.
4. Open Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `ml project.ipynb` and execute the notebook cells.

## Machine Learning Algorithm

**Linear Regression**

Linear Regression is used to model the relationship between wine characteristics and wine quality.

The target variable is logarithmically transformed during model training, and predictions are converted back using the exponential function.

## Evaluation Metrics

| Metric | Purpose |
|---|---|
| MAE | Measures average absolute prediction error |
| RMSE | Measures prediction error while penalizing larger errors |
| R² | Measures the proportion of variance explained by the model |

## Future Improvements

- Experiment with Random Forest and other regression algorithms.
- Perform feature selection.
- Apply cross-validation.
- Tune model hyperparameters.
- Compare different models to improve prediction performance.

## Conclusion

This project demonstrates an end-to-end Machine Learning workflow for white wine quality analysis, including data cleaning, exploratory data analysis, feature transformation, regression modeling, and model evaluation.

The project provides insights into how physicochemical properties can be used to predict white wine quality.
