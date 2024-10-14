# Sales Analysis Project

### By Tara Danneman

## Project Overview

AAL, a prominent Australian clothing brand since 2000, is expanding its business and needs assistance from the Head of Sales and Marketing (S&M) to make informed investment decisions. The tasks include identifying high-revenue states and creating sales programs for low-revenue states. This project involves analyzing the company's Q4 sales data in Australia, state by state, to provide data-driven insights for decision-making in the next year.

## Table of Contents

- [Project Overview](#project-overview)
- [Project Statement](#project-statement)
- [Data Analysis Steps](#data-analysis-steps)
- [Data Visualization](#data-visualization)
- Dependencies
- [How to Run](#how-to-run)

## Project Statement

AAL seeks to identify high-revenue states and create sales programs for low-revenue states. The analysis of Q4 sales data will provide insights to help the Head of Sales and Marketing make informed investment decisions for the next year.

## Data Analysis Steps

### Step 1: Preliminary Analysis

1. **Import Libraries and Data:**
   - Import necessary libraries such as pandas, numpy, datetime, matplotlib, and seaborn.
   - Load the dataset from an Excel file.

2. **Check for Null Values:**
   - Use `isnull()` and `notna()` methods to check for null values in the dataset.

3. **Handle Null Values:**
   - Although there are no null values in the dataset, options for handling null values are provided.

4. **Data Wrangling:**
   - Use `df.info()` to understand the data structure.
   - Normalize the 'Sales' column using Min-Max scaling to identify high and low revenue states.

5. **GroupBy Analysis:**
   - Group data by 'State' and perform aggregation to get statistical insights.
   - Group data by 'month' and 'State' to analyze sales trends over time.

### Step 2: Descriptive Statistical Analysis

1. **Descriptive Statistics:**
   - Perform descriptive statistical analysis on 'Sales' and 'Unit' columns.

2. **Identify High and Low Sales Groups:**
   - Determine which group and state are generating the highest and lowest sales.

3. **Generate Reports:**
   - Generate weekly, monthly, and quarterly reports using the [`groupby`](command:_github.copilot.openSymbolFromReferences?%5B%22%22%2C%5B%7B%22uri%22%3A%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Ftarad%2FOneDrive%2FDocuments%2FAI%20ML%20Class%2FNotebooks%2FFinal_Sales_Analysis_Project.ipynb%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%2C%22pos%22%3A%7B%22line%22%3A408%2C%22character%22%3A22%7D%7D%5D%2C%2225a7581d-9cfe-4801-9a1e-4eeccc0da7ff%22%5D "Go to definition") function.

## Data Visualization

### Step 3: Visualization

1. **Total Revenue by Day, Week, and Month:**
   - Use seaborn and matplotlib to create bar plots showing total revenue broken down by day, week, and month.

2. **Revenue Breakdown by State:**
   - Visualize the revenue breakdown for each state during the 4th Quarter, highlighting Victoria as the top revenue generator and Western Australia as the lowest.

## Dependencies

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## How to Run

1. **Clone the repository:**
   ```sh
   git clone <repository-url>
   ```
2. **Navigate to the project directory:**
   ```sh
   cd <project-directory>
   ```
3. **Install the required dependencies:**
   ```sh
   pip install -r requirements.txt
   ```
4. **Run the Jupyter Notebook:**
   ```sh
   jupyter notebook FINAL_SALES_ANALYSIS_PROJECT.ipynb
   ```

Feel free to explore the notebook and modify the code as needed to further analyze and visualize the data.
 

