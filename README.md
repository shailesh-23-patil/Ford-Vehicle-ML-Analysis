# Ford Vehicle ML Analysis

A machine learning project that analyzes used Ford vehicle data to identify the key factors influencing car prices and predict selling prices using regression models.

## Project Goal

The objective is to understand how vehicle attributes such as manufacturing year, mileage, model, fuel type, transmission, tax, MPG, and engine size affect used Ford car prices. The project demonstrates a complete machine learning workflow, from data cleaning and exploratory data analysis to model training and evaluation.

## Dataset

- **Dataset:** `ford.csv`
- **Target variable:** `price`
- **Features:**
  - `year`
  - `model`
  - `mileage`
  - `fuelType`
  - `transmission`
  - `tax`
  - `mpg`
  - `engineSize`

## Data Cleaning and Quality Checks

The project performs data-quality checks before model training:

- Identifies duplicate records.
- Checks for implausible manufacturing years.
- Removes records with zero engine size where appropriate.
- Removes unnecessary whitespace from model names.
- Reviews unusually high MPG values before deciding whether to retain them.

These steps help improve dataset consistency and reliability.

## Exploratory Data Analysis (EDA)

The notebook explores relationships between vehicle prices and different attributes, including:

- Distribution of vehicle prices.
- Relationship between manufacturing year and price.
- Effect of mileage on resale value.
- Price differences across models and fuel types.
- Influence of transmission type and engine size on vehicle prices.

Visualizations help identify patterns, trends, and potential relationships in the dataset.

## Machine Learning Approach

The project uses a structured machine learning workflow with Scikit-learn.

### Data Preprocessing
- Separates training and testing data before fitting preprocessing transformations.
- Standardizes numerical features where required.
- Applies one-hot encoding to categorical features.
- Uses pipelines to organize preprocessing and model training.

### Models
- Linear Regression
- Random Forest Regressor

### Evaluation Metrics
- R² Score
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Cross-validation

These metrics help compare model performance and assess prediction quality on unseen data.

## Key Insights

The analysis investigates the following potential patterns:

- Newer vehicles may have higher selling prices.
- Higher mileage may be associated with lower prices.
- Vehicle model, engine size, and transmission may influence price.
- Random Forest can capture nonlinear relationships that Linear Regression may not represent effectively.

Actual findings and model comparisons are available in the Jupyter Notebook.

## Technology Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
Ford-Vehicle-ML-Analysis/
├── ford.csv
├── ford_fixed.ipynb
└── README.md
```

## How to Run

1. Clone or download this repository.
2. Install Python and Jupyter Notebook.
3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

4. Open the project directory in Command Prompt.
5. Launch the notebook:

   ```bash
   jupyter notebook ford_fixed.ipynb
   ```

6. Run the notebook cells sequentially.

## Project Objectives

- Perform data cleaning and exploratory data analysis.
- Understand factors associated with used Ford vehicle prices.
- Build and compare regression models.
- Apply appropriate preprocessing and evaluation techniques.
- Demonstrate practical machine learning skills through a real-world dataset.

## Conclusion

Ford Vehicle ML Analysis is a practical regression project demonstrating data preprocessing, visualization, feature handling, model training, and performance evaluation. It can serve as a machine learning portfolio project for students and aspiring data analysts.

---

**Author:** Shailesh Patil

**Project Type:** Machine Learning — Regression