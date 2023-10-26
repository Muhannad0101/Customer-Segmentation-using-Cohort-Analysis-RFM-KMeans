# E-Commerce : Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans

### Content
"This is a transnational data set which contains all the transactions occurring for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers."

Per the UCI Machine Learning Repository, this data was made available by Dr Daqing Chen, Director: Public Analytics group. chend '@' lsbu.ac.uk, School of Engineering, London South Bank University, London SE1 0AA, UK.

### Solution
Here, I performed an analysis and created a Dashboard using Tableau to display the results of the total sales data for each country with the months for each time of the day, for example morning and evening periods, and so on from the billing time, and compared the profits against the transactions. also I create a dashboard for the top 5 countries, the top 10 clients, and the top ten descriptions.

![Screenshot 2023-06-08 205842](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/19318e17-a3f8-42ee-9efb-d1accb83edd1)

![Screenshot 2023-06-08 205930](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/9ca02ad2-caa2-44d1-a15d-9b69d838b765)

- Cohort Analysis:

1- Cohort Month: On the vertical axis, we have different cohorts grouped by months, ranging from 2010-12 to 2011-12. Each cohort represents users who started their relationship with a company or service in that month.

2- Cohort Index: On the horizontal axis, we have the Cohort Index, representing the number of months since the starting month. A Cohort Index of 1 is the month the cohort started, 2 is the subsequent month, and so on.

3- Retention Rate: The values in the grid show the percentage of the cohort that remains engaged with the company or service over time. A retention rate of 100% for all cohorts in the first month (Cohort Index 1) is expected, as that's the month when the users started. As time progresses (moving rightward on the Cohort Index), the retention rate tends to drop, showing how many of the original users continue to engage or transact with the business.

- Analyzing the chart:

The 2010-12 cohort started with 100% retention (as all cohorts do) and by the 13th month, retained 27% of its original users.
The 2011-01 cohort had a retention of 15% by its 12th month.
Later cohorts, such as those from mid-2011 onwards, have fewer data points because they've existed for fewer months relative to the earlier cohorts.

- Key Insights:

The 2010-12 cohort seems to have the best long-term retention, retaining 50% of its users by the 12th month.
Some cohorts show a slight increase in certain months (e.g., the 2011-02 cohort in month 9 or the 2011-04 cohort in month 6), which could be due to specific marketing campaigns, seasonal effects, or other external factors.
The chart allows businesses to understand user behavior and longevity over time, enabling them to tailor their marketing and retention strategies effectively.

![1](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/6c6ffa4c-c67f-4830-bf16-6bad6e275fa4)


- RFM (Recency, Frequency, Monetary)

1- CustomerID: This is a unique identification number for each customer. It allows the business to differentiate between individual customers.

2- Recency: This typically refers to the number of days since the last transaction or interaction a customer had with the business. A lower number suggests that the customer has interacted with the business more recently. For example, a recency of 9 for CustomerID 12349.0 means that this customer had their last transaction or interaction with the business 9 days ago.

3- Frequency: This indicates how many times the customer has transacted or interacted with the business during a specific period. In this table, CustomerID 12347.0 has had 7 interactions or transactions.

4- Monetary: This represents the total amount of money a customer has spent with the business during a particular period. For instance, CustomerID 12348.0 has spent a total of 1797.24 (likely in a local currency).

- A quick analysis of the data suggests:

CustomerID 12346.0 has not made any transactions recently (316 days ago) and has spent no money despite having 2 interactions or transactions.
CustomerID 12347.0 transacted very recently (only 7 days ago), had 7 transactions, and spent a total of 431.00.
CustomerID 12348.0 had their last transaction 66 days ago, had 4 transactions in total, and spent 1797.24.
CustomerID 12349.0 is also a recent customer with their last transaction 9 days ago. They made 1 transaction and spent 1757.55.
CustomerID 12350.0 hasn't transacted in a while (301 days ago), had only 1 transaction, and spent 334.40.

![3](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/d59ca8ee-b5fb-4127-ad2a-0405967684ed)

![output](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/a982fd94-1a93-4ac1-b072-a901fe44f4c9)


- Customer lifetime value (CLV)

1- CustomerID: This is a unique identification number for each customer. It allows the business to differentiate between individual customers.

2- CLV (Customer Lifetime Value): This represents the projected net profit attributed to the entire future relationship with a customer. In other words, it's an estimation of how much each customer is worth to the business over the duration of their relationship. The higher the CLV, the more valuable that customer is to the business.

- Quick Analysis:

CustomerID 17841.0 has the highest CLV of 2,976,046.0. This implies that this customer is projected to bring the most net profit to the business over the duration of their relationship compared to the other customers listed.
CustomerID 14646.0 has the second-highest CLV with 558,978.0.
CustomerID 18102.0 is close behind with a CLV of 512,877.0.
The remaining customers have CLVs in descending order, with CustomerID 14911.0 having the lowest CLV among this list at 265,145.0.

![Screenshot 2023-07-06 195320](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/dd698805-7a56-49b5-9fe7-4f93cba4ee3e)
