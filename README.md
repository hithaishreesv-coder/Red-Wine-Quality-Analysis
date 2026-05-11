# Red Wine Quality Analysis and Prediction

## Project Overview

This project focuses on analysing red wine quality using Python. The aim of the project is to understand which chemical properties of red wine are most related to wine quality and to build regression models to predict wine quality.

The dataset contains physicochemical properties of red wine, such as acidity, sugar, chlorides, sulphur dioxide, density, pH, sulphates, alcohol, and quality score.

This project was completed using Python in a Jupyter/Colab notebook.

---

## Dataset

The dataset used in this project is the red wine quality dataset.

The dataset contains:

- 1,599 rows
- 12 columns
- 11 independent feature variables
- 1 target variable: `quality`

The target variable represents the quality score of red wine.

---

## Features in the Dataset

The dataset includes the following variables:

- Fixed acidity
- Volatile acidity
- Citric acid
- Residual sugar
- Chlorides
- Free sulfur dioxide
- Total sulfur dioxide
- Density
- pH
- Sulphates
- Alcohol
- Quality

---

## Project Objectives

The main objectives of this project were:

- Import and explore the red wine dataset
- Identify the number of rows and columns
- Analyse feature spread and variability
- Generate a correlation matrix
- Identify variables most correlated with wine quality
- Examine which variables follow a normal distribution
- Apply Principal Component Analysis
- Compare PCA results before and after normalisation
- Calculate empirical probabilities for wine quality scores
- Build a multiple linear regression model
- Improve the model using polynomial regression
- Evaluate model performance using R-square and error metrics

---

## Tools and Technologies Used

- Python
- Google Colab / Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- SciPy

---

## Exploratory Data Analysis

The dataset was imported and explored using Python.

The dataset contains 1,599 records and 12 columns.

The independent variables were analysed to identify which features had the least spread of data values.

The three variables with the least spread were:

- Density
- Chlorides
- Citric acid

---

## Correlation Analysis

A correlation matrix was created to understand the relationship between all feature variables and the target variable `quality`.

The top three feature variables with the strongest correlation with wine quality were:

- Alcohol
- Sulphates
- Citric acid

This means these features showed stronger relationships with the wine quality score compared to other variables.

---

## Distribution Analysis

Histograms were used to examine whether the variables followed a normal distribution.

The variables that were observed to approximately follow a Gaussian distribution were:

- pH
- Density

Chlorides also showed a distribution close to Gaussian, but with a right tail.

---

## Principal Component Analysis

Principal Component Analysis was applied to the independent feature variables.

PCA was first performed on the original feature values. The first principal component explained most of the variance in the dataset.

The feature contributing more than 30% to the variance distribution was:

- Total sulfur dioxide

---

## PCA after Normalisation

The PCA analysis was repeated after normalising all feature variables using StandardScaler.

After normalisation, the features contributing more than 30% to the observed variance distribution were:

- Fixed acidity
- Citric acid
- Density

This showed that normalisation changed the PCA results because all variables were placed on the same scale.

---

## Empirical Probability Analysis

Empirical probability was calculated using the wine quality score.

The following probabilities were calculated:

- Probability of wine quality being less than 5
- Probability of wine quality being equal to or greater than 8

The results were:

- P(Quality < 5) = 0.0394
- P(Quality >= 8) = 0.0113

This means only a small proportion of wines had very low or very high quality scores.

---

## Hypothesis Testing

Hypothesis testing was used to test claims about the average quality of red wine.

A confidence interval was calculated using the sample data.

At 98% confidence level, the calculated confidence interval was approximately:

```text
5.589 to 5.683
