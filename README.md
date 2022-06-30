# Amazon_Vine_Analysis

## Project Overview
Assist the client to determine if there is any bias toward favorable reviews from Vine members. I did so by picking a dataset from a set list and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the data into pgAdmin. 

## Methodology
Tools/Programs/Languages used:

- Google Colab
- Python / PySpark
- AWS RDS
- ETL operations
- SQL
- pgAdmin
- Excel

##
- I used PySpark to import data from an S3 bucket and read it as a dataframe.

![image](https://user-images.githubusercontent.com/44425379/176713636-67421df2-604b-4819-b02a-8f5a9940f22a.png)

- Then, I cleaned up the data and filtered the data by the amount of reviews and stars given by Amazon Vine Members and Non-Amazon Vine Members.
- This led me to create 3 different tables. 

![image](https://user-images.githubusercontent.com/44425379/176714525-d6b8e338-2f66-4fc4-8f36-3f46454230bf.png)

![image](https://user-images.githubusercontent.com/44425379/176714562-dded9241-0a05-4dd0-9aee-27421aba6592.png)

- Afterwards, I connected to an AWS RDS (cloud database) instance and added each "clean" DataFrame to its corresponding table.

![image](https://user-images.githubusercontent.com/44425379/176715338-a6af0bd9-0a7d-4552-823d-35f86ad41ae9.png)

- Once I confirmed connection to the cloud database, I then linked AWS to my database in pgAdmin. I used basic SQL queries to make sure the data loaded correctly.


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

### Conclusion
- I would conclude that there is no positivity bias for reviews in the Vine program as they are such a small percentage of the total reviews.
- Only about a third of the total vine reviews had 5 star reviews. 
