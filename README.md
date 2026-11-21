# Sales Data Exploratory Analysis with pandas, Matplotlib and Seaborn

Exploratory data analysis (EDA) of an online retailer's sales data, completed as part of the Mission Ready Data Analysis Accelerator using a Microsoft Fabric notebook.

## Dataset
An Excel workbook with three sheets (Sales, Invoice and Product), merged into a single table of 83,277 line items using the invoice number and stock code as keys.

## What I did
1. Loaded each sheet into its own DataFrame and created a Sales column (Quantity x Unit Price).
2. Checked for missing values and calculated summary statistics.
3. Merged the Sales, Invoice and Product tables.
4. Removed the top 1% of Sales and Quantity values for charting, because a single transaction of 74,215 units made the charts unreadable.
5. Visualised the data with scatter plots, histograms, bar charts and a line chart, plus a correlation heatmap.
6. Summarised sales by product category and built a Country x Product Category pivot table.

## Key findings
- The UK accounts for roughly 90% of total revenue.
- The business is a home decor and gift retailer. Top categories include Christmas, candles, glassware, mugs and lights.
- Sales peak around October and November, ahead of Christmas, and dip around April.
- Quantity and Sales are very strongly correlated (0.98), while Unit Price shows almost no relationship with either.
- Sales per line item are strongly right-skewed: many small purchases and a few large ones.
- Data quality issue: the largest single category is Uncategorized, so category insights should be read with care.

## Tools
Python, pandas, matplotlib, seaborn, Microsoft Fabric notebooks.
# sales-eda-pandas-seaborn
