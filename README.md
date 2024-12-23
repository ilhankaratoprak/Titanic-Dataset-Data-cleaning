# Titanic Dataset Project

This project involves analyzing and cleaning the Titanic dataset. The Titanic dataset contains information about passengers aboard the Titanic ship, and it is commonly used in machine learning and data analysis projects.

## Project Goal

The goal of this project is to analyze the Titanic dataset and predict the survival status of passengers during the ship's sinking. The data cleaning process has been performed from three different perspectives: **missing data**, **incorrect or inconsistent data**, and **outliers**. These steps ensure that the data is cleaned and prepared for further analysis and modeling.

## Technologies Used

- **Python**: For data processing and analysis.
- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical calculations and array operations.
- **Matplotlib & Seaborn**: For data visualization.

## Dataset

The Titanic dataset contains information about each passenger, including the following columns:

- **PassengerId**: Passenger's ID number.
- **Pclass**: Passenger's ticket class.
- **Name**: Passenger's name.
- **Sex**: Passenger's gender.
- **Age**: Passenger's age.
- **SibSp**: Number of siblings or spouses aboard.
- **Parch**: Number of parents or children aboard.
- **Ticket**: Ticket number.
- **Fare**: Ticket fare.
- **Cabin**: Cabin number.
- **Embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).
- **Survived**: Survival status (0 = did not survive, 1 = survived).

## Data Cleaning Steps

### 1. Missing Data

Missing data is a common issue in data analysis. The following steps were taken to handle missing data in the Titanic dataset:

- **Age**: Missing values in the Age column were filled with the mean age of the passengers.
- **Embarked**: Missing values in the Embarked column were filled with the most frequent value, which was "S" (Southampton).
- **Cabin**: The Cabin column had a significant number of missing values, so it was entirely removed from the dataset.

### 2. Incorrect or Inconsistent Data

Incorrect or inconsistent data can lead to misleading analysis. The following steps were applied to address this:

- **Sex**: The Sex column, which had categorical values ("male" and "female"), was converted into numerical values (Female = 0, Male = 1).
- **Pclass**: The Pclass column was also transformed into numerical values to ensure consistency across the dataset.

### 3. Outliers

Outliers can distort the results of data analysis. The following steps were performed to detect and handle outliers:

- **Fare**: Extreme values in the Fare column were identified and addressed (e.g., by capping values or normalizing them).
- **Age**: Age values were inspected for unrealistic values (e.g., age 0 or above 100) and corrected accordingly.

## Analysis and Visualization

Once the data cleaning process was completed, the following visualizations were generated to understand survival patterns among passengers:

- Distribution of age for passengers who survived and those who did not.
- Distribution of passengers who survived and those who did not by ticket class.
- Survival rates by gender.

## Usage Instructions

To run this project on your local machine, follow the steps below:

1. Install Python 3.x.
2. Install the necessary libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
