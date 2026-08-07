Automobile Dataset - Exploratory Data Analysis (EDA)
📌 Project Overview
This project performs Exploratory Data Analysis (EDA) on the Automobile Dataset using Python.
The objective is to understand the structure of the dataset, analyze feature distributions, identify relationships among variables, and compute different distance and dissimilarity measures used in Data Science.
📂 Dataset Information
Dataset Name: Automobile Dataset
Total Records: 205
Total Features: 26
Libraries Used:
Pandas
NumPy
Matplotlib
Seaborn
🔍 Tasks Performed
1. Data Loading
Imported the Automobile dataset using Pandas.
Displayed the complete dataset.
2. Dataset Exploration
Displayed dataset shape.
Displayed the first five rows.
Identified data types of each attribute.
Displayed column names.
Generated summary statistics using describe().
3. Data Quality Check
Checked for missing (null) values using isnull().sum().
4. Correlation Analysis
Computed the correlation matrix for numerical features.
Visualized the correlation matrix using a heatmap.
5. Data Visualization
Generated visualizations to understand data distribution:
Distribution of Wheel-base
Distribution of Width
Distribution of Number of Cylinders
Distribution of Number of Doors
📏 Distance Measures Implemented
Euclidean Distance
Calculated the Euclidean distance between the symboling and highway-mpg attributes.
Manhattan Distance
Calculated the Manhattan distance between curb-weight and engine-size.
Minkowski Distance
Computed the Minkowski distance (p = 3) between symboling and highway-mpg.
Cosine Dissimilarity
Calculated cosine similarity and converted it into cosine dissimilarity.
📊 Key Observations
The dataset contains 205 automobile records and 26 attributes.
Both numerical and categorical features are present.
The correlation heatmap shows strong positive and negative relationships among several numerical variables.
Wheel-base and width exhibit approximately normal distributions.
Most automobiles have four cylinders.
Most vehicles have either two or four doors.
Euclidean, Manhattan, Minkowski, and Cosine dissimilarity measures were successfully computed for selected attributes.
🛠 Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook / Google Colab
🎯 Learning Outcomes
Loaded and explored a real-world dataset.
Understood dataset structure and feature types.
Performed descriptive statistical analysis.
Checked data quality and missing values.
Visualized feature distributions and correlations.
Applied different distance metrics:
Euclidean Distance
Manhattan Distance
Minkowski Distance
Cosine Dissimilarity
Improved understanding of exploratory data analysis techniques.
📌 Conclusion
This project provides a comprehensive exploratory analysis of the Automobile dataset.
It demonstrates essential data preprocessing, visualization, statistical analysis, correlation analysis, and similarity/distance calculations, which are fundamental steps in data science and machine learning workflows.
