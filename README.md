# Global Superstore Analytics

## Table of Contents

- [Problem Statement and Overall Objectives](#problem-statement-and-overall-objectives)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning - Power Query Editor (DAX)](#data-cleaning---power-query-editor-(dax))
- [Exploratory Data Analysis](#exploratoty-data-analysis)
- [Data Analysis](#data-analysis)
- [Results/Findings](#resultsfindings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)

### Problem Statement and Overall Objectives

The main purpose of this Global Superstore project was/is to investigate the company's sales and profit by analyzing the historical dataset and tracking 
the sales and profit for each year, segment, and market. Additionally, it highlights the impact of different customers and products within the company's business. 

Data Scope: The data scope for this analysis will include all the years during which the company has sold products and managed orders.
View Required: A summary page presenting the company's sales and profit, taking into consideration the different factors mentioned above.

### Data Sources 

The data used for this analysis includes the orders, people, and returns data, which are stored in an XLSX format across different sheets. 
The data has been uploaded to Power BI as an Excel workbook.

### Tools

- Microsoft Power BI: The tool is used to create comprehensive, interactive data visualizations and share important business insights. 
      [Learn more](https://www.microsoft.com/sv-se/power-platform/products/power-bi?ef_id=_k_cb76b16ddc2510de7ad4d7779827f495_k_&OCID=AIDcmmc1fckbp7_SEM__k_cb76b16ddc2510de7ad4d7779827f495_k_&msclkid=cb76b16ddc2510de7ad4d7779827f495&market=se)

### Data Cleaning - Power Query Editor (DAX)

Initially the following tasks were performed: 

1. Data collection and inspection
   Since there are multiple sheets in the data file, a critical quality check was performed before collecting the data,
   such as verifying column count and headers, to ensure that the data is correct and ready for uploading.
   
2. Transformation & Modeling
   In Power Query Editor, some critical tasks were performed to transform the dataset and make it more suitable for analysis based on the project's goals.
   For example, the data type was changed for some columns, and new columns were created—both custom and conditional—to extract needed information,
   such as order years and delivery days.

   NB! Since the tranformation & modeling phase is iterative, this step was performed several times when different changes were needed to correct the dataset.

   Once the tranformed data was uploaded, in the modeling view, the desired model/relationship was created between the different tables/data.

### Exploratory Data Analysis

EDA involved exploring the Global Superstore data to answer key questions, such as: 

- What are the total sales, and which years had the highest and lowest performance?
- How many products were sold overall, and how does this break down by year, segment, and market?
- What is the average delivery time for order shipments?
- How many orders have been returned over the years?
- Which are the top 6 most profitable and least profitable products in sales?
- Who are the company's top 10 customers, and which segment includes most of them?

### Data Analysis

#### Summary Page
The dashboard shows information about profit and sales based on different factors, such as segment, market, and year. 
It also displays the top customers, as well as profit and loss products. Finally, the global map shows sales by region, which facilitates comparison with sales by market.

<img width="1002" alt="Image_DashB_PO" src="https://github.com/user-attachments/assets/0bd89925-ebda-4cac-8738-b5b83de733a7">

#### Some interesting code and graphics from the Python analysis in Visual Studio Code.

Please check the IPYNB file in the files section to see all the Python Pandas analyses.

- The top 10 customers by profit:

![Top 10_customers_profit](https://github.com/user-attachments/assets/257076f7-e5eb-4634-a408-0f4460288675)

- The top 10 products by profit:

![Top_products](https://github.com/user-attachments/assets/88d3220e-480f-4f72-8965-bbf4d1eb8b99)

- The top 6 Loss products:
  
![Top 6 Loss_Product](https://github.com/user-attachments/assets/f30a0d34-5e47-4cb1-89c9-f9f7d842e363)

### Results/Findings

- Total sales amount to approximately $12.6 million. The highest sales were recorded in 2015 with $4.3 million, while the lowest was in 2012 with $2.3 million.
  Sales have increased each year, indicating a positive trend.

- The total quantity of products sold is about 178,300. The Asian market has the highest total sales, followed by Europe, America, and others. However, by region, Europe shows the highest sales, followed by the American region. This indicates that while Asia leads in total market sales, specific European regions excel geographically. The company's largest segment is 'Consumer,' followed by 'Corporate' and 'Home Office.' Additionally, the quantity sold has increased each year, reflecting growing sales annually.
  
- The average delivery time for orders is about 4 days, which is reasonable and less than a week. This faster delivery helps improve customer satisfaction.
  
- Approximately 1,079 orders have been returned. Compared to the total number of orders across all markets and regions, this represents a small number of returns.
  
- Canon Image Copier’ is the most profitable product, followed by ‘Cisco Smart Phone.’ The top loss product is the ‘Cubify Cubex Double Head Printer,’ followed by the ‘Lexmark M Laser Printer.

- Most of the top 10 customers are in the 'Consumer' segment, but the most profitable customer who buys the most is in the 'Corporate' segment.

### Recommendations

1. **Focus on Profitable Segments**: With the most profitable customer in the Corporate segment, the company should increase marketing efforts and tailor offerings for corporate clients. Focusing on these segments could include bulk purchase discounts, customized solutions, and enhanced after-sales support.

2. **Optimize Consumer Segment Engagement**: Since most top customers are in the Consumer segment, maintaining and improving customer satisfaction and loyalty in this group should remain a priority. This might include personalized marketing, loyalty programs, or improved customer service.

3. **Leverage High-Performing Products**: With "Canon Image Copier" and "Cisco Smart Phone" being top profit generators, the company should focus on promoting these products further. Expanding their product lines or bundling them with related items could boost sales even more.

4. **Address Loss-Making Products**: The significant losses from products like "Cubify Cubex Double Head Printer" and "Lexmark M Laser Printer", etc. suggest a need to reevaluate these items. The company could consider phasing them out, renegotiating supplier terms, or improving product features to enhance profitability.

5. **Improve Return Management**: Although returns are relatively low, the company should continue to monitor return reasons and reduce them where possible. This could involve improving product quality, refining the return policy, or enhancing customer support to prevent returns.

6. **Enhance Sales in Key Regions**: While the Asian market has high sales, the European region outperforms geographically. The company could explore why Europe is leading and replicate successful strategies in other regions.

7. **Maintain Fast Delivery Times**: The average delivery time of 4 days is reasonable. Continuing to optimize logistics to ensure fast delivery will likely increase customer satisfaction and repeat purchases.

By focusing on these areas or recommendations, the company can strengthen its market position, improve profitability, and continue to grow in the coming years.

### Limitations

1. **Data Accuracy and Reliability**: The accuracy of the insights is dependent on the quality and correctness of the historical dataset. Any inaccuracies or inconsistencies in the data can lead to misleading conclusions in the analysis.

2. **Lack of Statistical Validation**: The analysis presented in the Power BI dashboard might lack rigorous statistical validation. Without additional statistical analysis, such correlation or regression analysis, the findings may not be robust or generalizable.

3. **Limited Context and Insights**: The dashboard may provide a snapshot of data but might not account for underlying factors or external variables influencing the results. Additional context or qualitative analysis might be needed to fully understand the reasons behind the trends and patterns observed.

💻🖱️⌨️💻🖱️🖥️






















