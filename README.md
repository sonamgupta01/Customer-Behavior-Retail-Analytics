# RetailPulse — Customer Shopping & Retail Analytics

An end-to-end data analytics project that explores customer shopping patterns, purchase behavior, product preferences, and spending trends using Python, PostgreSQL, SQL, and Power BI.

## Overview

RetailPulse transforms raw customer shopping data into meaningful insights that can help businesses understand their customers, evaluate purchasing patterns, and make data-driven retail decisions.

The project follows a complete analytics workflow, starting with data exploration and cleaning in Python, continuing with SQL analysis in PostgreSQL, and ending with an interactive Power BI dashboard and a presentation of key findings.

## Dataset

The dataset contains **3,900 customer shopping records** and includes information such as:

- Customer demographics: age and gender
- Product details: purchased items, categories, sizes, colors, and seasons
- Purchase information: purchase amounts and previous purchases
- Customer feedback: review ratings
- Shopping preferences: purchase frequency and payment methods
- Retail services: subscription status, discounts, and shipping types

## Tech Stack

- **Python:** Pandas, data exploration, data cleaning, and feature engineering
- **PostgreSQL:** Database management and structured data storage
- **SQL:** Data analysis, aggregations, filtering, grouping, and comparisons
- **Power BI:** Interactive dashboard development and data visualization
- **Jupyter Notebook:** Python development and analysis

## Project Workflow

### 1. Python — Data Exploration and Cleaning

Loaded the shopping dataset into Pandas and explored its structure, data types, summary statistics, and missing values.

Key activities:
- Inspected the dataset using `head()`, `info()`, and `describe()`.
- Identified missing values in customer review ratings.
- Handled missing review ratings using the median rating within each product category.
- Standardized column names for easier database and SQL operations.
- Created age groups to compare shopping behavior across customer segments.
- Converted purchase frequency into an approximate number of days.
- Removed a redundant promotional-code column after checking that it duplicated the discount-applied information.

### 2. PostgreSQL — Database Storage

Connected Python to PostgreSQL using SQLAlchemy and Psycopg2.

Key activities:
- Created and used the `customer_behavior` database.
- Loaded the cleaned dataset into a PostgreSQL table named `customer`.
- Prepared the data for structured querying and further analysis.

### 3. SQL — Customer and Retail Analysis

Used SQL queries to investigate customer purchasing patterns and compare retail metrics.

Analysis areas included:
- Identifying popular product categories and purchased items.
- Comparing average purchase amounts across shipping types.
- Examining customer review ratings by product.
- Comparing purchasing behavior between subscribers and non-subscribers.
- Exploring customer spending patterns and purchase frequency.

SQL concepts used include `SELECT`, `WHERE`, `GROUP BY`, aggregate functions, `ORDER BY`, and `LIMIT`.

### 4. Power BI — Interactive Dashboard

Built an interactive dashboard to present shopping trends and customer insights visually.

Dashboard analysis areas include:
- Customer distribution by age group and gender.
- Purchase patterns across product categories.
- Customer subscription status.
- Shopping preferences and product performance.
- Comparisons of purchase amounts and customer ratings.

Interactive slicers help users explore the data by relevant customer and shopping attributes.


## Key Learnings

- Performed exploratory data analysis and data cleaning using Python.
- Practiced SQL-based analysis on a PostgreSQL database.
- Connected Python, PostgreSQL, and Power BI within one analytics workflow.
- Designed interactive visualizations to communicate analytical findings.
- Developed an end-to-end understanding of how raw data can be transformed into business insights.

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries: `pandas`, `sqlalchemy`, and `psycopg2-binary`.
3. Open the Jupyter Notebook and update the dataset path.
4. Run the notebook cells to explore, clean, and prepare the data.
5. Configure PostgreSQL and update the database connection settings using your own credentials.
6. Execute the SQL analysis queries in PostgreSQL.
7. Open the Power BI report and configure the database connection if required.
8. Review the dashboard and project presentation.

## Project Structure

```text
retail-pulse/
├── Customer_Shopping_Behaviour_Analysis.ipynb
├── customer_shopping_behavior.csv
├── sql_queries.sql
├── RetailPulse_Dashboard.pbix
└── README.md
```


## Conclusion

RetailPulse demonstrates an end-to-end retail analytics workflow by combining Python-based data preparation, PostgreSQL data storage, SQL analysis, and Power BI visualization. It showcases practical data analytics skills and the ability to turn customer shopping data into clear, actionable business insights.
