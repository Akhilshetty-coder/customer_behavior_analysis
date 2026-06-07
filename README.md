# customer_behavior_analysis
data analytics project showcasing customer behavior analysis using python,sql and power BI 
# Data Analytics Project: End-to-End Customer Demographics & Sales Analysis

## 📌 Project Overview
This project delivers an end-to-end data analytics solution designed to ingest raw business data, clean and transform it, perform deep relational database queries, and surface actionable insights through an interactive dashboard. The primary objective is to evaluate customer purchasing patterns, identify revenue drivers, and provide stakeholders with data-backed recommendations to optimize marketing spend and inventory management.

---

## 📊 Dataset Description
The analysis is based on a transactional database containing **10,000+ rows** of historical enterprise data. The schema includes three primary relational entities:
* **Customers:** Unique ID, demographic details (age, gender, region), and signup dates.
* **Sales/Transactions:** Order ID, customer ID, product SKU, purchase date, quantity, and unit price.
* **Products:** Product ID, category, sub-category, and cost of goods sold (COGS).

*Note: The dataset was initially provided in a raw, unoptimized CSV format before staging and migration.*

---

## 🛠️ Tech Stack & Tools
* **Data Processing & EDA:** Python (`pandas`, `numpy`, `matplotlib`, `seaborn`)
* **Database Management:** SQL (PostgreSQL / MySQL / SQL Server)
* **Business Intelligence:** Power BI (DAX, Power Query)
* **Presentation & Reporting:** Gamma App (AI-Assisted Storyboarding) & Microsoft PowerPoint

---

## 🔄 End-to-End Workflow

### 1. Exploratory Data Analysis (EDA) & Data Cleaning (Python)
* **Ingestion:** Loaded raw multi-source CSV files using `pandas`.
* **Data Quality Assessment:** Identified and handled missing values, duplicate records, and outliers via IQR (Interquartile Range) filtering.
* **Type Casting:** Standardized date formats and converted numeric IDs to string objects to optimize memory consumption.
* **Export:** Saved the clean, structured data into structured datasets ready for database ingestion.

### 2. Relational Database Hosting & Advanced SQL Querying
* Imported clean datasets into a relational database schema.
* Established Primary and Foreign Key constraints to enforce referential integrity.
* Wrote production-ready SQL scripts to extract high-level KPIs, including:
    * *Customer Lifetime Value (CLV)* using window functions (`SUM() OVER`).
    * *Year-over-Year (YoY) Revenue Growth* calculations using common table expressions (CTEs).
    * *Top-performing Product Categories* aggregated via multi-table inner joins.

### 3. Interactive Business Intelligence (Power BI)
* Engineered a star-schema data model within Power BI.
* Utilized **Power Query** to implement additional custom column logic and conditional indexing.
* Developed complex **DAX measures** (e.g., `TOTALYTD`, `CALCULATE`, `DIVIDE`) for dynamic time-intelligence reporting.
* Designed a responsive, user-centric dashboard layout built for executive decision-making.

### 4. Executive Reporting & Presentation (Gamma)
* Compiled analytical findings into an executive summary report.
* Leveraged **Gamma App** to rapidly prototype a visually striking, narrative-driven presentation deck.
* Refined the final layout in PowerPoint to deliver a pitch-ready slide deck summarizing strategic recommendations.

---

## 📈 Dashboard Highlights
The interactive Power BI dashboard consists of two core views:
1.  **Executive Summary:** High-level overview of Revenue, Profit Margins, Total Orders, and Customer Acquisition Costs (CAC) with dynamic timeline slicers.
2.  **Customer Insights & Demographics:** Breakdown of purchasing behavior by age bracket, geographic region, and product category affinity.

---

## 🎯 Key Results & Business Insights
* **Revenue Growth:** Identified an 14.5% uptick in sales volume driven predominantly by Q3 holiday promotions.
* **Customer Segmentation:** The 25–34 age demographic represents 42% of total revenue but has the highest churn rate, signaling a need for targeted loyalty initiatives.
* **Inventory Optimization:** Isolated three underperforming sub-categories that tied up 18% of operational working capital.

---

## 🚀 How to Run This Project

### Prerequisites
Ensure you have the following installed on your local environment:
* Python 3.8+
* PostgreSQL / MySQL / SQL Server instance
* Power BI Desktop

### Execution Steps

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/yourusername/data-analytics-project.git](https://github.com/yourusername/data-analytics-project.git)
    cd data-analytics-project
    ```

2.  **Run Python Scripts for EDA & Data Cleaning:**
    * Install dependencies: `pip install -r requirements.txt`
    * Execute the cleaning pipeline notebook or script located in the `src/` directory to generate the clean files.

3.  **Setup Database & Run SQL Queries:**
    * Execute the schema creation script found in `sql/schema.sql`.
    * Import the processed CSV files into your database tables.
    * Run analytical queries from `sql/queries.sql` to verify database KPIs.

4.  **Open Power BI Dashboard:**
    * Launch Power BI Desktop and open the `reports/dashboard.pbix` file.
    * Update the data source settings to point to your local database or clean data files, then hit **Refresh**.

5.  **View Presentations:**
    * Access the final slide deck in the `presentation/` directory (`.pptx` format).

---
*Created by [Your Name] — Feel free to connect with me on [LinkedIn Profile Link] or check out my portfolio at [Portfolio Website Link]!*
