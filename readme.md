# Project Background
La Baguette Enchantée is a small bakery located in Paris. As a family business, its owners put a lot of dedication into delivering the best products and attention to its clients. They have been collecting transaction data since 2021, and they think it's time to put this data into use. This project analyzes La Baguette Enchantée's sales data to identify customer purchasing patterns and uncover insights that will help improve the business operations of the bakery.

### This project provides insights and recommendations on the following areas:
- **Sales Over Time**: Analysis of sales by month, day of the week, and hour of the day to uncover seasonality patterns and peak sales periods and provide insights for staffing, inventory, and the creation of new promotions.
- **Product Performance Analysis**: Analysis of the top- and low-performing products, identifying which contributes the most to the bakery's revenue and assessing their seasonal performance.
- **Market Basket Analysis**: An analysis of frequent product combinations to understand how product bundling and promotions could help improve sales.

**The Jupyter Notebook of the project can be found [here](https://github.com/fedemaximovicz/BakerySales/blob/master/bakery_sales.ipynb)**.

# The Data
La Baguette Enchantée is a fictitious bakery created to emulate a real-world scenario for this project. The data used is from Kaggle and uploaded by Matthieu Gimbert, [click here to go to the Kaggle page of the dataset](https://www.kaggle.com/datasets/matthieugimbert/french-bakery-daily-sales).
 
The data consists of 234,005 transactions of a French bakery from 2021 to 2022.

### Structure of the dataset (after cleaning and formatting)
![structure of the data](/images/data.png)


| **Column Name** | **Description**                       |
|-----------------|---------------------------------------|
| date            | Transaction date                      |
| time            | Transaction time                      |
| ticket_number   | Unique purchase identifier            |
| article         | Product name (e.g., Croissant, Baguette)|
| quantity        | Number of items purchased             |
| unit_price      | Price per unit in EUR                 |


# Business Insights and Findings
**Sales in 2021 and 2022 followed a similar trend, peaking during the summer months**. August recorded the highest sales in both years, with a total monthly revenue of **€48,697.05 in 2021 and €53,888.80 in 2022**. The **sales declined significantly in the winter** months, reaching the **lowest point in January**. The total monthly revenue in January 2021 was **€15,271.67 and €15,690.70 in 2022**.

![monthly sales](/images/monthly_revenue.png)

**Saturday and Sunday recorded the highest sales volume and revenue**, surpassing weekday performance. This trend highlights a key opportunity for targeted promotions and optimized staffing.

![daily sales](/images/daily_revenue.png)

**Revenue is highest during the daytime, peaking at 11 AM with an average of €159.45**. Sales decline in the evening, indicating lower demand during later hours.


![hourly sales](/images/hourly_revenue.png)

## Product Performance
**The best-selling product of the bakery by a significant margin is the Traditional Baguette** generating a revenue of **€144,795.20** in this period (2021 - 2022) and **representing 25.9% of the total revenue**. This product also sold a total quantity of **117,495 units**. The second best-selling product is the Formule Sandwich, which generated 34,936.50 in revenue, sold 5214 units and represents 6.25% of the total revenue.

![best selling products](/images/best-selling.png)

### Daily Performance
The revenue and quantity sold of the top five best performing products increase during the weekend, except for the Formule Sandwich. This suggests that the Formule Sandwich is primarily a weekday item, likely consumed by workers during breaks or students.

![average daily sales of top 5 products](/images/daily_revenue_product.png)

### Hourly Performance
Early in the morning, apart from the Traditional Baguette, the most popular products are the Croissant and Pain au Chocolat, which indicates they are primarily purchased for breakfast. Sales for these items peak in the morning before declining throughout the day.

![average hourly sales of top 5 products](/images/hourly_revenue_product.png)

The Traditional Baguette remains the best-selling product throughout the day, reaching its highest sales at 11 AM, with an average revenue of €54.80 and an average of 44.5 units sold.

The Formule Sandwich experiences two sales peaks, aligning with typical lunch breaks and post-work hours. Sales start rising in the morning, peaking at noon with an average revenue of €35.80 and 5.3 average units sold. A second peak occurs at 7 PM, generating an average revenue of €32.50. This confirms that the Formule Sandwich is primarily purchased by workers and students.

# Methodology and Tools
