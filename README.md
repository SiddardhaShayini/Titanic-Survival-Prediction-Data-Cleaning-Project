
# Titanic Survival Prediction – Data Cleaning Project

## Project Overview

This mini project focuses on **cleaning and preprocessing the Titanic dataset** using Python and Pandas. The cleaned data is prepared for further machine learning or data analysis.

## Steps Performed

### 1. Upload and Load Dataset

-   Uploaded the Titanic CSV file using Google Colab.
-   Loaded the dataset into a Pandas DataFrame.
-   Displayed the first 5 rows.

### 2. Basic Data Summary

-   Used `df.info()` to check:
    -   Number of rows and columns
    -   Column names
    -   Data types
    -   Missing values

### 3. Descriptive Statistics

-   Used `df.describe()` to view basic statistics such as:
    -   Mean
    -   Minimum
    -   Maximum
    -   Standard deviation

### 4. Handling Missing Values

-   Filled missing values in the **Age** column using the median age.
-   Filled missing values in the **Embarked** column using its most frequent value (mode).
-   Dropped the **Cabin** column because it contained many missing values.

### 5. Encoding Categorical Variables

-   Converted **Sex** into numerical values using `LabelEncoder`.
-   Converted **Embarked** into numerical columns using `OneHotEncoder`.

This makes the categorical data suitable for machine learning models.

### 6. Visualizing Age

-   Created a histogram with a KDE curve to visualize the distribution of the **Age** column after missing values were handled.

### 7. Save Cleaned Dataset

-   Saved the cleaned dataset as:

```text
titanic_cleaned.csv

```

-   Downloaded the cleaned CSV file from Google Colab.

## Technologies Used

-   Python
-   Pandas
-   Scikit-learn
-   Matplotlib
-   Seaborn
-   Google Colab

## Output

The final output is a cleaned and encoded Titanic dataset named:

**`titanic_cleaned.csv`**

## Conclusion

The Titanic dataset was successfully cleaned by handling missing values, removing a column with excessive missing data, encoding categorical variables, and visualizing the Age distribution. The resulting dataset can be used for further analysis or building a **Titanic survival prediction model**.
