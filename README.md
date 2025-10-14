# PowerBI-Sales-Dashboard-Superstore
A sales overview dashboard built with Power BI and Superstore data.

Power BI Sales Overview Dashboard 📊
🎯 Project Goal
The primary goal of this project was to gain hands-on experience with the Power BI Desktop environment, practice foundational data cleaning techniques using Power Query, and develop an interactive Sales Overview Dashboard. This project serves as the culmination of Week 1 of a Power BI Foundations and Data Cleaning curriculum, showcasing skills in end-to-end report creation.

⚙️ Project Details & Tech Stack
Technology Used: Microsoft Power BI Desktop and Power Query Editor.

Dataset Source: The dashboard was built using the publicly available Superstore Sales Dataset from Kaggle, which contains detailed retail sales data.

Link: Kaggle - https://www.kaggle.com/datasets/vivek468/superstore-dataset-final

🛠️ Data Cleaning & Transformation
Before visualization, the data was prepared in the Power Query Editor to ensure accuracy and usability. Key steps included:

Connecting & Importing: Established connection to the CSV/Excel source data.

Data Type Management: Corrected and standardized data types across all columns (e.g., currency, date, and text fields).

Null Value Handling: Identified and removed or addressed missing values (nulls).

Column Splitting: Performed necessary column operations (e.g., splitting a column) to create more granular data fields for analysis.

📈 Dashboard Key Features (KPIs and Visuals)
The dashboard provides a comprehensive view of the sales performance, covering all required metrics:

1. Key Performance Indicators (KPIs)
Metric	Value (Example)	Insight
Total Sales	$0.32M	Overall revenue generated.
Total Profit	-$9.27K	Crucial metric highlighting a net loss (negative profit) that requires immediate attention.
Total Orders	CA-2014-100090	Total count or example ID representing transaction volume.

Export to Sheets
2. Sales Distribution and Trend Analysis
Analysis	Visual Used	Key Insight
Sales by Region	Bar Chart	Identifies the West region as having the highest sales ($118K).
Sales by Category	Pie Chart	Shows Technology (38.09%) and Furniture (38.35%) are the largest categories by sales share.
Sales by Sub-category	Bar Chart	Reveals Phones ($52K) and Tables ($34K) are the top-selling sub-products.
Monthly Sales Trend	Line Chart	Illustrates a clear upward trend in sales from 2014 ($54K) to 2017 ($110K).

Export to Sheets
3. Interactivity
A Year/Category Slicer is included, allowing users to dynamically filter all visuals on the dashboard by specific years (2014-2017) and product categories.

