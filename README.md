# Ford Vehicle ML Analysis

Repository: Ford-Vehicle-ML-Analysis

This project analyzes used Ford vehicle data to understand the main drivers of car prices and build machine learning models that can predict a vehicle's selling price from its features.

## Project Goal

The objective is to study how attributes such as year, mileage, engine size, horsepower-like extracted variables, fuel type, and model influence used Ford car prices. The notebook also demonstrates proper machine learning workflow practices, including data cleaning, train/test splitting before preprocessing, and model evaluation.

## Dataset

- File: `ford.csv`
- Target variable: `price`
- Features include:
  - `year`
  - `model`
  - `mileage`
  - `fuelType`
  - `transmission`
  - `tax`
  - `mpg`
  - `engineSize`

## Data Cleaning and Quality Checks

The project includes a strong data-quality review before modeling:

- checked for duplicate rows
- detected impossible years
- removed zero engine size values
- stripped extra spaces from model names
- kept unusually high MPG values because they can be valid in some cases

This makes the analysis more reliable and demonstrates professional data-science practice.

## Exploratory Data Analysis

The notebook explores the relationships between price and the main features:

- price distribution is right-skewed
- newer vehicles generally cost more
- higher mileage is associated with lower prices
- automatic transmission and larger engine sizes often correlate with higher price
- model type matters significantly, with some models priced much higher than others

## Modeling Approach

The workflow uses a scikit-learn pipeline that separates preprocessing from model training:

- train/test split performed first
- numerical features standardized
- categorical features encoded using one-hot encoding
- comparison between:
  - Linear Regression
  - Random Forest Regressor
- evaluation using:
  - R2 score
  - MAE
  - RMSE
  - cross-validation

This avoids data leakage and produces more trustworthy evaluation results.

## Key Insights

- Car price is strongly influenced by age, mileage, and model type.
- Newer cars command higher value.
- Engine size and transmission type also affect price significantly.
- The random forest model captured non-linear patterns better than a simple linear model.
- One-hot encoding was preferred over label encoding for a linear model because ordinal categories do not have a true numeric meaning.

## Tech Stack

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- scikit-learn
- Jupyter Notebook

## Files in This Project

- `ford_fixed.ipynb` — full analysis notebook
- `ford.csv` — dataset used for modeling

## How to Run

Open the notebook in Jupyter or VS Code and run the cells sequentially:

```bash
jupyter notebook ford_fixed.ipynb
```

## Project Summary

This project is a practical machine learning case study focused on regression, data cleaning, and model comparison. It is especially useful for showcasing real-world data handling and proper ML pipeline design in interviews or portfolio work.
