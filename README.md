# Amazon_Vine_Analysis
The first part of the challenge is using PySpark to perform the ETL process to extract, transform and load data of the Amazon major appliances dataset to PostgreSQL.  After data is loaded, Amazon vine review data it is exported as a csv file and loaded into Python for further analysis to determine if there is any bias toward favorable reviews from Vine members in your dataset.

## Results
- How many Vine reviews and non-Vine reviews were there?
  There were 35 Vine reviews and 4957 non-Vine reviews in the major appliances dataset.
![review_number]

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  There were 18 5-star reviews that is part of the Vine program.  For non-Vine, there were a total 1,963 5-star review.
![5_star_reviews_number]

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  51.4% of the Vine reviews were 5 stars while only 39.6% of non-Vine reviews were 5 stars.
![5_star_percentage]

## Summary
- The mean star rating for Vine reviews is 4.37 while for non-Vine reviews the mean is 3.25.  After running the 2 samples t-test, since the p-value is smaller than 0.01, there is significant statistical evidence to support that the mean star rating of Vine and non-vine reviews are different. Together, with percentage of 5-star reviews percentage of Vine program (51.4%) way higher than non-Vine program (69.6%).  We can conclude that there is positivity bias for reviews in the Vine program.

- Statistical analysis (e.g. 2 sample t-test) could be applied to the 1-star rating reviews to verify if Vine program favour the product more than non-Vine users.