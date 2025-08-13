# Walmart-data-Analysis-etl


<img width="1598" height="753" alt="walmart_project-piplelines" src="https://github.com/user-attachments/assets/6e49f1c9-e260-43a7-bd8f-d1f124d2d388" />


## Project Overview

This project is an end-to-end data analysis solution designed to extract critical business insights from Walmart sales data. I utilize Python for data processing and analysis, SQL for advanced querying, and structured problem-solving techniques to solve key business questions. The project is ideal for data analysts looking to develop skills in data manipulation, SQL querying, and data pipeline creation.

---

## Project Steps

### 1. Set Up the Environment
   - **Tools Used**: Visual Studio Code (VS Code), Python, SQL (MySQL and PostgreSQL)
   - **Goal**: Created a structured workspace within VS Code and organized project folders for smooth development and data handling.

### 2. Set Up Kaggle API
   - **API Setup**: Obtained Kaggle API token from [Kaggle](https://www.kaggle.com/) by navigating to my profile settings and downloaded the JSON file.
   - **Configure Kaggle**: 
      - Placed the downloaded `kaggle.json` file in my local `.kaggle` folder.

### 3. Download Walmart Sales Data
   - **Data Source**: Used the Kaggle API to download the Walmart sales datasets from Kaggle.
   - **Dataset Link**: [Walmart Sales Dataset](https://www.kaggle.com/najir0123/walmart-10k-sales-datasets)
   - **Storage**: Saved the data in the `data/` folder for easy reference and access.


### 4. Explore the Data
   - **Goal**: Conducted an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
   - **Analysis**: Used functions like `.info()`, `.describe()`, and `.head()` to get a quick overview of the data structure and statistics.

### 5. Data Cleaning
   - **Remove Duplicates**: Identified and removed duplicate entries to avoid skewed results.
   - **Handle Missing Values**: Droped rows or columns with missing values that are insignificant; filled values where essential.
   - **Fix Data Types**: Ensured all columns have consistent data types (e.g., dates as `datetime`, prices as `float`).
   - **Currency Formatting**: Use `.replace()` to handle and format currency values for analysis.
   - **Validation**: Checked for any remaining inconsistencies and verify the cleaned data.

### 6. Feature Engineering
   - **Create New Columns**: Calculated the `Total Amount` for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.
   - **Enhance Dataset**: Adding this calculated field will streamline further SQL analysis and aggregation tasks.

### 7. Load Data into MySQL and PostgreSQL
   - **Set Up Connections**: Connected to MySQL and PostgreSQL using `sqlalchemy` and load the cleaned data into each database.
   - **Table Creation**: Set up tables in both MySQL and PostgreSQL using Python SQLAlchemy to automate table creation and data insertion.
   - **Verification**: Run initial SQL queries to confirm that the data has been loaded accurately.

### 8. SQL Analysis: Complex Queries and Business Problem Solving
   - **Business Problem-Solving**: Wrote  and executed complex SQL queries to answer critical business questions, such as:
     - Revenue trends across branches and categories.
     - Identifying best-selling product categories.
     - Sales performance by time, city, and payment method.
     - Analyzing peak sales periods and customer buying patterns.
     - Profit margin analysis by branch and category.
       
   

## Requirements

- **Python 3.8+**
- **SQL Databases**: MySQL, PostgreSQL
- **Python Libraries**:
  - `pandas`, `numpy`, `sqlalchemy`, `mysql-connector-python`, `psycopg2`
- **Kaggle API Key** (for data downloading)
  

---

## Results and Insights
       
- **Sales Insights**: Key categories, branches with highest sales, and preferred payment methods.
- **Profitability**: Insights into the most profitable product categories and locations.
- **Customer Behavior**: Trends in ratings, payment preferences, and peak shopping hours.
