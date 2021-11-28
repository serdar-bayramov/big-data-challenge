# big-data-challenge

## Background

Many of Amazon's shoppers depend on product reviews to make a purchase. Amazon makes these datasets publicly available. However, they are quite large and can exceed the capacity of local machines to handle. One dataset alone contains over 1.5 million rows; with over 40 datasets, this can be quite taxing on the average local computer. Your first goal for this assignment will be to perform the ETL process completely in the cloud and upload a DataFrame to an RDS instance. The second goal will be to use PySpark or SQL to perform a statistical analysis of selected data.

Create DataFrames to match production-ready tables from two big Amazon customer review datasets.

The datasets used for this project:
* Music reviews
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Music_v1_00.tsv.gz

* Mobile electronics reviews
https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Mobile_Electronics_v1_00.tsv.gz


## Steps in this project:

1. Create PostgreSQL database locally using PgAdmin
2. Create tables in PostgreSQL:

2.1 review_id_table
2.2 customers table
2.3 products table
2.4 vine table

3. Create PostgreSQL database in AWS RDS
4. Connect successfully PgAdmin to server AWS RDS
5. Create 2 google colab noteboooks and load the data from https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt
6. Transform the data such that they are suitable to load into the tables in the database
7. Query the data to make sure they are successfully loaded

