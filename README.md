# E-commerce Sales Data Analysis Using Python

**Internship:** Data Science Virtual Internship  
**Module:** Module 02 – Week 2 (Intermediate)  
**Dataset:** UCI Online Retail  
**Tools:** Python, NumPy, Pandas, Matplotlib, Google Colab

## Project overview
This project performs exploratory data analysis (EDA) on a real-world online retail transaction dataset from the UCI Machine Learning Repository. Each row represents an item on an invoice for a UK-based online retailer.

## Project questions
- How do sales change over time?
- Which products and countries generate the most revenue?
- How many orders and customers are represented?
- What patterns appear after cleaning cancellations, duplicate records and invalid sales lines?

## Dataset source and attribution
- Official page: https://archive.ics.uci.edu/dataset/352/online-retail
- Official download archive: https://archive.ics.uci.edu/static/public/352/online+retail.zip
- Citation: Chen, D. (2015). *Online Retail* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5BW33
- License: CC BY 4.0. Please retain attribution to the dataset creator and UCI.

The dataset contains 541,909 transaction rows from 1 December 2010 to 9 December 2011. The original fields include invoice number, stock code, product description, quantity, invoice date, unit price, customer ID and country. The company mainly sells gifts and has wholesale customers.

## Project files
- `Ecommerce_Sales_Data_Analysis.ipynb` — complete Google Colab/Jupyter notebook.
- `README.md` — project documentation.
- `requirements.txt` — Python dependencies.
- `DATASET_SOURCE.txt` — official dataset source and citation.

The notebook downloads the official UCI ZIP archive when run. The raw dataset is not included in this project ZIP or required to be uploaded to GitHub.

## Analysis performed
1. Import Python libraries and download/load the dataset.
2. Inspect rows, columns, data types and descriptive statistics.
3. Check missing values and duplicate rows.
4. Convert dates and numeric fields to appropriate types.
5. Remove duplicate records and rows missing essential sales fields.
6. Identify cancellations and non-positive quantity/price rows.
7. Calculate revenue as quantity × unit price (GBP).
8. Analyze monthly revenue.
9. Identify top products and countries by revenue.
10. Analyze order and customer activity.
11. Group and aggregate sales data.
12. Explore quantity and order-revenue relationships.
13. Filter, sort and export analysis results.
14. Generate a written summary.

## How to run in Google Colab
1. Download and extract this project ZIP.
2. Open https://colab.research.google.com/
3. Select File → Upload notebook.
4. Upload `Ecommerce_Sales_Data_Analysis.ipynb`.
5. Select Runtime → Run all.
6. The notebook downloads the UCI dataset archive automatically. If this fails, download `Online Retail.xlsx` from the official UCI dataset page and upload it when prompted.
7. Run all cells and review the tables and charts.

## Expected visualizations
- Monthly E-commerce Sales Revenue (line chart)
- Top 10 Products by Sales Revenue (horizontal bar chart)
- Top 10 Countries by Sales Revenue (horizontal bar chart)
- Distribution of Orders per Customer (histogram)
- Order Quantity vs Order Revenue (scatter plot)

## Important methodology notes
- Invoice numbers beginning with `C` indicate cancellations, according to UCI's dataset documentation.
- Completed-sales analysis excludes cancellation invoices and rows with non-positive quantity or unit price.
- Revenue is calculated in British pounds (GBP): `Quantity * UnitPrice`.
- Rows with missing customer IDs can remain in total sales analysis, but are excluded from customer-level calculations.
- This dataset is historical and represents one retailer, not the entire e-commerce market.
