# power_bi-Projects
![image](https://github.com/kashifkhan9555/power_bi-Projects/assets/67798954/a4fc7830-7801-4cc5-8d0e-1188228b7fb3)
ntroduction
In today's business landscape, data-driven decision-making is crucial for success. The Superstore Sales Analysis and Forecasting project leverages the power of data to uncover patterns, trends, and key insights within a sales dataset. By employing advanced analytics and visualization techniques, this project assists stakeholders in understanding historical sales performance and predicting future trends.

Process
Data Preparation

The initial phase involved performing data cleaning tasks, including the removal of null values, the elimination of unnecessary columns, handling duplicates, and adjusting data types to ensure data quality.
Data Modeling

The subsequent step was to create calculated measures and tables using DAX (Data Analysis Expressions) in Power BI, enhancing the dataset's analytical capabilities.

  # Created time-series table of sales for forecasting.
  TimeSeriesTable = 
  SUMMARIZE(
    SuperStore_Sales_Dataset,
    SuperStore_Sales_Dataset[Order Date],
    "Total Sales", SUM(SuperStore_Sales_Dataset[Sales])
  )  
  
  # Calculate a measure to determine the number of days it took for delivery.
  DaysToDeliver = 
  DATEDIFF(
    SuperStore_Sales_Dataset[Order Date],
    SuperStore_Sales_Dataset[Ship Date],
    DAY
  )
Data Analysis

Following data modeling, an in-depth data analysis was conducted within Power BI, utilizing various visualization techniques like matrices to identify trends in sales, region-wise sales, category-wise sales, and other pertinent insights.
Dashboard Creation

The project proceeded with the development of an interactive and dynamic dashboard in Power BI. This dashboard was designed to include bookmark features, allowing for seamless navigation between different charts and visualizations to provide a more comprehensive view of the data.
Sales Forecasting

To deliver forward-looking insights, Power BI's advanced forecasting feature was utilized to perform a 10-day sales forecast. This forecasting capability assists stakeholders in anticipating future trends and making informed decisions.

Dashboard
The dashboard section offers an array of visualizations that empower users to explore and understand historical sales data. Key features of the dashboard include:

Visualization of monthly and yearly sales trends.
Comparison of sales across different categories and sub-categories.
Geographical distribution of sales.
Identification of top payment modes, segments, ship modes, and much more.
![image](https://github.com/kashifkhan9555/power_bi-Projects/assets/67798954/efe5a6dc-3a71-4ad3-90bf-459aeafde4b7)
Sales Forecasting
![image](https://github.com/kashifkhan9555/power_bi-Projects/assets/67798954/4c3da416-e72f-4282-830f-20222dad4d6a)
The sales forecasting page focuses on predicting sales for the subsequent 10 days. Leveraging historical sales data and advanced forecasting techniques of Power BI.
Key Insights
The dashboard and forecasting page unveil the following key insights:

Monthly Peaks: Noteworthy sales spikes in February, August, and October hint at recurring patterns.
Parallel Growth: While 2020 exhibits higher sales than 2019, the trend patterns remain consistent.
Geographic Leaders: California takes the lead in sales, closely followed by New York.
Region Impact: The West region contributes the most to overall sales.
Payment Preference: Cash On Delivery (COD) emerges as the preferred payment method.
Consumer Champion: The consumer segment generates the highest sales figures.
Top Category: Office Supplies stand out as the dominant sales category.
Preferred Shipping: Standard Class is the preferred shipping choice.
Sub-Category Stars: Phones and chairs emerge as the top-selling sub-categories.
Tech Stack
Project relies on the following key technologies:

Power BI Desktop Design, visualization, and interactive reporting.
DAX (Data Analysis Expressions) Creation of calculations and measures supporting data visualizations.
Advanced Analytics Predict future sales trends based on historical data.
Power Query Clean and transform raw data into a structured format.
Files Information
Data

SuperStore Processed Data: This file holds the data that has undergone cleaning and processing.
Sales TimeSeries: This file includes an additional table created using DAX, which played a role in the forecasting process.
Results

Dashboard: Within this section, you will find two sheets - one dedicated to the interactive dashboard and the other to the forecasting report.
Data Source
The Superstore Sales Data used in this project can be accessed here.

License
This project is licensed under the MIT License. You are free to use, modify, and distribute the code and visuals as long as the original license terms are maintained.
Enjoy exploring the Power BI Sales Insights and Forecasting Dashboard! If you have questions or feedback, feel free to contact me.

Contact: Kashifkhan4013@gmail.com
