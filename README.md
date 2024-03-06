# Clothing Store Sales Analysis

![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/pexels-edgars-kisuro-1488463.jpg)

## Introduction
In the contemporary digital marketplace, e-commerce stores are inundated with data reflecting customer behaviours, sales efficiency, and product performance. Extracting actionable insights from this data is critical for strategic decision-making and sustaining competitive advantage. 
This project documentation details an extensive SQL-based data analysis performed on a dataset from 'TheLook', a fictitious e-commerce clothing store developed by the Google Looker team, using Google BigQuery. 
The analysis covers a period from August 2019 to February 2024, focusing on sales transactions, customer demographics, and digital marketing efficacy.

## Problem Statement
'TheLook' requires a comprehensive understanding of its operational performance, customer engagement, and marketing effectiveness to enhance its decision-making process. 
The core objectives were to identify sales trends, evaluate brand and product performance, understand customer acquisition channels, and assess order fulfilment success. 
The analysis aimed to tackle these objectives by utilizing SQL queries to derive insights that would drive data-driven marketing strategies.

## Methodology and Analysis
## 1. Sales Performance by Month

- **Query Utilized:** A query was designed to calculate monthly revenue, total customers, and total orders, excluding cancelled and returned orders to ensure an accurate representation of effective sales.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap.png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Revenue%20Per%20Months.png)

- **Insights and Recommendation:** Seasonal trends were evident, with January and December showing peak revenues, likely due to holiday shopping. Marketing campaigns should be aligned with these peak periods to maximize sales. The analysis also suggested a need for strategies to improve customer retention and increase order volume during off-peak months.

## 2. Customer Demographics by Country

- **Query Utilized:** A query extracted customer counts per country, detailing the gender distribution within each.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(1).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Customer%20Per%20Country.png)

- **Insights and Recommendation:**  China and the United States top the list with the highest number of total customers. This could suggest a strong market presence or brand awareness in these regions.

There is a relatively balanced gender distribution in most countries, with a slight male dominance in some cases. This information could be used to tailor marketing campaigns to be more gender-neutral or to address any gender disparities in engagement.

## 3. Revenue by Gender

- **Query Utilized:** A query was created to segment the customers by gender, which is essential for understanding how different genders contribute to the overall sales.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(2).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Revenue%20By%20Gender.png)

- **Insights and Recommendation:** Males have generated slightly more revenue than females according to the data provided. This could suggest that either males are purchasing higher-value items or are more frequent buyers.

Despite the higher revenue from males, females have purchased a higher quantity of items. This could imply that females are more active shoppers but at a lower price point per item. These insights can inform targeted marketing strategies. For instance, marketing higher-value items to males and increasing the volume of lower-value, high-interest items for females could be effective.

## 4. Revenue by Age Group

- **Query Utilized:** A CASE statement was used to categorized customers into age groups, which is a common practice to identify demographic segments within the customer base.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(3).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Revenue%20By%20Age%20Group.png)

- **Insights and Recommendation:** The 'Adults' and 'Elderly' age groups have the highest number of customers, indicating that these demographics are the primary market segments for the e-commerce store.
Given the significant number of elderly customers, there might be an opportunity to market products more aggressively to this age group, which is often underrepresented in e-commerce.

## 5. Brand Performance

- **Query Utilized:** The query ranked the top and least-performing brands by revenue and quantity sold. Below is the query for the top-selling brands.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(4).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Top%2010%20Brands.png)

- **Insights and Recommendation:** Calvin Klein leads in both revenue and quantity, suggesting strong brand preference and market penetration.

While Diesel has a lower quantity sold compared to Calvin Klein, the revenue is quite close, indicating that Diesel's products may have a higher average price point.

Knowing the top-selling brands can guide inventory stocking decisions and sales strategies, including which brands to feature in marketing campaigns or promotions.

Here's the query for the least-performing brands.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(5).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Least%2010%20Brands.png)

- **Insights and Recommendation:** Brands like "marshal" and "Made in USA" are at the bottom of the list in terms of revenue, which might indicate a lack of customer interest or poor market fit.
The store might consider reviewing the product range, pricing strategies, and marketing efforts for these low-performing brands.
It may also be worth exploring whether these brands are facing supply issues or if the low sales figures are due to consumer preferences shifting away from these brands.

## 6. Product Category Performance

- **Query Utilized:** The query focused on the top-selling and least-selling product categories, providing insights into consumer preferences. Below is the query for the top-selling categories.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(6).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Top%2010%20Category.png)

- **Insights and Recommendation:** 'Outerwear & Coats' and 'Jeans' are the top-selling categories by revenue, indicating strong customer demand for these products.

While 'Outerwear & Coats' leads in revenue, 'Jeans' is the leader in quantity, suggesting a high turnover rate which could be due to a combination of popularity and perhaps lower price points.

The data suggests that customers are spending more on certain categories, potentially driven by seasonality (outerwear being popular in colder seasons) or fashion trends. This insight could inform inventory stocking levels and promotional activities, especially focusing on the top categories during peak seasons or marketing pushes.

Here's the query for the least-performing categories.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(7).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Least%2010%20Category.png)

