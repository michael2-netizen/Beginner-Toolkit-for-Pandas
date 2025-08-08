<img width="512" height="208" alt="image" src="https://github.com/user-attachments/assets/87e11b12-42be-47df-a553-aa8d2472ff55" />

 # <u>Getting Started with Pandas</u>
##  <u>1. Objective</u>:
1. Understand what Pandas is and its role in data analysis
2. Install Pandas using pip or conda
3. Test your installation by importing Pandas and loading a sample dataset

4. Learn the structure of typical Pandas workflows

5. Understand common Pandas functions: read_csv(), head(), describe(), info(), etc.
##  <u>2.Summary of the Technology</u>
**Pandas** is a powerful, open-source data analysis and manipulation library built on top of the Python programming language. It offers flexible and intuitive data structures, such as *Series* and *DataFrames*, that make working with structured (tabular) data fast and easy.

When you're dealing with data stored in formats like spreadsheets or databases, Pandas is the go-to tool. It helps streamline tasks such as **data exploration, cleaning, transformation, and analysis.**
At its core, **Pandas** provides two primary data structures:

1. **Series**: A one-dimensional labeled array.

2. **DataFrame**: A two-dimensional labeled data structure (similar to a spreadsheet or SQL table).

The **DataFrame** is the most commonly used structure and is ideal for handling tabular data.

<img width="541" height="394" alt="image" src="https://github.com/user-attachments/assets/0d0b74dd-70c2-4cbc-a91a-98f03ce933c5" />


Pandas comes with built-in support for **reading and writing** a variety of file formats and data sources, including:

CSV

Excel

SQL databases

JSON

Parquet

To load data, use functions that start with **read_, such as read_csv() or read_excel()**. Similarly, to export or store data, use functions that start with **to_, such as to_csv() or to_sql().**

<img width="1115" height="302" alt="image" src="https://github.com/user-attachments/assets/55ca6ab0-eddf-4427-8f65-84b6d5a80aff" />


*Where is it used:*

* Data cleaning and preprocessing

* Exploratory data analysis (EDA)

* Statistical modeling and visualization

* Data pipelines and automation
### Real-world Example
*Here are three real-world companies using Pandas in their data workflows:*

* **Netflix** – Analyzes user viewing data to personalize recommendations and optimize content delivery strategies.

* **Airbnb** – Uses Pandas for cleaning and analyzing property listing data, helping hosts and guests find better matches.

* **Spotify** – Leverages Pandas to process massive datasets for music recommendation systems and user behavior analytics.
##  <u>3.System Requirements</u>
|   Component                    | Requirement                           |
|   ---------------              | ------------------------------------- |
|   OS                           | Linux, macOS, or Windows              |
|   Editor                       | VS Code, Jupyter Notebook, or PyCharm |
|   Python Version               | 3.8 or higher                         |
|   Package Manager              | pip or conda                          |
|   Required Libs                | pandas, numpy, jupyter                |
## <u>4.Installation & Setup Instructions</u>
### *Step-by-Step Guide:*

* Install Pandas with pip

<img width="1600" height="232" alt="image" src="https://github.com/user-attachments/assets/36cb5780-7668-479a-9e29-760939f3b0ed" />


* (Optional) To install with additional performance dependencies:

<img width="1600" height="231" alt="image" src="https://github.com/user-attachments/assets/6ac71b36-a0ab-43e6-8ca3-5da55e61037d" />


* This installs optional dependencies like numexpr and bottleneck for faster operations on large datasets.
* **verify the installation:**
You can open a Python shell or Jupyter notebook and run the code below:

<img width="1600" height="384" alt="image" src="https://github.com/user-attachments/assets/7c5b7ecf-dad4-4d40-a823-67e518417bbb" />


## <u>5.Working With Pandas Example</u>
For our first example, we will use a CSV file containing the Ames Housing dataset—a real estate dataset—to demonstrate the functionality of the pandas library in Python programming.
### step 1: Import pandas 
We start by importing the `pandas` library, which is commonly used for data manipulation and analysis.
#importing pandas as pd
### step 2: Load the Dataset
We load the CSV file named ames.csv into a pandas DataFrame. This file should be located in your working directory.
#Load the dataset
### Step 3: Preview the Data
We use df.head() to view the first 5 rows of the dataset. This gives us a quick glimpse of what the data looks like. We can also use df.tail() to view the last 5 rows of the dataset.
### Step 4: View Column Names
To understand the structure of the dataset, we print out all the column names using df.columns.tolist().
* Data Exploration

