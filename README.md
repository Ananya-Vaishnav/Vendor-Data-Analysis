# 📊 Vendor Performance Analysis

This project analyzes vendor performance data using **Python (EDA, SQLAlchemy, Pandas)** and creates a professional **Power BI dashboard** to visualize insights.  
It covers the complete workflow from data ingestion to visualization.

---

## 🚀 Project Workflow

1. **Data Ingestion**
   - Connected to a PostgreSQL database (`inventory_db`).
   - Extracted data from multiple CSVs (`purchases.csv`, `sales.csv`, `vendor_invoice.csv`, etc.).
   - Loaded data into database tables using `ingestion_db.py`.

2. **Data Transformation**
   - Created a vendor sales summary (`vendor_sales_summary`) using SQL queries.
   - Cleaned and enriched the dataset in Python:
     - Removed whitespace
     - Handled missing values
     - Calculated new metrics:
       - **Gross Profit**
       - **Profit Margin**
       - **Stock Turnover**
       - **Sales-to-Purchase Ratio**

3. **Exploratory Data Analysis (EDA)**
   - Performed EDA in Jupyter Notebooks (`EDA.ipynb`, `Vendor Performance Analysis.ipynb`).
   - Used **Pandas, Matplotlib, Seaborn** for analysis & visualization.

4. **Visualization with Power BI**
   - Built an interactive dashboard (`Vendor Performance PowerBI Dashboard.pbix`) with:
     - Sales and Purchase Summary
     - Vendor-wise Gross Profit & Profit Margin
     - Top Performing Vendors & Brands
     - Filters for Vendor, Brand, and Date

5. **Final Report**
   - Exported dashboard to PDF (`Vendor Performance Report.pdf`).

---

## 📂 Project Structure

vendor-analysis-project/
│
├── data/ # Raw CSV files
│ ├── begin_inventory.csv
│ ├── end_inventory.csv
│ ├── purchases.csv
│ ├── purchase_prices.csv
│ ├── sales.csv
│ └── vendor_invoice.csv
│
├── logs/ # Log files
│ ├── ingestion_db.log
│ └── get_vendor_summary.log
│
├── EDA.ipynb # Initial exploratory analysis
├── Vendor Performance Analysis.ipynb # SQL + Data summary notebook
├── get_vendor_summary.py # Script to generate vendor summary
├── ingestion_db.py # Script to ingest CSV data into DB
├── vendor_sales_summary.csv # Final cleaned dataset
├── Vendor Performance PowerBI Dashboard.pbix # Power BI file
├── Vendor Performance Report.pdf # Exported dashboard as PDF
└── README.md # Project documentation


---

## 🛠️ Tools & Technologies
- **Python**: Pandas, Matplotlib, Seaborn, SQLAlchemy
- **Database**: PostgreSQL
- **BI Tool**: Power BI
- **Logging**: Python `logging` module
- **Version Control**: Git & GitHub

---

## 📊 Dashboard Preview
*(Insert a screenshot of your Power BI dashboard here once uploaded)*  

---

## 📌 How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/Ananya-Vaishnav/Vendor-Data-Analysis.git
   cd Vendor-Data-Analysis
2. Install required Python libraries:
   pip install pandas sqlalchemy psycopg2 matplotlib seaborn
   
3. Setup PostgreSQL database inventory_db and ingest data:
   python ingestion_db.py
   
4. Generate vendor summary:
   python get_vendor_summary.py
   
5. Open Power BI and load vendor_sales_summary.csv to view the dashboard.

✨**Results & Insights**
  -Identified top performing vendors & brands by sales and profit.
  -Calculated profit margins and stock turnover for each vendor.
  -Interactive dashboard helps decision-makers analyze purchases, sales, freight costs, and vendor efficiency.

📧 **Contact**

👩‍💻 Author: Ananya Vaishnav
🔗 GitHub: Ananya-Vaishnav
📩 Email: ananyavaishnav05@gmail.com
