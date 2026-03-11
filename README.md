# E-commerce Sales Data Cleaning and Analysis

## Project Overview

This project analyzes a messy e-commerce sales dataset containing approximately **30,000 transactions**.  
The goal of the project was to clean inconsistent and incomplete data and perform exploratory data analysis (EDA) to uncover meaningful business insights.

The dataset initially contained multiple data quality issues including duplicate records, inconsistent date formats, mixed currency formats, missing values, and inconsistent text fields. These issues were resolved using data cleaning techniques in Python before performing analysis and visualization.


## Dataset Description

The dataset contains transactional information including:

- Order ID  
- Order Date  
- Customer Name  
- Email Address  
- Phone Number  
- Product  
- Quantity  
- Unit Price  
- Discount  
- Total Amount  
- Order Status  
- Shipping Address  
- City  
- State  
- ZIP Code  

Two versions of the dataset are included in this repository:

- **raw_sales_sample.csv** → Sample of the original messy dataset  
- **clean_sales_data.csv** → Final cleaned dataset used for analysis

---

## Data Cleaning Steps

Several preprocessing steps were performed to improve the quality of the dataset:

### 1. Duplicate Removal
Duplicate transactions were detected and removed to ensure accurate analysis.

### 2. Date Standardization
The dataset contained multiple date formats. All dates were converted into a consistent datetime format.

### 3. Text Normalization
Customer names, emails, cities, states, and order statuses had inconsistent casing. These fields were standardized.

### 4. Currency Cleaning
Price fields contained currency symbols and commas. These values were cleaned and converted into numeric format.

### 5. Discount Formatting
Discount values stored as percentage strings were converted into numeric values.

### 6. Phone Number Standardization
Phone numbers stored in multiple formats were cleaned and standardized.

### 7. Missing Value Handling
Missing values were handled appropriately depending on the column and context.

---

## Feature Engineering

Additional features were created to support deeper analysis:

- **Revenue = Unit Price × Quantity**
- **Year extracted from order date**
- **Month extracted from order date**

These features allowed the analysis of seasonal sales patterns and revenue trends.

---

## Exploratory Data Analysis

The following analyses were performed:

- Product performance analysis
- Revenue distribution analysis
- Geographic sales distribution
- Customer purchasing behavior
- Seasonal sales trends

---

## Key Insights

- The top 3 products — Standing Desk, Ergonomic Chair, and Streaming Mic Bundle account for nearly 40% of total revenue, revealing a strong concentration in high    ticket office furniture and equipment.
- Revenue is geographically skewed, with TX and CA alone contributing over 20% of total sales, while the remaining 18 states split the rest.
- December accounts for a disproportionate share of annual revenue, dwarfing every other month and suggesting a strong end of year purchasing spike driven by        holiday or budget flush buying.
- Over half of all orders (57%) include a discount, indicating heavy reliance on promotions to drive conversions across the customer base.
- Repeat buyers represent just 55% of customers yet drive 77% of total revenue, making customer retention the single most important lever for sustaining sales       performance.

---

## Visualizations

The project includes visualizations to highlight important patterns in the data:

- Revenue by Product
- Monthly Sales Trend
- Revenue Distribution
- Sales by State
- Discount Impact on Revenue
- Top Customers by Revenue

These visualizations help identify trends, top-performing products, and customer behavior.

## Tools Used
- Python  
- Pandas  
- Matplotlib  
- Seaborn  

## Repository Structure

```
ecommerce-sales-analysis
│
├── data
│   ├── raw_sales_sample.csv
│   └── clean_sales_data.csv
│
├── notebook
│   └── sales_analysis.ipynb
│
├── visuals
│   ├── revenue_by_product.png
│   ├── monthly_sales_trend.png
│   └── sales_by_state.png
│
└── README.md


## How to Run the Project

1. Clone the repository
2. Open the notebook in Jupyter Notebook or Google Colab
3. Install the required Python libraries
4. Run the notebook cells sequentially to reproduce the analysis

---

## Purpose of the Project

This project demonstrates key data analyst skills including:

- Data cleaning and preprocessing
- Exploratory data analysis
- Data visualization
- Business insight generation