| Function        | Description                                                 |
|----------------|-------------------------------------------------------------|
| `df.head(n)`    | First n rows (default 5)                                    |
| `df.tail(n)`    | Last n rows                                                 |
| `df.info()`     | Summary of DataFrame: columns, dtypes, non-null counts      |
| `df.describe()` | Statistical summary (mean, std, etc. for numeric columns)   |
| `df.shape`      | Returns (rows, columns)                                     |
| `df.columns`    | List of column names                                        |
| `df.dtypes`     | Data types of each column                                   |
| `df.sample(n)`  | Random sample of n rows                                     |
| `df.nunique()`  | Count of unique values per column                           |
* Data Selection / Filtering

| Syntax                               | Description                     |
| ------------------------------------ | ------------------------------- |
| `df['Column']`                       | Select a single column          |
| `df[['Col1', 'Col2']]`               | Select multiple columns         |
| `df.iloc[0]`                         | Row by index (integer location) |
| `df.loc[0]`                          | Row by label/index name         |
| `df[df['Col'] > 100]`                | Filter rows by condition        |
| `df[(df['A'] > 5) & (df['B'] < 10)]` | Multiple conditions             |
### Step 5: Cleaning the Data

Before performing any analysis, it's important to inspect and clean the data. This includes handling missing values, removing duplicates, and converting data types if necessary.

#### Check for Missing Values
When dealing with very many missing values in one column that's not important for your analysis, the best action is to drop the entire column.
Below are a few more functions for data cleaning using the pandas library:
* Data Cleaning

| Function               | Description                     |
| ---------------------- | ------------------------------- |
| `df.isnull()`          | Detect missing values           |
| `df.isnull().sum()`    | Count missing values per column |
| `df.dropna()`          | Drop rows with missing values   |
| `df.fillna(value)`     | Fill missing values             |
| `df.duplicated()`      | Check for duplicate rows        |
| `df.drop_duplicates()` | Remove duplicate rows           |
| `df.replace(a, b)`     | Replace values                  |
This provides a basic foundation for exploring and analyzing structured data using pandas.
## <u> 6.AI Prompt Journal</u>
AI Prompt Journal

1. **Using AI to Comprehend Existing Codebase Prompts**

Prompt Used:

"Explain what this Pandas script does line by line."

[Link to curriculum for the prompt](https://ai.moringaschool.com/ai-software/ai-use-cases/usecases-comprehend/#_1_understanding_existing_code_functionality)

Response Summary:
The AI broke down each line, explaining data loading, inspection, and cleaning.

Reflection:
Very helpful for understanding unfamiliar Pandas scripts.


2. **Using AI to Debug Code**

Prompt Used:

"Why does my Pandas code return 'KeyError: Column not found' when I try df['total_bill']?"

[Link to curriculum for the prompt](https://ai.moringaschool.com/ai-software/ai-use-cases/usecases-debugging/#_tracing_error_messages_and_stack_traces)

Response Summary:
The AI explained that column names may have typos or trailing spaces. It suggested using df.columns to verify names.

Reflection:
Quickly identified and resolved a common beginner issue. Saved time that would’ve been spent searching Stack Overflow.


3. **Using AI to Refactor and Enhance Code**

Prompt Used:

"Refactor this code to include missing value handling."

[Link to curriculum for the prompt](https://ai.moringaschool.com/ai-software/ai-use-cases/usecases-refactor/#_understanding_code_refactoring_with_ai)

AI Response Summary:
The AI suggested adding a missing value check, .dropna() if needed.

## <u> 7.Common Issues & Fixes </u>
| Issue                 | Error Message                                   | Fix                                                   |
| --------------------- | ----------------------------------------------- | ----------------------------------------------------- |
| Typo in column name   | `KeyError: 'totl_bill'`                         | Check spelling using `df.columns`                     |
| File not found        | `FileNotFoundError`                             | Ensure file path is correct or use a public dataset   |
| Missing package       | `ModuleNotFoundError: No module named 'pandas'` | Install using `pip install pandas`                    |
| Jupyter not launching | Server error or command not found               | Ensure Jupyter is installed and in PATH, or reinstall |
