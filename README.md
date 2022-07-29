# Amazon_Vine_Analysis

## Overview of the analysis: 

This is an analysis of the Amazon Vine program using one of the 50 datasets provided.  The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. Using the Mobile Apps dataset and PySpark to perform the ETL process to extract the dataset and transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Using PySpark again to determine if there is any bias toward favorable reviews from Vine members in the Mobile Apps dataset. 

## Results: 

- How many Vine reviews and non-Vine reviews were there?

![image](https://user-images.githubusercontent.com/101137700/181662860-2b7d646c-eb10-40ba-b259-1e8a4fddf198.png)

As demonstrated above there were zero Vine reviews for any of the mobile apps in this data set.

![image](https://user-images.githubusercontent.com/101137700/181662875-3259a47c-1adb-4bce-879e-22ff26674005.png)

And here you can see literally all the other reviews in this dataset.


- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

![image](https://user-images.githubusercontent.com/101137700/181663212-973a668f-247d-44c3-82f5-ed8b5295ba5a.png)

Since there were zero Vine reviews to begin with, there were zero 5 star vine reviews.

![image](https://user-images.githubusercontent.com/101137700/181663298-7fc19727-ca09-43a2-8379-402c225e025f.png)

But seen here there is only 59,278 5 star non-Vine reviews.

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

![image](https://user-images.githubusercontent.com/101137700/181663377-0287ba39-f48b-4094-9abc-db6a1cf18191.png)

The Vine percentage an obvious 0% but the non-Vine percentage of 5-star reviews comes in at 45.77%

It won't even let me try to find the percentage of the Vine reviews since you can not divide by zero. 

## Summary: 

There is zero bias for Vine reviews because there wasn't even any submitted for all 129,516 mobile apps in the dataset that was used. Can't really have a bias if no one even participated in the review program. There really isn't even an additional analysis that can be done to further examine bias.
