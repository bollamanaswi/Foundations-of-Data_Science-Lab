# Titanic Dataset – Data Cleaning Using Pandas

## 📌 Project Description

This notebook demonstrates basic **data cleaning and missing-value handling** using the Titanic dataset with Python and Pandas.

The notebook explores the dataset structure, checks data types and missing values, and demonstrates different ways to remove rows or columns containing null values.

## 📊 Dataset

The Titanic dataset contains **891 rows and 12 columns**. The columns include:

* PassengerId
* Survived
* Pclass
* Name
* Sex
* Age
* SibSp
* Parch
* Ticket
* Fare
* Cabin
* Embarked

The dataset is loaded into a Pandas DataFrame using `pd.read_csv()`.

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Google Colab
* Jupyter Notebook

## 🔍 Operations Performed

### 1. Import Libraries

```python
import pandas as pd
import numpy as np
```

### 2. Load the Dataset

```python
df = pd.read_csv("Titanic-Dataset.csv")
```

### 3. Explore the Dataset

The notebook uses:

```python
df.head()
df.tail()
df.shape
df.columns
df.dtypes
```

These commands are used to view the first and last records, identify the number of rows and columns, display column names, and check data types.

### 4. Check Missing Values

```python
df.isnull().sum()
```

Initially, the dataset contains missing values in:

* Age – 177
* Cabin – 687
* Embarked – 2

The remaining columns contain no null values at this stage.

### 5. Remove Completely Empty Rows

```python
df.dropna(how='all', inplace=True)
```

This removes rows where **all column values are null**.

### 6. Remove Rows with Missing Age

```python
df.dropna(subset=['Age'], inplace=True)
```

This removes rows where the `Age` value is missing. After this operation, the `Age` column has no null values.

### 7. Use `thresh` with Multiple Columns

```python
df.dropna(
    subset=['Cabin', 'Embarked'],
    thresh=1,
    inplace=True
)
```

Here, `thresh=1` means that a row must have **at least one non-null value** among `Cabin` and `Embarked`.

Therefore, a row is removed only when **both Cabin and Embarked are null**.

In the notebook, this operation does not reduce the remaining null counts because the rows generally have at least one of these two values available.

### 8. Remove Rows Containing Any Null Value

```python
df.dropna(axis=0, inplace=True)
```

`axis=0` works on rows. This removes rows containing one or more null values. The resulting dataset has zero null values in every column.

### 9. Remove Columns Containing Null Values

```python
df.dropna(axis=1, inplace=True)
```

`axis=1` works on columns. This removes columns containing null values.

### 10. Remove Rows with Any Null Value Using `how='any'`

```python
df.dropna(how='any', inplace=True)
```

This removes any row containing at least one null value. After the operation, all columns contain zero null values.

## 🎯 Learning Objectives

Through this notebook, we learn how to:

* Load datasets using Pandas
* Inspect a DataFrame
* Identify rows and columns
* Check column data types
* Detect missing values
* Remove completely empty rows
* Remove rows based on a specific column
* Understand `subset` and `thresh`
* Remove rows using `axis=0`
* Remove columns using `axis=1`
* Use `how='all'` and `how='any'`

## 📌 Key Concepts

### `dropna()`

`dropna()` is a Pandas function used to remove missing values from a DataFrame.

### `subset`

Specifies the columns that should be considered when checking for missing values.

### `thresh`

Specifies the **minimum number of non-null values required**.

For example:

```python
subset=['Cabin', 'Embarked'], thresh=1
```

means at least **one of the two columns must contain a value**.

```python
subset=['Cabin', 'Embarked'], thresh=2
```

means **both columns must contain values**.

### `axis`

* `axis=0` → operates on rows
* `axis=1` → operates on columns

## 📈 Conclusion

This notebook provides practical experience with **Pandas data cleaning techniques**, especially handling missing values. It demonstrates how different `dropna()` parameters such as `subset`, `thresh`, `how`, and `axis` affect a dataset.

These techniques are important preprocessing steps before performing **data analysis and machine learning**.
