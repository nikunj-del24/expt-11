# expt-11
# Nikunj Deep Upadhyay
# entc b1
# 25070123081

Aim
To create a dataset using Python, save it as a CSV file, and perform various operations using the Pandas library, including loading datasets, exploring structure, and analyzing data.

Note: This experiment contains a dataset that was used in a file seperately. It can be found by the name of Cars93.csv within the repository itself. However, incase that file cannot be accessed, the data is provided at the end for reference as well.
Theory
Pandas is a powerful Python library used for handling and analyzing structured data. It provides efficient tools for creating, storing, loading, and analyzing datasets.

In this experiment, both dataset creation and dataset loading from external files are performed, along with multiple operations to understand and analyze the data.

Dataset Creation
A dataset can be created using a dictionary in Python and then converted into a DataFrame.

import pandas as pd

data = {
    "Roll Number": [101,102,103,104,105],
    "Gender": ["Male","Female","Female","Male","Male"],
    "Department": ["Computer Science","IT","ENTC","Mechanical","Computer Science"],
    "CGPA": [8.2,7.5,9.1,6.8,8.7]
}

df = pd.DataFrame(data)
Saving Dataset
The created dataset can be saved into a CSV file using:

df.to_csv("student_data.csv", index=False)
index=False ensures that row indices are not saved in the file.
Basic DataFrame Operations
1. Shape of Dataset
df.shape
Returns number of rows and columns
Example: (5, 4)
2. Size of Dataset
df.size
Returns total number of elements in dataset
3. Information of Dataset
df.info()
Displays:

Number of entries
Column names
Data types
Non-null values
Memory usage
Descriptive Statistics
df.describe()
Provides statistical summary:

Count
Mean
Standard deviation
Minimum and maximum values
Percentiles
Loading Dataset from File
A dataset can be loaded from an external CSV file:

df = pd.read_csv("Cars93.csv")
This loads a large dataset containing attributes such as:

Manufacturer
Model
Type
Price
MPG (mileage)
Horsepower
Passengers
and more
Operations on Loaded Dataset
1. Dataset Size
df.size
Total number of elements in dataset
2. Dataset Shape
df.shape
Returns rows and columns (e.g., 93 rows × 10 columns)
3. Statistical Summary
df.describe()
Provides summary statistics for numerical columns like:

Price
MPG
Horsepower
4. Viewing Data
df.head()
Displays first 5 rows
df.tail()
Displays last 5 rows
5. Column Names
df.columns
Returns all column names in dataset
6. Random Sampling
df.sample(5)
Displays 5 random rows from dataset
7. Dataset Information
df.info()
Provides detailed structure of dataset including null values
8. Data Types
df.dtypes
Displays datatype of each column
9. Checking Missing Values
df.isnull().sum()
Shows number of missing (null) values in each column
10. Checking Duplicate Values
df.duplicated().sum()
Returns number of duplicate rows
11. Counting Unique Values
df.nunique()
Returns number of unique values in each column
Key Learnings
Creation of dataset using dictionary
Conversion into DataFrame
Saving dataset as CSV file
Loading dataset from external file
Exploring dataset structure
Performing statistical analysis
Handling missing and duplicate data
Conclusion
In this experiment, dataset creation and loading techniques were successfully implemented using the Pandas library .

The experiment helped in:

Understanding how to create and store datasets
Learning how to load real-world datasets
Exploring dataset structure using various functions
Performing statistical analysis
Identifying missing and duplicate values
Thus, Pandas proves to be an essential tool for data analysis and preprocessing in real-world applications such as data science and machine learning.

Dataset used for reference:
image 1 image 2 image 3
