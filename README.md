# Walmart Sales Analysis Project

## Overview
This project is an end-to-end data analysis on Walmart's sales data, where I applied Python and SQL to uncover critical business insights. By leveraging advanced data manipulation and querying techniques, I was able to answer key business questions related to Walmart's sales performance. This project showcases my skills in data cleaning, SQL querying, feature engineering, and pipeline creation, and it demonstrates my ability to structure and analyze large datasets for actionable insights.

## Project Workflow

### 1. Project Setup
- **Environment**: I structured the project within Visual Studio Code (VS Code) using Python and SQL (MySQL and PostgreSQL).
- **Data Source**: The Walmart sales dataset was sourced from Kaggle, with the Kaggle API set up to automate data download directly into the project directory.
- **Libraries Used**: I utilized `pandas`, `numpy`, `sqlalchemy`, and SQL connectors to work seamlessly with both MySQL and PostgreSQL databases.

### 2. Data Loading and Exploration
- **Data Loading**: Loaded the Walmart sales dataset into a Pandas DataFrame.
- **Exploratory Analysis**: Used `.info()`, `.describe()`, and `.head()` functions to understand data structure, assess column data types, and check for missing values.
- **Observations**: Identified initial issues such as missing values, inconsistent data types, and potential duplicate records that could impact analysis accuracy.

### 3. Data Cleaning
- **Duplicate Removal**: Removed duplicate entries to ensure data accuracy.
- **Handling Missing Values**: Used targeted imputation and row/column removal where necessary to handle missing values.
- **Data Type Consistency**: Ensured all columns had appropriate data types, converting date columns to `datetime` format and price columns to `float`.
- **Currency Formatting**: Standardized currency formats for consistency in financial calculations.

### 4. Feature Engineering
- **New Features**: Created a `Total_Amount` column by calculating `unit_price * quantity` to represent total revenue per transaction.
- **Purpose**: This feature facilitated deeper sales analysis by allowing aggregation and comparisons across different products, categories, and branches.
  
### 5. Data Upload to SQL Databases
- **Database Setup**: Established connections with MySQL and PostgreSQL using SQLAlchemy and set up tables for the cleaned data.
- **Data Loading**: Uploaded the transformed dataset into both databases to enable SQL-based analysis and comparisons.
- **Verification**: Conducted initial SQL queries to confirm data accuracy post-upload.

### 6. SQL Analysis: Solving Business Problems
Using SQL, I addressed the following key business questions:

#### 6.1 Revenue Trends Across Branches and Categories
   - **Objective**: Identify which branches and product categories generate the most revenue.
   - **Solution**: Aggregated sales by branch and category, revealing that certain branches consistently outperform others in specific categories. This insight helps prioritize high-performing locations and product lines.

#### 6.2 Identifying Best-Selling Product Categories
   - **Objective**: Determine which categories drive the majority of sales.
   - **Solution**: Created queries to rank categories by total sales volume, identifying the top 5 best-sellers. This analysis helps in inventory management and targeted marketing strategies.

#### 6.3 Sales Performance by Time, City, and Payment Method
   - **Objective**: Understand customer behavior across different times, locations, and payment preferences.
   - **Solution**: Performed temporal analysis by day and month to spot peak shopping periods, observed differences in city-wise sales performance, and assessed payment method preferences. This provides insights into customer patterns that can influence staffing and promotions.

#### 6.4 Analyzing Peak Sales Periods and Customer Buying Patterns
   - **Objective**: Identify trends in customer buying behavior to optimize stock and staff scheduling.
   - **Solution**: Leveraged SQL window functions to analyze time-based trends, revealing peak hours and seasonal shopping behaviors. This can aid in better resource allocation during high-demand periods.

#### 6.5 Profit Margin Analysis by Branch and Category
   - **Objective**: Determine the most profitable branches and product categories.
   - **Solution**: Calculated profit margins across branches and categories, highlighting the most lucrative areas. This information can support strategic decision-making for expanding high-margin product lines.

### 7. Key Insights and Results

- **High-Performing Branches and Products**: Branches WALM001 and WALM002 were found to have the highest revenue and profit margins, particularly in categories A and B, suggesting targeted marketing and inventory strategies.
- **Customer Preferences**: Weekends and late afternoons saw the highest footfall, with a preference for credit card payments. This insight can be leveraged for time-sensitive promotions and staff planning.
- **Sales Patterns**: Top product categories included electronics, home goods, and seasonal items, which could inform product placement and seasonal promotions.
- **Profit Optimization**: Profit margins varied significantly by category, indicating opportunities for re-evaluating pricing or supplier negotiations for lower-margin items.

### 8. Documentation and Publishing

- **Documentation**: Maintained clear and detailed documentation throughout the project to ensure reproducibility. Each query and step is explained with its objective, approach, and results.
- **GitHub Publishing**: The project is hosted on GitHub with all essential components:
  - `README.md` (this document)
  - SQL query scripts
  - Python scripts for data loading and cleaning
  - Jupyter Notebook for Python-based analysis (optional)
  
## Results and Insights

This section summarizes the actionable insights derived from the analysis:

1. **Revenue Trends**: Branches and categories that drive revenue the most, offering strategic insights for scaling operations.
2. **Customer Behavior**: Time-based shopping patterns and preferred payment methods, useful for staff and stock management.
3. **Profitability**: High-profit categories and branches identified for targeted investment and marketing.

## Future Enhancements

Potential extensions to enhance this project include:

- Integration with a dashboard tool (e.g., Power BI or Tableau) for dynamic, interactive data visualization.
- Expanding the dataset with additional factors, such as customer demographics or competitor data, for a more comprehensive analysis.
- Automating the data pipeline to enable real-time analysis and reporting.




