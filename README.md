# e-commerce-sales-dashboard

## E-Commerce Sales Dashboard preview :
![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/0a39f6d9-c6fc-4983-baa3-4672c59d25a9)


## Overview
The E-Commerce Sales Dashboard is a comprehensive data visualization project designed to provide insights into various aspects of an e-commerce business. This project uses two CSV files and one Power BI file to create visualizations for the following metrics:

Profit by Month
Profit by Sub-Category
Quantity by Category
Quantity by Payment Mode
Amount by State
Amount by Customer Name


### Files Included
1. Details.csv: This file contains detailed information about individual sales transactions, including product details, customer information, and payment modes.

2. Orders.csv: This file contains order-level information, including order dates, shipment details, and order quantities.

3. Seasonal Sales Report.pbix: This Power BI file contains the dashboard with all the visualizations created based on the data from the CSV files.

## Getting Started
### Prerequisites
Microsoft Power BI Desktop: To view and interact with the Power BI dashboard.
Any spreadsheet software (Excel, Google Sheets) to view and understand the CSV files.

## Step 1 : Installation
### Clone the repository:

git clone https://github.com/dishadey-github/e-commerce-sales-dashboard.git

## Step 2 : Open the CSV files:
### Load Details.csv:
Click on Home in the top menu.
Select Get Data > Text/CSV.
Browse to the location of Details.csv and click Open.
In the preview window, click Load to import the data.

### Load Orders.csv:
Repeat the process by clicking Get Data > Text/CSV.
Browse to the location of Orders.csv and click Open.
In the preview window, click Load to import the data.

## Step 3 : Open the Power BI dashboard:
### Open Seasonal Sales Report.pbix using Microsoft Power BI Desktop.
### Data Explanation
### Details.csv
### Columns:
TransactionID: Unique identifier for each transaction.
ProductID: Unique identifier for each product.
CustomerID: Unique identifier for each customer.
Quantity: Number of items purchased.
Price: Price per item.
Profit: Profit made on the transaction.
Category: Product category.
SubCategory: Product sub-category.
PaymentMode: Mode of payment used by the customer.
State: State where the transaction took place.
CustomerName: Name of the customer.

### Orders.csv
### Columns:
OrderID: Unique identifier for each order.
OrderDate: Date when the order was placed.
ShipDate: Date when the order was shipped.
ShipMode: Mode of shipment.
CustomerID: Unique identifier for each customer.
ProductID: Unique identifier for each product.
Sales: Total sales amount.
Quantity: Number of items ordered.
Discount: Discount applied to the order
Profit: Profit made on the order.
Category: Product category.
SubCategory: Product sub-category.
CustomerName: Name of the customer.

## Step 4 : Data Transformation and Preparation
### 1. Open Power Query Editor:
Click on Transform Data to open the Power Query Editor. In view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.

### 2. Inspect and Clean Data:
Verify that both datasets (Details and Orders) are loaded correctly.
Check for any inconsistencies or missing values and handle them accordingly (e.g., removing null values, correcting data types).

### 3. Merge Queries (Optional):
If necessary, merge the Details and Orders tables based on common columns like CustomerID or ProductID.
Click on Home > Merge Queries and select the appropriate columns to merge on.
Create New Columns (Optional):

### 4. Create calculated columns or measures as needed, such as Total Profit, Total Sales, etc.
Use the Add Column tab to create new custom columns.

### 5. Add column for Average Order Value
AOV = [Amount]/[Quantity]

### 5. Close and Apply:
After making the necessary transformations, click Close & Apply to load the transformed data into Power BI.

## Step 5: Create Visualizations
### Profit by Month: This visualization shows the monthly profit trends. It helps in identifying seasonal trends and monthly performance.
Drag the OrderDate field to the axis of a Stacked Cloumn chart.
Drag the Profit field to the values area.
Set the aggregation to Sum if not already done.

### Profit by Sub-Category: This chart displays the profit generated by each product sub-category, helping to identify the most and least profitable product lines.
Use a Stacked Bar chart.
Drag SubCategory to the axis.
Drag Profit to the values area.

### Quantity by Category: This visualization shows the total quantity of items sold in each category. It provides insights into which categories have the highest sales volume.
Use a Donut chart.
Drag Category to the axis.
Drag Quantity to the values area.

### Quantity by Payment Mode: This chart illustrates the distribution of sales quantities across different payment modes, revealing customer payment preferences.
Use a  Pie chart or Donut chart.
Drag PaymentMode to the legend or axis.
Drag Quantity to the values area.

### Amount by State: This map visualization displays the total sales amount by state, helping to identify geographical sales performance.
Use a Stacked Bar chart or map visualization.
Drag State to the location field.
Drag Sales or Amount to the values area.

### Amount by Customer Name: This chart lists the sales amount for each customer, identifying the top customers contributing to the revenue.
Use a Stacked Cloumn chart chart.
Drag CustomerName to the rows or axis.
Drag Sales or Amount to the values area.

## Step 5: Customize and Format Visualizations
### Adjust Visuals:
Resize and arrange the visualizations on the report canvas for a clear and intuitive layout.

### Add Titles and Labels:
Add titles and labels to each chart to make them self-explanatory.
Use the formatting options to change colors, fonts, and styles as needed.

### Add Filters and Slicers:
Add slicers for important dimensions like Date, Category, or State to allow interactive filtering of the data.
Step 5: Save and Share the Report

### Save the Report:
Click on File > Save As and save your Power BI file with an appropriate name, such as E-Commerce Sales Dashboard.pbix.
Publish to Power BI Service (Optional):

### Customization
### Open Seasonal Sales Report.pbix in Power BI Desktop.
Use the Fields pane to drag and drop new fields into existing visualizations or create new visualizations.
Use the Visualizations pane to change the type of charts or add new elements like slicers, filters, and more.

## Quarter 1, State - Delhi :
![Quarter 1, Delhi](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/3460fb20-aadf-43be-aab0-75282a0db7dd)

## Quarter 1, State - Andrapradesh :
![Quarter 1, Andrapradesh](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/67c3fb7d-9b0d-46f5-87aa-7c074ba7f850)

## Quarter 4, State - Karnataka :
![Quarter 4, Karnataka](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/c5f88117-a56c-45a3-8689-ccaa57f4cb86)

## Quarter 2, State - Karnataka :
![Quarter 2, Karnataka](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/8c6ef209-2193-459f-b57e-dd12c8ad3b2f)

## Quarter 2, State - Kerala :
![Quarter 2, Kerala](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/61186196-259e-4bff-85e4-1c21e5e59538)

## Quarter 3, State - West Bengal :
![Quarter 3, West Bengal](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/eaf1f86e-7a28-4c83-9be0-cbf2208d86cc)

## Final Interactive Report for E-Commerce Sales Dashboard :
![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/0a39f6d9-c6fc-4983-baa3-4672c59d25a9)

### Dashboard Link : https://app.powerbi.com/groups/me/reports/ab034c62-d28c-454a-af27-227aa14f3cda/b8405238833b12d06212?bookmarkGuid=31425bc8-7d30-48df-aa73-69b791987dab&bookmarkUsage=1&ctid=76a2ae5a-9f00-4f6b-95ed-5d33d77c4d61&portalSessionId=21d31427-cc6e-4381-813c-bf517e1b87f3&fromEntryPoint=export
