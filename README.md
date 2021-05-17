# Amazon_Vine_Analysis

## Project Overview

This project is designed to analyze Amazon reviews written by members of the paid Amazon Vine program. This program is a service that allows manufacturers and publishers to recieve reviews for their products. 

In this project, approximately 50 datasets were accessable to choose from and analyze. For this specific analysis, I chose to look at outdoor supplise. I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin ([ETL process code](https://github.com/Ariannatopbjerg/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb)). I then used PySpark to determine if there is any bias toward favorable reviwes from Vine members in the dataset ([bias analysis code](https://github.com/Ariannatopbjerg/Amazon_Vine_Analysis/blob/main/Vine_Review_Analysis.ipynb)). 

## Results

- How many Vine reviews and non-Vine reviews were there?

  Total Vine reviews

  ![](https://github.com/Ariannatopbjerg/Amazon_Vine_Analysis/blob/main/images/total_paid.PNG)

  Total non-Vine reviews

  ![](https://github.com/Ariannatopbjerg/Amazon_Vine_Analysis/blob/main/images/total_unpaid.PNG)

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

  Total 5 star Vine reviews

  ![](https://github.com/Ariannatopbjerg/Amazon_Vine_Analysis/blob/main/images/5star_paid.PNG)

  Total 5 star non-Vine reviews

  ![](https://github.com/Ariannatopbjerg/Amazon_Vine_Analysis/blob/main/images/5star_unpaid.PNG)

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

  Percentage of 5 star Vine reviews

  ![](https://github.com/Ariannatopbjerg/Amazon_Vine_Analysis/blob/main/images/percent_paid.PNG)

  Percentage of 5 star non-Vine reviews

  ![](https://github.com/Ariannatopbjerg/Amazon_Vine_Analysis/blob/main/images/percent_unpaid.PNG)

## Summary

By looking at the above results, there is no positive bias for reviews in the Vine program. Both Vine and non-Vine reviews showed a 52% 5 star rate for the products, which indicates that the Vine:non-Vine reviews ratio is almost equal to eachother.

An additional analysis that could be done to support my above statement would be to analyse the mean, median, and mode of the star ratings for the Vine and non-Vine reviews.
