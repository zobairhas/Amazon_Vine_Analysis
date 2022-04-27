# Amazon_Vine_Analysis

## Project Overview
Assist the client to determine if there is any bias toward favorable reviews from Vine members. I did so by picking a dataset from a set list and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the data into pgAdmin. 

## Methodology
Tools/Programs/Languages used:

- Google Colab
- Python / PySpark
- pgAdmin
- AWS (RDS)
- ETL

## Summary of Results
- How many Vine reviews and non-Vine reviews were there?
  - Total Vine Reviews = 613
  - Total non-Vine Reviews = 64,968

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  - Total Vine 5 star reviews = 222
  - Total non-Vine 5 star Reviews = 30,543


- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  - Percentage Vine 5 star reviews = 0.7%
  - Percentage non-Vine 5 star reviews = 99.3%

- I would conclude that there is no positivity bias for reviews in the Vine program as they are such a small percentage of the total reviews.
- Only about a third of the total vine reviews had 5 star reviews. 
