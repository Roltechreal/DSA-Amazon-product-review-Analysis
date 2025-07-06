# DSA-Amazon-product-review-Analysis
a Retail tech company provided us with their product and customer review data to generate insights that can guide product improvement, marketing strategies, and customer engagement.
## Project Topic: Amazon Product Review Analysis.
## Introduction 
a  retail tech company provided us with unsorted data for us to analyze and give feedback in order for them to make decisions with the analysis output, The dataset contains information scraped from Amazon product pages, including: 
   1. Product details: name, category, price, discount, and ratings, 
   2. Customer engagement: user reviews, titles, and content. 
     Each row represents a unique product, with aggregated reviewer data 
stored as comma-separated values 
### Total Records: 1,465 
### Total Fields: 16 columns 
     
we had to clean the data, then analyse before visualizing. it has beeen a great experience working on data as a data analyst, we used Excel as a tool to achieve the end result of this project.  

## Project overview
by Analysing the various parameters in the data received, we seek to gather enough insight to make reasonable decisions which can enable us to find compelling stories around our data from the insight gotten and to know the best performing from our data.
## Data source
The data is gotten from scraped Amazon product pages. 

## Tools used
we used Microsoft Excel in achieving this project

## Data Cleaning
In the initial phase of data cleaning, the following where carried out:
### Data Loading and inspection
Data cleaning and formatting, we added some calculated columns.

#### Some analytical questions were asked in order to find solutions to the problems 
1. What is the average discount percentage by product category?
2. How many products are listed under each category?
3. What is the total number of reviews per category?
4. Which products have the highest average ratings?
5. What is the average actual price vs the discounted price by categor
6. Which products have the highest number of reviews?.
7. How many products have a discount of 50% or more?
8. What is the distribution of product ratings (e.g., how many products are rated 3.0,
4.0, etc.)?
9. What is the total potential revenue (actual_price × rating_count) by category?
10. What is the number of unique products per price range bucket (e.g., <₹200,₹200–₹500, >₹500)?.
1. How does the rating relate to the level of discount?
12. How many products have fewer than 1,000 reviews?
13. Which categories have products with the highest discounts?
14. Identify the top 5 products in terms of rating and number of reviews combined.

## Analysis

we first of all, clean the data before we start our analysis.
in this analysis, category is the primary key. we added some calculated columns. 
To get the average discount percent, calculated column was created with the dormular = Actual price-Discounted price/actual price * 100). 
we added calculated column to know the product that have a discount of 50% or more with the formular
= IF( Discount %>=50,"yes,"No") .

We added another Calculated Column called Total Potential Revenue, we use thw formula to get = (Actual price* Rating Count). 

We created a new Column called Column Price Bucket with the formula =IF (Discounted price<200,"<₹200"
IF(Discounted price <=500")).

To calculate dor the top 5 products by rating plus number of reviews xombines, we created calculated column with the formula = Average Rating+ (Ratimg count/ scaling factor).

### Providing solutions to the questions raised earlier with regards to the data.
1. Average discount percentage by product category is gotten from our pivot table, where we put category in Rows and Discount % as values, we summarize by Average. The iamage below shows the results of this result of this analysis.

2. To know the number of Products listed under category, we use Pivots table by placing category in Rows and products name in value ( we set to count Dist). Below is the result.

3. For Total number is of reviews per category, a pivot table was created, Category is placed underRows and Rating count and was placed under values. below is the result.

4. Products with the highest Average ratings, the data was sorted out ( The Average Column in descending order).

5. Average actual price vs discounted price, pivot table were used. Category is set under the Rows, actual price and Discounted price was placed under values. the result is shown below.

6. Products with the highest number of reviews, Rating count column was sorted in descending order as shown below.

7. Number of Products with a discount of 50% or more, we use a Count IF functions.

8. Distribution of product rating, we use pivot table, The rating is used as the Rows and Peoduxt name as Values as shown below.

9. Total potential revenue by category, we use pivot table by putting category in Rows and potential Revenue 





