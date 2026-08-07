# Iris Dataset - Correlation Analysis and Measures of Dispersion

## Overview

This project performs Exploratory Data Analysis (EDA) on the Iris dataset using Python. 
The analysis focuses on understanding the dataset, identifying relationships between numerical features through a correlation matrix, and measuring the spread of data using both absolute and relative measures of dispersion.

The Iris dataset is one of the most widely used datasets in machine learning and statistics. It contains 150 observations of iris flowers belonging to three different species: Setosa, Versicolor, and Virginica.
Each observation includes four numerical features—sepal length, sepal width, petal length, and petal width—and one categorical feature representing the flower species.

## Objectives

* Load and explore the Iris dataset.
* Identify numerical and categorical features.
* Examine the structure and quality of the dataset.
* Generate descriptive statistics.
* Compute and visualize the correlation matrix using a heatmap.
* Calculate absolute measures of dispersion.
* Calculate relative measures of dispersion.
* Interpret the statistical results to understand feature relationships and variability.

## Dataset Information

* **Dataset:** Iris Flower Dataset
* **Source:** Seaborn Built-in Dataset
* **Total Records:** 150
* **Numerical Features:**

  * Sepal Length
  * Sepal Width
  * Petal Length
  * Petal Width
* **Categorical Feature:**

  * Species (Setosa, Versicolor, Virginica)

## Exploratory Data Analysis

The following analyses were performed:

* Imported the required Python libraries.
* Loaded the Iris dataset.
* Displayed the first and last five records.
* Checked the dataset dimensions.
* Identified column names and data types.
* Examined dataset information.
* Verified missing values and duplicate records.
* Generated descriptive statistics for all numerical features.

## Correlation Analysis

A Pearson correlation matrix was generated to measure the relationship between numerical features. The correlation matrix was visualized using a heatmap for easier interpretation.

### Key Findings

* Petal Length and Petal Width show the strongest positive correlation.
* Sepal Width has comparatively weaker correlation with the remaining features.
* No strong negative correlations were observed.

## Absolute Measures of Dispersion

The following measures were calculated to determine the actual spread of the data:

* Range
* Variance
* Standard Deviation

These measures provide information about how widely the observations are distributed around the mean.

## Relative Measures of Dispersion

The following relative measures were calculated:

* Coefficient of Range
* Coefficient of Quartile Deviation
* Coefficient of Mean Deviation
* Coefficient of Variation (CV)

These measures express variability relative to a central value, making it possible to compare the spread of different features regardless of their scale.

## Technologies Used

* Python
* Pandas
* NumPy
* Seaborn
* Matplotlib

## Conclusion

This project demonstrates the complete statistical exploration of the Iris dataset through correlation analysis and dispersion measures. 
The analysis helps in understanding relationships among features, identifying variability within the dataset, and preparing the data for further machine learning or statistical modeling.
