# E-Commerce Sales Report

## E-Commerce Sales Dashboard preview :
![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/0a39f6d9-c6fc-4983-baa3-4672c59d25a9)


#### Overview 
The E-Commerce Sales Dashboard is a comprehensive data visualization project designed to provide insights into various aspects of an e-commerce business. This project uses two CSV files and one Power BI file to create visualizations for the following metrics: 

- Profit by Month
- Profit by Sub-Category
- Quantity by Category
- Quantity by Payment Mode
- Amount by State
- Amount by Customer Name


#### Files Included
- Details.csv: This file contains detailed information about individual sales transactions, including product details, customer information, and payment modes.
- Orders.csv: This file contains order-level information, including order dates, shipment details, and order quantities.
- Seasonal Sales Report.pbix: This Power BI file contains the dashboard with all the visualizations created based on the data from the CSV files.

#### Getting Started
#### Prerequisites
Microsoft Power BI Desktop: To view and interact with the Power BI dashboard.
Any spreadsheet software (Excel, Google Sheets) to view and understand the CSV files.

#### Step 1 : Installation
#### Clone the repository:
```
git clone https://github.com/dishadey-github/e-commerce-sales-dashboard.git
```

#### Step 2 : Open the CSV files:
- Load Details.csv & Orders.csv:
- Click on Home in the top menu.
- Select Get Data > Text/CSV.
- Browse to the location of Details.csv, Orders.csv (do this separately) and click Open.
- In the preview window, click Load to import the data.

#### Step 3 : Open the Power BI dashboard:
#### Open Seasonal Sales Report.pbix using Microsoft Power BI Desktop.
#### Data Explanation
#### Details.csv
#### Columns:
- TransactionID: Unique identifier for each transaction.
- ProductID: Unique identifier for each product.
- CustomerID: Unique identifier for each customer.
- Quantity: Number of items purchased.
- Price: Price per item.
- Profit: Profit made on the transaction.
- Category: Product category.
- SubCategory: Product sub-category.
- PaymentMode: Mode of payment used by the customer.
- State: State where the transaction took place.
- CustomerName: Name of the customer.

#### Orders.csv
#### Columns:
- OrderID: Unique identifier for each order.
- OrderDate: Date when the order was placed.
- ShipDate: Date when the order was shipped.
- ShipMode: Mode of shipment.
- CustomerID: Unique identifier for each customer.
- ProductID: Unique identifier for each product.
- Sales: Total sales amount.
- Quantity: Number of items ordered.
- Discount: Discount applied to the order
- Profit: Profit made on the order.
- Category: Product category.
- SubCategory: Product sub-category.
- CustomerName: Name of the customer.

#### Step 4 : Data Transformation and Preparation
#### 1. Open Power Query Editor:
  Click on Transform Data to open the Power Query Editor. In view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.

#### 2. Inspect and Clean Data:
  Verify that both datasets (Details and Orders) are loaded correctly.\
Check for any inconsistencies or missing values and handle them accordingly (e.g., removing null values, correcting data types).

#### 3. Merge Queries (Optional):
  If necessary, merge the Details and Orders tables based on common columns like CustomerID or ProductID.\
Click on Home > Merge Queries and select the appropriate columns to merge on.

#### 4. Create calculated columns or measures as needed, such as Total Profit, Total Sales, etc.
  Use the Add Column tab to create new custom columns.

#### 5. Add column for Average Order Value
```
  AOV = [Amount]/[Quantity]
```

#### 6. Close and Apply:
  After making the necessary transformations, click Close & Apply to load the transformed data into Power BI.

#### Step 5: Visualizations
  Refer the detailed breakdown given below.

#### Step 6: Customize and Format Visualizations
#### 1. Adjust Visuals:
  Resize and arrange the visualizations on the report canvas for a clear and intuitive layout.

#### 2. Add Titles and Labels:
  Add titles and labels to each chart to make them self-explanatory.\
  Use the formatting options to change colors, fonts, and styles as needed.

#### 3. Add Filters and Slicers:
  Add slicers for important dimensions like Date, Category, or State to allow interactive filtering of the data.


#### Detailed breakdown from a Data Visualization and Business Analysis perspective:

![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/bc4703f6-f2a2-4501-b004-9389be3de757)

#### Overall Metrics
- Sum of Amount (438K): Displays the total revenue generated.
- Sum of Quantity (5615): Shows the total number of units sold.
- Sum of Profit (37K): Indicates the total profit earned.
- Sum of AOV (121K): Represents the Average Order Value.
These key performance indicators (KPIs) give a quick snapshot of the business’s overall health and performance.


![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/a57abb1b-a921-4af5-a8bb-a0a0a0baaacb)

