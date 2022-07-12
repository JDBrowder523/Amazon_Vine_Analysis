# Amazon_Vine_Analysis

## Overview:

 The purpose of this analysis is to use AmazonAWS and Google Colab to analyze product reviews from Amazon to determine the relationship between paid Vine and unpaid reviews.  The dataset used is book review data and can be downloaded from the following webpage: "https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Books_v1_02.tsv.gz".

## Results:
 - The data was filtered to only include books with more than 20 reviews.  This eliminated all of the paid reviews, as the only 2 instances of paid reviews had 3 and 6 total votes, respectively.  The code used to determine this is shown below:

 ![This is an image](https://github.com/JDBrowder523/Amazon_Vine_Analysis/blob/main/Images/only_paid_reviews.png)

 - The results were filtered to show only the books that had more than 20 votes and had greater than 50% of their total votes being helpful votes. Using this filtered DataFrame, the following statistics were determined:

### Total Paid and Unpaid Reviews:

 - The total number of Vine (paid) reviews is 0 and the total number of non-Vine (unpaid) reviews is 375,353. Since the total number of Vine reviews is 0 for the filtered dataset, we will ignore this part of the data for the rest of the analysis.

 ![This is an image](https://github.com/JDBrowder523/Amazon_Vine_Analysis/blob/main/Images/total_paid_vs_unpaid.png)

### Total 5 Star Unpaid Reviews:

 - The total number of non-Vine (unpaid) reviews is 226,910.

 ![This is an image](https://github.com/JDBrowder523/Amazon_Vine_Analysis/blob/main/Images/total_5star_reviews.png)

### Percentage of 5 Star Unpaid Reviews:

 - The percentage of non-Vine (unpaid) reviews is 60.45%.

 ![This is an image](https://github.com/JDBrowder523/Amazon_Vine_Analysis/blob/main/Images/percentage_5star_reviews.png)

## Summary:

 There are only 2 Vine (paid) reviews in this dataset, which is a very small sample size.  Therefore, it is not helpful to use this information to determine a relationship between the Vine and non-Vine reviews.  We can, however, conclude that the lack of Vine reviews shows that the vine program does not put much emphasis on book reviews.  
 An additional analysis could be performed to get the summary statistics for all reviews to determine the mean, median, and IQR values.  This could be used to determine if there is a relationship between the number of votes and the star rating.
