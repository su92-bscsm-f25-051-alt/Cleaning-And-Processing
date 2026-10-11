# Titanic Dataset --- Data Cleaning and Preprocessing

## Assignment Overview

This project performs data cleaning and preprocessing on the Titanic
dataset from Kaggle. The objective is to inspect the data, handle
data-quality issues, create useful features, and prepare the dataset for
further analysis and machine learning.

## Dataset Information

-   **Dataset title:** Titanic --- Machine Learning from Disaster
-   **Dataset source:** [Kaggle Titanic Competition --- Dataset and
    Data](https://www.kaggle.com/competitions/titanic/data)
-   **Competition overview:** [Titanic --- Machine Learning from
    Disaster](https://www.kaggle.com/competitions/titanic)
-   **File used:** `train.csv`
-   **Original dataset size:** 891 rows and 12 columns
-   **Target column:** `Survived`
    -   `0` = Did not survive
    -   `1` = Survived

The dataset contains passenger information such as passenger class,
name, sex, age, number of siblings or spouses aboard, number of parents
or children aboard, ticket, fare, cabin, and port of embarkation. The
objective of the original Kaggle challenge is to explore which passenger
characteristics were associated with survival.

## Data Cleaning and Preprocessing Steps

1.  Loaded the Titanic training dataset from the Kaggle input folder.
2.  Inspected the dataset shape, data types, summary statistics, and
    missing values.
3.  Checked for duplicate records.
4.  Standardized text values and converted columns to suitable data
    types.
5.  Checked and handled invalid values.
6.  Examined missing values and created a `Deck` feature from the
    `Cabin` column.
7.  Detected possible outliers in `Age` and `Fare` using the
    Interquartile Range (IQR) method.
8.  Applied a log transformation to `Fare` to create `Fare_log`.
9.  Created additional features:
    -   `FamilySize`
    -   `IsAlone`
    -   `Title`
10. Split the data into training and validation sets.
11. Prepared numerical features using median imputation and standard
    scaling.
12. Prepared categorical features using most-frequent imputation and
    one-hot encoding.
13. Checked the processed data and saved the cleaned dataset.

## Output Files

The notebook saves the cleaned dataset to:

`/kaggle/working/titanic_cleaned.csv`

It also creates an original backup at:

`/kaggle/working/titanic_original_backup.csv`

These paths are available inside the Kaggle Notebook environment.
Download the files from the notebook's output section if you need them
on your computer.

## Tools and Libraries

-   Python
-   Pandas
-   NumPy
-   Matplotlib
-   Scikit-learn
-   Kaggle Notebooks

## How to Run

1.  Open a Kaggle Notebook.
2.  Add the Titanic dataset as notebook input. You may need to join the
    competition and accept its rules to access the data.
3.  Run the notebook cells in order, from the dataset-loading cell to
    the final conclusion.
4.  Review the displayed summaries and preprocessing results.
5.  Download `titanic_cleaned.csv` from the notebook's output files.

## Conclusion

This assignment demonstrates common data cleaning and preprocessing
techniques, including data inspection, missing-value handling, data-type
correction, outlier detection, feature engineering, train-validation
splitting, encoding, and scaling. These steps prepare the data for
further analysis and machine learning.