- **Insights and Recommendation:** Categories like "Clothing Sets" and "Jumpsuits & Rompers" are among the least selling by revenue, which may indicate a lower demand or possibly higher return rates.

Low revenue figures in categories like "Leggings" and "Skirts" could be an opportunity for targeted marketing campaigns, bundled offers, or product improvements to boost sales.

The store might consider reducing stock levels for these underperforming categories to minimize holding costs and reallocate space and resources to more profitable categories.

## 7. Order Cancellations and Returns by Brand and Category

- **Query Utilized:** The queries identified brands and categories with the highest cancellations and returns. Below are the brands with the highest cancellations and returns

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(8).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Top%20Cancelled%20Brand%20Orders.png)

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(9).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Top%20Returned%20Brand%20Orders.png)

- **Insights and Recommendation:** Brands like Allegra K, Calvin Klein, and Carhartt have the highest number of cancelled and returned orders, which could point to various issues such as customer satisfaction, product quality, or possibly issues with product sizing or expectations set by product listings.

Strategies should be implemented to reduce these rates, which could include improving product descriptions, quality control measures, customer service training, or even revising the return policy.

Below are the product categories with the highest cancellations and returns.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(10).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Top%20Cancelled%20Category%20Orders.png)

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(11).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Top%20Returned%20Category%20Orders.png)

- **Insights and Recommendation:**  'Intimates' and 'Jeans' are at the top of the list for cancellations. This could indicate sizing issues, discrepancies in product descriptions, or customer expectations not being met.

High cancellation rates in specific categories like 'Fashion Hoodies & Sweatshirts' and 'Sleep & Lounge' may require a review of product descriptions, imagery, and sizing guides to ensure they are accurate and informative.

Similar to cancellations, 'Intimates' and 'Jeans' lead in returns. This further suggests possible issues with fit, quality, or customer satisfaction that need addressing.

Consider reducing stock for categories with high returns and cancellations to minimize financial loss. Also, enhance customer engagement efforts to better understand the reasons behind cancellations and returns, possibly through surveys or direct feedback mechanisms.

## 8. Traffic Channel Performance

- **Query Utilized:** The query aims to categorize users by their traffic source, which is crucial for understanding which marketing channels are most effective at acquiring customers.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(12).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Traffic%20Channel%20Performance.png)

- **Insights and Recommendation:** The 'Search' channel has brought in the most customers, indicating that search engine marketing and optimization strategies are likely paying off.

With 'Organic' being the second-highest, it shows a strong organic presence, which could be due to effective SEO or a strong brand presence. The significant number of customers from 'Facebook' suggests that social media is an effective channel for customer acquisition for this e-commerce store.

This data can help in making informed decisions about where to allocate marketing budgets to maximize ROI. Investment in search and organic channels may be increased, while the approach to email and display advertising might need to be reassessed. 

## 9. Average Order Value (AOV) Trends

- **Query Utilized:** Monthly and yearly AOV was calculated to understand spending behaviour.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(13).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20AOV%20By%20Month%20%26%20Year.png)

- **Insights and Recommendation:** The AOV seems to fluctuate throughout the year, with certain months like February '24 and September '23 showing higher values.

Peaks in AOV may indicate seasonal effects, such as holiday shopping or seasonal promotions that increase the average spend. This data can inform various business decisions, including pricing strategies, marketing campaigns, and inventory planning.

## 10. Top Customers by Revenue

- **Query Utilized:** The query uniquely identifies the top 10 customers by total revenue.

SQL Query             |  SQL Result
:-------------------------:|:-------------------------:
![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/Snap%20(14).png)  |  ![](https://github.com/Joel-web3/Clothing_Store_Sales_Analysis/blob/main/The%20Look%20-%20Top%2010%20Customers.png)

- **Insights and Recommendation:** The top customers by total revenue are valuable assets to the store and could be targeted for loyalty programs, special promotions, or exclusive previews of new products.

These customers might also provide valuable feedback on their shopping experience and preferences, which can guide product selection and customer service improvements. The store could use personalized marketing strategies to maintain and enhance the relationship with these top customers, ensuring they continue to engage with the store.

If a significant portion of revenue is coming from a small group of customers, the store might consider diversifying its customer base to mitigate the risk of revenue loss if one or more of these top customers were to decrease their spending.

## Conclusion

This portfolio project, employing advanced SQL queries in Google BigQuery, provides 'TheLook' with a granular analysis of its e-commerce performance. Each query was carefully crafted to unearth specific insights, forming a basis for strategic recommendations. 

The analysis highlighted the store's strengths and opportunities across various facets of the business, from customer acquisition to product strategy. This report not only demonstrates the analytical capability but also underscores the importance of data-driven decision-making in marketing analytics.

Throughout the analysis, Google BigQuery was instrumental as a powerful tool for processing large sets of e-commerce data. 

Its ability to quickly execute complex SQL queries across extensive datasets showcases its utility for data analysts and marketing professionals. This project is a testament to the proficiency in leveraging BigQuery to derive actionable business insights, a skill that is highly valuable in the modern data-centric business environment.
