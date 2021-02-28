# Analyzing Swarovski jewellery

Author: Nadine Mukondiwa

Date: 22 February 2021

------

[TOC]

------

## Introduction

Earrings have always been my favourite pieces of jewellery. Usually, I buy more affordable jewellery from Amazon or Walmart. However, in this project, I was interested in analyzing how much Swarovski products cost to decide how much to save to buy something from the brand. Ideally, I would like to purchase earrings, but the analysis includes other types of jewellery.

Questions I planned to answer

- Is there an equal number of products in each category?
- What is the average price of products in each category?
- What is the average price of products based on the plating? 
- What is the distribution of earring prices?
- What are different discount amounts available for earrings?



## Methodology

### Data gathering

To gather the data, I used the requests and Beautiful Soup libraries to do web scraping of the "Earrings," "Necklaces and Pendants," "Bracelets," "Rings," and "Brooches" webpages. I then used pandas for data cleaning and data manipulation. 

### Statistical analysis

To test the assumption that the categories have an equal number of products, I used the Chi-square goodness of fit test. 

To determine the budget, I found the confidence interval of the average price.

### Data visualization

I used the Seaborn library for data visualization. 

## Results

### Is there an equal number of products in each category?

![product_count](C:\Users\ndmuk\OneDrive\Data Analysis Projects\Data Analyst Portfolio Projects\Portfolio projects\Insights projects\FINAL FINAL Portfolio Projects\Swarovski Analysis\images\product_count.png)

The categories do not have an equal number of products in each category. The necklaces and pendants category has the most products, and the Brooches category has the least. 

### What is the average price of products in each category?

![](C:\Users\ndmuk\OneDrive\Data Analysis Projects\Data Analyst Portfolio Projects\Portfolio projects\Insights projects\FINAL FINAL Portfolio Projects\Swarovski Analysis\images\avg_price.png)

Earrings have one of the lowest average prices. Products from the Atelier Swarovski collection are costly. Necklaces and pendants' average price is **$601.50**, and the average cost of earrings collection was **$391.14**.  

### What is the average price of products based on the plating?

![](C:\Users\ndmuk\OneDrive\Data Analysis Projects\Data Analyst Portfolio Projects\Portfolio projects\Insights projects\FINAL FINAL Portfolio Projects\Swarovski Analysis\images\plating_avg.png)

As seen in chart 3, Ruthenium plated products have a large distribution of prices. Rose-gold tone plated items have the least variability, and they also have some of the lower prices among the different types of plating, but they do have a lot of expensive outliers.  

### What is the distribution of earring prices?

![](C:\Users\ndmuk\OneDrive\Data Analysis Projects\Data Analyst Portfolio Projects\Portfolio projects\Insights projects\FINAL FINAL Portfolio Projects\Swarovski Analysis\images\earring_distribution.png)



Chart1 in the appendix shows that 75% of the earrings cost under **$200**. However, if I wanted to get any earrings pair, I could save as much as **$500** because the highest price is **$479**. 

### What different discount amounts are available for earrings?

![](C:\Users\ndmuk\OneDrive\Data Analysis Projects\Data Analyst Portfolio Projects\Portfolio projects\Insights projects\FINAL FINAL Portfolio Projects\Swarovski Analysis\images\discounts.png)

Of the products on sale, most of them were at a 50% discount. 


## Conclusion

Using a confidence interval of 99%, the average price of Swarovski earrings is between **$142.17** and **$177.93**. Therefore I decided that **$200** would be a reasonable amount to save up for earrings. Lastly, waiting for a future sale could save much money because I could save up to 50% on some earrings, so I will make sure to wait for a sale.

## Appendix

Chart 1

![](C:\Users\ndmuk\OneDrive\Data Analysis Projects\Data Analyst Portfolio Projects\Portfolio projects\Insights projects\FINAL FINAL Portfolio Projects\Swarovski Analysis\images\prices_distribution.png)



Chart 2

![](C:\Users\ndmuk\OneDrive\Data Analysis Projects\Data Analyst Portfolio Projects\Portfolio projects\Insights projects\FINAL FINAL Portfolio Projects\Swarovski Analysis\images\prices_jitter.png)

Chart 3



![](C:\Users\ndmuk\OneDrive\Data Analysis Projects\Data Analyst Portfolio Projects\Portfolio projects\Insights projects\FINAL FINAL Portfolio Projects\Swarovski Analysis\images\plating_boxplot.png)