# Diwali Sales Data Analysis

## Project Overview

This project performs data cleaning and exploratory data analysis (EDA)
on Diwali sales data using Python. The analysis explores customer
demographics, purchasing behaviour, state-wise sales, occupation-wise
sales, and product-category performance.

The goal is to identify patterns in customer purchases and understand
which customer groups, locations, occupations, and product categories
contribute to sales.

## Project Objectives

-   Load and understand the Diwali sales dataset.
-   Identify and remove duplicate records.
-   Check missing values and handle the `Amount` column.
-   Convert the `Amount` column to an integer data type.
-   Remove columns that are not used in the analysis.
-   Standardize the values in the `Gender` column.
-   Explore customer demographics and purchasing behaviour.
-   Analyze sales and orders by state, occupation, and product category.
-   Create visualizations to communicate the findings.

## Dataset

**Dataset file:** `Diwali Sales Data.csv`

The notebook uses the following columns in its analysis:

-   `User_ID`
-   `Cust_name`
-   `Product_ID`
-   `Gender`
-   `Age Group`
-   `Age`
-   `Marital_Status`
-   `State`
-   `Zone`
-   `Occupation`
-   `Product_Category`
-   `Orders`
-   `Amount`

The dataset is loaded with Pandas using `encoding='latin1'`.

## Tools and Libraries

-   **Python** -- programming language.
-   **Pandas** -- data loading, cleaning, grouping, and aggregation.
-   **Matplotlib** -- chart creation.
-   **Seaborn** -- statistical and categorical visualizations.
-   **Jupyter Notebook** -- development environment.

## Data Cleaning

The notebook performs the following preparation steps:

1.  Checks the dataset structure, columns, sample records, and data
    types.
2.  Checks for duplicate records and removes them using
    `drop_duplicates()`.
3.  Checks missing values using `isnull().sum()`.
4.  Calculates the mean of `Amount` and fills missing `Amount` values
    with that mean.
5.  Converts `Amount` to integer data type.
6.  Removes the `Status` and `unnamed1` columns.
7.  Replaces `F` with `Female` and `M` with `Male` in the `Gender`
    column.

**Data preparation note:** The notebook's initial notes mention missing
values in `Orders`, `Amount`, `Status`, and unnamed columns. The code
explicitly fills missing values in `Amount` and removes `Status` and
`unnamed1`. It does not show a separate missing-value treatment for
`Orders`.

## Exploratory Data Analysis

The notebook includes the following analyses:

### Customer and Gender Analysis

-   Customer count by gender.
-   Total sales amount by gender.
-   Customer count by age group and gender.
-   Total sales amount by age group.

### State Analysis

-   Total orders by state.
-   Total sales amount by state.

### Occupation Analysis

-   Total sales amount by occupation.

### Product Category Analysis

-   Total sales amount by product category.
-   Top 10 product categories by number of orders.
-   Product-category distribution by gender.
-   Top 10 product categories by sales amount.

## Key Findings

The written observations in the notebook report the following:

-   Female customers are more numerous than male customers.
-   Female customers generate higher sales than male customers.
-   The 26--35 age group has the highest customer count among male and
    female customers.
-   The 26--35 age group contributes the highest sales, followed by the
    36--45 age group.
-   Uttar Pradesh has the highest number of orders, followed by
    Maharashtra and Karnataka.
-   The notebook's final observations identify Uttar Pradesh as the
    state with the highest sales; Maharashtra and Karnataka are also
    among the leading states.
-   Customers working in the IT sector contribute the highest sales
    among occupations, followed by Healthcare and Aviation.
-   The Food product category contributes the highest sales, followed by
    Clothing & Apparel.
-   The Food category receives the highest number of orders.

These findings reflect the observations written in the notebook. Exact
totals and percentages are not included here.

## How to Run the Project

1.  Download or clone this repository.

2.  Keep `Diwali Sales Data.csv` in the same folder as the notebook, or
    update the CSV file path in the notebook.

3.  Install the required libraries:

    ``` bash
    pip install pandas matplotlib seaborn jupyter
    ```

4.  Start Jupyter Notebook:

    ``` bash
    jupyter notebook
    ```

5.  Open `sales_analysis_project(5).ipynb`.

6.  Run the notebook cells from top to bottom.

## Project Structure

``` text
Diwali-Sales-Analysis/
│
├── Data/
│   ├── Diwali Sales Data.csv
│   └── sales_analysis_project.ipynb
│
├── Documentation/
│   └── Diwali_Sales_Analysis_Documentation.docx
│
└── README.md

Update the folder or file names in this structure if your repository
uses different names.

## Conclusion

This project demonstrates a Python-based data analysis workflow,
including data loading, cleaning, grouping, aggregation, and
visualization. The analysis highlights customer purchasing patterns and
compares sales across age groups, states, occupations, and product
categories. The findings can help describe customer behaviour and the
sales categories that performed strongly in the analyzed dataset.


