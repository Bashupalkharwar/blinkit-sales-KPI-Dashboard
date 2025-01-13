# blinkit-sales-KPI-Dashboard
# Project Overview:
This Power BI dashboard offers a detailed analysis of Blinkit, India's leading last-minute delivery app. By focusing on sales data, item specifics, and outlet performance, the project aims to provide actionable insights through comprehensive data cleaning, modeling, and visualization techniques.
Steps for Building the Power BI Dashboard
# Steps for Building the Power BI Dashboard

# 1. Requirement Gathering / Business Understanding
- **Objective:** Conduct a comprehensive analysis of Blinkit’s:
- Sales Prformance
- Customer satisfaction
-	Inventory distribution
-	Identify opportunities for optimization using KPIs and visualizations.

**Key KPIs to Track:**
- Total Sales
- Average Sales
- Number of Items Sold
- Average Rating


**2. Data Walkthrough**
  - Load and explore the dataset in Power BI.
  -	Objectives:

   	- Understand the dataset structure, including:
       - 	Column names
       - 	Data types
       - 	Missing or invalid data
    -	Identify relationships and fields for calculated columns/measures.
      
**Example columns** to expect in the dataset:
- Sales, Item Type, Fat Content, Outlet Size, Outlet Type, Rating, Outlet Establishment Year, etc.


**3. Data Connection**
-	Import the dataset into Power BI.
    -	Source: Excel, CSV, SQL Database, or any other data source.
    -	Use Home > Get Data option to connect your data source.

**4. Data Cleaning / Quality Check (Power Query Editor)**
	**Steps:**
- Remove Empty Rows/Columns: Filter out unnecessary data.
-	Handle Missing Values: Use data imputation or remove null values.
-	Change Data Types: Ensure columns like Sales (Currency), Rating (Decimal), etc., are assigned correct data types.
-	Filter Data: Keep relevant rows/fields.
- Transform Columns:
    - Extract Year from the establishment date.
    - Split concatenated fields if any.
-	Note: Save these changes in the Applied Steps section.


**5. Data Modeling**
**Steps:**
-	Create relationships between tables (if applicable).
Example: Link Sales to Outlet and Item Type.
-	Use Star Schema for efficient analysis.
-	Define Primary and Foreign Keys.
-	Ensure relationships are set to One-to-Many for better filtering.

**6. DAX Calculations**
- Write custom measures to calculate KPIs:
    - **Total Sales:**
    - Total_sales = SUM('BlinkIT Grocery Data'[Sales])
