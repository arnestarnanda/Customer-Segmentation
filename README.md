# Customer Segmentation
# Use Case
#### Use Case Summary
#### Objective Statement:
* To find out the total amount of income in each year
* To find out how much the difference in the total amount of income/revenue per month in each year.
* To know how to optimize marketing strategies to the right customers to generate more revenue 
* Get customer segmentation using RFM model.

#### Challenges:
* Large size of dataset
* Dataset have different data types.
* Transactional Data

#### Methodology / Analytic Technique:
* Exploratory analysis (Graph Analysis)
* Clustering Model
* Segment Analysis using RFM

#### Business Benefit:
* Know how to treat customers with specific criteria.
* Increase business revenue.
* Marketing Strategy Right on Target

#### Expected Outcome:
* Know how many the total amount of revenue in each year
* Know how many the difference in the total amount of revenue per month in each year.
* Ability to optimize marketing strategies to the right customers to generate more revenue 
* Get customer segmentation using RFM model.

# Business Understanding
Retail is the process of selling consumer goods or services to customers through multiple channels of distribution to earn a profit.
<br>
This case requires data-driven answers to the following questions:
* How much is the total amount of income/revenue in each year ?
* How much is the difference in the total amount of income/revenue per month in each year?
* How to make the ability to optimize marketing strategies to the right customers to generate more revenue ?
* How to get customer segmentation using RFM model ?

# Data Understanding
* Data of a retail transaction from 04 January 2011 to 31 December 2014
* The dataset has 4 columns and 5009 rows.

#### Data Source
* Source Data: https://www.kaggle.com/datasets/siddinho/sample-orders-dataset-retail    

#### Data Dictionary 
* Order Date 	: Transaction date
* Order Id		: Order code of each transaction
* Customer		: Customer's name
* Grand Total	: Total customer spending

# Data preparation
Code Used :
* Python Version :Python 3.8.8
* Packages : Pandas, Numpy, Matplotlib, Seaborn, Datetime, Warnings.

# Data Cleansing
* The order_date data type which is an object is wrong because the column value is a transaction date which should be a datetime data type, so we need to change the order_date data type from the object to datetime.
* Create a new column that takes only the year and month from the order_date column.

# Exploratory Data Analysis
### How much is the grand total per month in each year and which month has the highest and lowest grand total in each year?
* 2011
![2011](https://user-images.githubusercontent.com/109860070/201472703-8125fb61-5da4-461b-ba30-d8bff0b0977b.png)
Based on the graph above, **February is the month with the lowest total sales of 1%**, while **September is the month with the highest total sales of 16.9%**. From January to February it **decreased by 1.9%**, then from February to March it experienced a **significant increase of 10.5%**, then from March to April it **decreased by 5.7%**. And from April to August there was no significant increase, then from August to September there was an **increase of 11.1%**, but from September to October there was a very large **decrease up to 10%**, then from October to November **increased by 9.7%**. and closed at the end of the year in November with a percentage of **14.4% of total revenue in each month**.

* 2012
![2012](https://user-images.githubusercontent.com/109860070/201472709-91408713-c3cb-4357-b582-6f1e64660b1f.png)
Based on the graph above, **February is the month with the lowest grand total of 2.6%**, while **November is the month with the highest grand total of 16.1%**. The grand total in **January 2012 was higher than in January 2011 to 3.9%**, then in February it **decreased to 2.6%**. In March it experienced a **significant increase to 8.2%** and in April it **decreased slightly to 7.3%**. Furthermore, in May it **decreased to 6.4%** and in June also **decreased to 5.3%** before in July it **increased again to 6.1%**. In August the grand total **increased to 7.8%** and in September it **increased significantly to 13.7%**, then in October it **decreased significantly to 6.7%**. The end of the year had a very high grand total, **November was 16.1%** and December **slightly decreased to 15.9%**.

* 2013
![2013](https://user-images.githubusercontent.com/109860070/201472719-3d0693fc-dca4-4071-bec5-5cddd5d891fe.png)
Based on the graph above, **January is the month with the lowest grand total of 3%**, while **December is the month with the highest grand total of 16%**. 2013 started with a relatively low grand total, amounting to **only 3% in January**, then in February it **increased to 3.8%** and in March it **increased to 8.4%**. In April it **decreased to 6.5%** and in March it **increased again to 9.3%**. It then **fell in June to 6.5%**. The highest grand total in the first half was in May with a percentage of 9.3%. Entering the second half of 2013, the grand total for **July and August did not differ significantly**, in July it was 6.3% and in August it was 5.5%. In the following month or September, there was a **significant increase in the grand total of up to 12%**. sales tend to **increase** at the end of the year, in November by 14% and in December by 16%.

* 2014
![2014](https://user-images.githubusercontent.com/109860070/201472721-c0ae0fbb-31ec-45f1-9e80-3b85d927fef1.png)
Based on the graph above, **February is the month with the lowest grand total of 2.8%**, while **November is the month with the highest grand total of 15.3%**. The grand total in **January** this year was not as low as the previous year at **6.1%** and then **decreased to 2.8%** and in March **rose significantly to 7.3%**. Three months later, **the grand total went up gradually**. The grand total in **April was 5.5%**, in May it **increased by 6.2%**, in June it **increased by 6.6%**. The grand total was **stagnant from June to July, both at 6.6%**. Then in August it **increased to 8.4%**, in September it **increased to 12.3%** before **decreasing in October to 10.6%**. After that, the grand total in November **increased to 15.3%** and in December **decreased again to 12.3%**.

 
