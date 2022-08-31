# Amazon Vine Analysis
## Overview of the analysis
The purpose of this project is to analize Amazon reviews written by members of the paid Amazon Vine program and determine if there is any bias toward favorable reviews from Vine members.

We will pick one of the 50 datasets available and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Afterwards, we will perform a series of calulation to conclude if there is any bias.

## Data Source
- [Amazon Review Dataset](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Pet_Products_v1_00.tsv.gz)
## Results
### Vine Reviews Result
![Paid](https://github.com/msevillano89/Amazon_Vine_Analysis/blob/main/Images/Paid.png)

### Non-Vine Reviews Result
![Unpaid](https://github.com/msevillano89/Amazon_Vine_Analysis/blob/main/Images/Unpaid.png)

- **How many Vine reviews and non-Vine reviews were there?** There were a total of 170 Vine reviews and 3,7840 non-Vine reviews.

- **How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?** There were a total of 65 5-stars Vine reviews and 2,0612 5-stars non-Vine reviews.

- **What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?** 38.24% of Vine reviews were 5-stars and 54.47% of non-Vine reviews were 5-stars.

## Summary
As noted in the results, we the is some positivity bias for reviews in the Vine program as almost 39% of all reviews resulted in 5-star reviews.It would be helpful to perform descriptive statiscal analysis and developed a histogram to determine the frequency of the reviews for Vine and non-Vine users.
