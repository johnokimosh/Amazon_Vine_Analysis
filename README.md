# Amazon_Vine_Analysis

## Overview of the analysis: Explain the purpose of this analysis.

Client requests analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

1. Select 1 of approximately 50 datasets with reviews of a specific product, from clothing apparel to wireless products.
2. Use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin.
3. Use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset.
4. Write a summary of the analysis for client to deliver to key stakeholders.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions:
![final_table](https://user-images.githubusercontent.com/27740513/148696554-e96f276b-3ef5-4dec-8c3e-7921113cc2b3.png)

1. How many Vine reviews and non-Vine reviews were there?
- Total Vine (paid) reviews were 90.
- Total Non-Vine (unpaid) reviews were 37,385
2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- Total Vine (paid) 5-Star reviews were 44
- Total Non-Vine (unpaid) 5-Star reviews were 37,385
3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
- Percentage of Vine (paid) 5-Star reviews were 48.89%
- Percentage of Non-Vine (unpaid) 5-Star reviews were 39.12%

## Summary:

1. Is there any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement.
- Vine reviews have a positivy bias of approximately 9.77 percentage points. It can be assumed that when a customer is selected to review an free product for the program they are rating the product higher compared to a customer purchasing the same products.

2. Provide one additional analysis that you could do with the dataset to support your statement.
![verified_table](https://user-images.githubusercontent.com/27740513/148704659-11d8ec3f-d66f-425e-a0da-ff0ff80362d5.png)

- Per Amazon: An "Amazon Verified Purchase" review means we've verified that the person writing the review purchased the product at Amazon and didn't receive the product at a deep discount.

- A. Total Verified Non-Vine (unpaid) reviews were 9,355
- B. Total Verified Non-Vine (unpaid) 5-Star reviews were 3,594
- C. Percentage of Verifired Non-Vine (unpaid) 5-Star reviews were 38.42%

- After completing an additional analysis to filter "verified purchases" the to get an more accurate representation of customer who actually purchased the products, the positive bias for Vine reviews increases by 10.47 percentage points.
