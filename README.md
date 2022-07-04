## Project Overview

This repo contains project files for an Analysis of Jumia Kenya's Offers. 

The project aims to answer the following research questions;<b>
1. Is there a correlation between the price of products and their offers? If yes, is it possible to predict offers given price?
2. How many product categories does jumia feature in its offers?
3. What are the top 5 categories with the most number of items on offer?
4. What 5 categories have the least number of items on offer?
5. What are the min, max, average, and standard deviation of offer prices?
6. How many products have the max and minimum discounts?
7. Plot for the distribution of discounts. Is it normally distributed?
8. Assuming there was only 1 item in stock when you ran this script;

        . what is the value of all products on offer?

        . What is the value of products in their given categories? 
        
9. Split the dataset into a train, validation, and test groups and create a machine learning model to predict offers given prices.
10. What is the significance of this project?</b>


The project utilizes the following data science concepts;

### a. Data mining & Web scraping.

I created my dataset by scraping jumia Kenya's website for all products that were on offer.

The script scraped a total of 46 pages returning about 1,154 products.

The following data was collected:
    - Name of the Products
    - Category of the Product
    - Link to the image of the product
    - Price of the Products
    - Offer price at which the products are sold
    - Percentage discount on each product

I then stored the scraped data into a sqlite3 database which I later used to make a pandas data frame.

### b. Data Cleaning

I utilized the following techniques to clean my data;

- <b>Outliers</b>
Using the standard deviation method (3 stds) to clean numerical columns.
- <b>Missing Values</b>
Initially, the scraped data did not have any null values. However, after removing outliers on the price and offer columns the issue of null values came about.
Since the percentage of the missing data was negligible (0.6%) I opted to drop all the rows with missing values.
- <b>Structural Errors in string</b>

### c. Data Visualization

I utilized various visualizations within the project to showcase;
 - Presence of outliers in the dataset
 - Distribution of prices

### d. Data Analysis

At the end of the project, I performed a comprehensive analysis to answer the research questions.



