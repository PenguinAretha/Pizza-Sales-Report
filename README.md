# Pizza-Sales-Report

In this project, my goal is to analyze sales report from a pizza shop. The processes include importing the dataset, cleaning, data processing and finally data visualization.

This data was sourced online.

Problem Statement

Analyze key indicators for pizza sales data to gain insights into business performance.

Metrics:

Total Revenue

Total Order Value

Total Pizzas Sold

Total Orders

Average Pizza Per Order

Chart Requirements

Daily Trend for Total Orders

Monthly Trend for Total Orders

Percentage of Sales by Pizza Category

Percentage of Sales by Size

Total Pizza Sold by Pizza Category

The first process, importing the dataset. Next is data cleaning. By using Power Query you can clean and process your data before loading into Power BI. Always remember, data cleaning is one of the most important steps in your analysis and must be carried out before proceeding with processing or visualization. In cleaning this dataset, I checked for empty rows and columns, ensured there were no duplicate rows and also made sure all columns or features were in the appropriate format. Initially, in the Pizza Size column, values were abbreviated to L, M, R, XL, XXL which I decided to replace with the corresponding size in full words using the Find and Replace. For example finding L and replacing with Large etc. When I was confident my data was clean I proceeded to processing it.

Now to data processing. To properly represent the KPIs required I had to create some new measures. For example, to get my Total Orders I had to create a new measure to find the distinct count of “order id” that is Total Orders = DISTINCTCOUNT(pizza_sales[order_id]). After creating all the new measures needed I then proceeded with analyses.
![Capture d'écran 2024-02-26 223334](https://github.com/PenguinAretha/Pizza-Sales-Report/assets/97256031/1950ae6b-040c-4da5-838c-e82581993742)

From the chart, it can be noticed that sales are highest on Thursday, Friday and Saturday. You realize that these days are towards the weekend which makes sense. For some reasons, the highest orders by month can be found in January and July.

Additionally, the Classic pizza category seems to be the people’s favorite as it has the highest percentage of sales whiles by pizza size, the large size seems to be the preferred.

Detailed information about the performance of each pizza brand can be found in the chart below.

![Capture d'écran 2024-02-26 223352](https://github.com/PenguinAretha/Pizza-Sales-Report/assets/97256031/780b4687-0e2f-402e-b302-e0cf268d9cdc)
