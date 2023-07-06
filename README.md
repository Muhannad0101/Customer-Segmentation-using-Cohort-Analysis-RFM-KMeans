# Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans

### Content
"This is a transnational data set which contains all the transactions occurring for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers."

Per the UCI Machine Learning Repository, this data was made available by Dr Daqing Chen, Director: Public Analytics group. chend '@' lsbu.ac.uk, School of Engineering, London South Bank University, London SE1 0AA, UK.

### Solution
Here, I performed an analysis and created a Dashboard using Tableau to display the results of the total sales data for each country with the months for each time of the day, for example morning and evening periods, and so on from the billing time, and compared the profits against the transactions. also I create a dashboard for the top 5 countries, the top 10 clients, and the top ten descriptions.


- Cohort Analysis:
The result is a cohort analysis heatmap that shows the retention rates of customers over time. The data is organized into cohorts based on the month in which a customer made their first purchase.

The columns represent the number of months since the customer's first purchase, and the rows represent the cohort month (i.e., the month in which the cohort made their first purchase).

Some cells in the heatmap have missing or NaN values, indicating that there were no customers in the cohort who made a repeat purchase in that particular month.

![1](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/6c6ffa4c-c67f-4830-bf16-6bad6e275fa4)


- RFM (Recency, Frequency, Monetary)
The "Recency" column represents the number of days since the customer's last purchase. Customers with lower recency values are more recently active and engaged with the business.

The "Frequency" column represents the number of purchases made by the customer. Customers with higher frequency values are more engaged and loyal to the business.

The "Monetary" column represents the total amount of money spent by the customer. Customers with higher monetary values are more valuable to the business.

Negative values in the recency column indicate that the customer made a purchase more recently than the date of the analysis. For example, customer 12347 made a purchase 7 days after the date of the analysis.

The Recency metric has a positive skewness value of 1.2489, indicating that the distribution has a longer tail on the right side and that there are more customers with low recency values (i.e., recently active) than high recency values. The frequency and monetary metrics have even higher positive skewness values of 63.8631 and 55.6776, respectively, indicating that the distributions are highly skewed towards customers with low frequency and monetary values.

Skewness test results indicate whether the skewness value is different from zero, which would indicate a symmetrical distribution. The p-value in the test result represents the probability of obtaining a skewness statistic as extreme as the one observed, assuming that the null hypothesis of a symmetrical distribution is true. In this case, the p-values for all three RFM metrics are very small, much smaller than the commonly used significance level of 0.05, indicating strong evidence against the null hypothesis and confirming that the distributions are highly skewed.

![3](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/d59ca8ee-b5fb-4127-ad2a-0405967684ed)

![2](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/52e485b4-8f6b-42df-a328-1ca78558e28d)

![output](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/a982fd94-1a93-4ac1-b072-a901fe44f4c9)


- Customer lifetime value (CLV)
is a metric that estimates the total amount of money a customer is expected to spend throughout their lifetime as a customer of a business. It is an important metric for because it helps to identify their most valuable customers and inform marketing and retention strategies to encourage these customers to continue making purchases and remain loyal.

For example, customer 17841 has a CLV of 2,976,046 currency units, indicating that they are expected to generate almost 3 million units of revenue for the business throughout their lifetime as a customer. This customer is likely very loyal to the business and makes frequent purchases, contributing to their high CLV value.

![Screenshot 2023-07-06 195320](https://github.com/Muhannad0101/Customer-Segmentation-using-Cohort-Analysis-RFM-KMeans/assets/102443619/dd698805-7a56-49b5-9fe7-4f93cba4ee3e)
