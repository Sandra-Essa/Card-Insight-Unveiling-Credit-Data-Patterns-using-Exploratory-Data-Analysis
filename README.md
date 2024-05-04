# Discover-Credit-Data-Patterns-Card-Insight-through-Exploratory-Data-Analysis


- [Business Problem](#Business-Problem)
- [Business Questions](#Business-Questions)
- [Data Preparation and Exploration](#Data-Preparation-and-Exploration)
- [User-Defined Function for Analysis](#User-Defined-Function-for-Analysis)


## Business Problem

- The project aims to conduct an exploratory data analysis (EDA) within the Credit Card Industry. Its primary goal is to assist the company in offering proactive services to customers, expanding its market share, and reducing customer churn. The focus lies in analyzing the dataset to understand its key characteristics using various visual methods, ultimately leveraging the data to make informed decisions.

## Business Questions

1) How many distinct customers are there?
2) How many different customer segments exist?
3) What is the average monthly spending per customer?
4) What is the average monthly repayment per customer?
5) If the monthly interest rate is 2.9%, what is the bank's monthly profit?
6) What are the top 5 product types?
7) Which city has the highest spending?
8) Which age group spends the most money?
9) Who are the top 10 customers in terms of repayment?
10) How does city-wise spending on each product vary on a yearly basis?
11) How does the total spend vary monthly across different cities?
12) What is the yearly expenditure pattern for air tickets?
13) How does monthly spending differ across various product categories?


## Data Preparation and Exploration

1) Cleaned data by replacing invalid age values and adjusting spend and repayment amounts exceeding limits.
2) Identified distinct customers and categories, checked data types, and handled missing values.
3) Created summaries for distinct customers, categories, average monthly spend and repayment, interest calculations, top products, city-wise spend, age group spending, and top customers in repayment.
4) Handling Age Data: If any customer's age is less than 18, it is replaced with the mean age value to ensure consistency and accuracy in the analysis.
5) Managing Spend Amount: If a customer's spend amount exceeds their limit, the spend amount is adjusted to 50% of their limit. The limit is obtained from the acquisition table, representing the per transaction limit on the customer's card.
6) Addressing Repayment Amount: If the repayment amount exceeds the limit, the repayment is set to the limit to maintain data integrity and relevance for further analysis.
7) Calculate Interest Earned: Apply a monthly interest rate of 2.9% on positive monthly profits. Interest is earned only on positive profits, not on negative amounts.
8) Conducted graphical analysis for monthly spend comparison, yearly spend on air tickets, monthly spend on products, and city-wise spend.

##  User-Defined Function for Analysis

Created a function summ(Product, timeperiod) to find top 10 customers for each city in terms of repayment amount, based on specified product (Gold/Silver/Platinum) and time period (yearly or monthly).