#### Profit by Month: This visualization shows the monthly profit trends. It helps in identifying seasonal trends and monthly performance.
- Stacked Cloumn chart Chart: Depicts monthly profit, showcasing seasonality or monthly trends.
- January, February, December: High-profit months shown in Blue columns.
- June, July, August, October: Low or negative profit months shown in Orange columns.
- Understanding these trends can help in planning marketing campaigns and inventory management to maximize profitability.
  

![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/cc267009-ce4c-4344-a0ca-a86218ba448c)

#### Profit by Sub-Category: This chart displays the profit generated by each product sub-category, helping to identify the most and least profitable product lines.
- Stacked Bar Chart: Shows the profit by specific product sub-categories.
- Printers: Highest profit.
- Bookcases, Saree, Accessories, Tables: Lower profits in descending order.
- This provides insights into which sub-categories are most profitable, aiding in product line decisions and marketing efforts.
  

![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/836b675b-dca7-41f8-a4ed-e049154931a4)

#### Quantity by Category: This visualization shows the total quantity of items sold in each category. It provides insights into which categories have the highest sales volume.
- Donut Chart: Illustrates the percentage of units sold by product category.
- Clothing: 63%
- Electronics: 21%
- Furniture: 17%
- This helps understand which product categories are most popular, guiding inventory decisions and product focus.
  

![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/510f7bdb-5983-4d0d-81b4-49ad6e8e7a3d)

#### Quantity by Payment Mode: This chart illustrates the distribution of sales quantities across different payment modes, revealing customer payment preferences.
- Donut Chart: Shows the percentage distribution of sales quantities by different payment methods.
- Cash on Delivery (COD): 44%
- UPI: 21%
- Debit Card: 13%
- Credit Card: 12%
- EMI: 10%
- This visualization highlights the most popular payment methods among customers, which can inform payment processing decisions and promotions.
  

![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/b547640f-b6b5-41c2-8919-49f2251794d0)

#### Amount by State: This map visualization displays the total sales amount by state, helping to identify geographical sales performance.
- Stacked Bar Chart: Illustrates the revenue distribution across different states.
- Maharashtra: Highest revenue.
- Madhya Pradesh, Uttar Pradesh, Delhi: Lower revenues in descending order.
- This helps identify geographical areas with the highest and lowest sales, aiding in targeted marketing and sales strategies.
  

![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/bb92742a-1889-4918-831b-e47af1ef3624)

#### Amount by Customer Name: This chart lists the sales amount for each customer, identifying the top customers contributing to the revenue.
- Stacked Cloumn Chart: Details the revenue generated by top customers.
- Hariyana: Highest spending customer.
- Other significant customers: Madhav, Madan, Shiva.
- This helps identify key customers who contribute the most to the business, enabling personalized marketing and loyalty programs.
  

![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/a11dbe22-37b7-460d-b29b-659cc7c9009a)

#### Time Period Selection
  Quarter and Year Filters: Allow users to filter the data by specific quarters or view all data, providing flexibility in analyzing trends over different time periods.
  
![image](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/83772afa-e405-48ba-8ad0-2213782bcd15)

#### Location Selection
  State Filters: Allow users to filter the data by specific states or view all data, providing flexibility in analyzing trends over different locations(statets).

  
# E-Commerce Sales Report (with filters)

### Quarter 1, State - Delhi :
![Quarter 1, Delhi](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/3460fb20-aadf-43be-aab0-75282a0db7dd)

### Quarter 1, State - Andrapradesh :
![Quarter 1, Andrapradesh](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/67c3fb7d-9b0d-46f5-87aa-7c074ba7f850)

### Quarter 4, State - Karnataka :
![Quarter 4, Karnataka](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/c5f88117-a56c-45a3-8689-ccaa57f4cb86)

### Quarter 2, State - Karnataka :
![Quarter 2, Karnataka](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/8c6ef209-2193-459f-b57e-dd12c8ad3b2f)

### Quarter 2, State - Kerala :
![Quarter 2, Kerala](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/61186196-259e-4bff-85e4-1c21e5e59538)

### Quarter 3, State - West Bengal :
![Quarter 3, West Bengal](https://github.com/dishadey-github/e-commerce-sales-dashboard/assets/60807918/eaf1f86e-7a28-4c83-9be0-cbf2208d86cc)


#### Conclusion
This dashboard effectively combines various visual elements to provide a holistic view of the e-commerce business’s performance. It leverages bar charts, pie charts, and KPIs to present data in an easily understandable format. By breaking down the data by time, geography, customer, payment method, category, and sub-category, it allows stakeholders to quickly identify trends, strengths, and areas for improvement. This comprehensive approach helps in making informed business decisions to drive growth and efficiency.
