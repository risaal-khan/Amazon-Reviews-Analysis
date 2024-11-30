# Amazon Reviews Analysis with Sentimental Analysis
One of the most important problems in e-commerce is the correct calculation of the points given to after-sales products. The solution to this problem is to provide greater customer satisfaction for the e-commerce site, product prominence for sellers, and a seamless shopping experience for buyers. Another problem is the correct ordering of the comments given to the products. The prominence of misleading comments will cause both financial losses and customer losses. In solving these 2 basic problems, e-commerce site and sellers will increase their sales, while customers will complete their purchasing journey without any problems.

## About
* This dataset containing Amazon Product Data includes product categories and various metadata. 

## Objective
* The product with the most comments in the electronics category has user ratings and comments. In this way, we expect you to perform sentiment analysis with your specific methods.

## Dataset Description   

This dataset contains Amazon product reviews, including details about reviewers, ratings, and calculated metrics. Below are the column descriptions:

## Column Descriptions

| Column Name            | Description                                                                           |
|------------------------|---------------------------------------------------------------------------------------|                                  
| `reviewerName`         | Name of the person who submitted the review.                                          |
| `overall`              | Overall rating given to the product by the reviewer (usually on a scale of 1 to 5).   |
| `reviewText`           | Text content of the review provided by the customer.                                  |
| `reviewTime`           | Date when the review was submitted.                                                   |
| `day_diff`             | Number of days since the review was submitted.                                        |
| `helpful_yes`          | Number of "helpful" votes the review received.                                        |
| `helpful_no`           | Number of "not helpful" votes the review received.                                    |
| `total_vote`           | Total number of votes (helpful and not helpful) the review received.                  |
| `score_pos_neg_diff`   | Difference between the number of helpful and not helpful votes.                       |
| `score_average_rating` | Average score based on the ratio of helpful votes to total votes.                     |
| `wilson_lower_bound`   | Lower bound of Wilson Score for ranking reviews based on helpfulness.                 |

## Insights

1. #### Sentiment Score Distribution
* The distribution of sentiment scores shows that the majority of reviews fall between 0.0 and 0.4, indicating a generally neutral to slightly positive sentiment among customers.
* The highest frequency of sentiment scores is observed in the 0.2 to 0.4 range, suggesting most customers have a moderately positive view.

![image](https://github.com/user-attachments/assets/44687f5c-43ee-4f90-9150-811b5d93fdf0)

2. #### Average Sentiment by Quarter and Year
* Trend: Sentiment scores generally decrease from Q1 to Q3 and then slightly increase in Q4 across the years 2012, 2013, and 2014.
* Highest Sentiment: The year 2014 has the highest average sentiment scores overall, indicating improved customer satisfaction in that year.

![image](https://github.com/user-attachments/assets/e53b7bb1-3f8f-4bb6-b85e-e187db58899c)

3. #### Wilson Lower Bound by Review Text
* The review text "UPDATE" has the highest Wilson lower bound score, indicating a high level of confidence in its positive sentiment. 
* This suggests that updates or follow-up reviews tend to be more positively received.

4. #### Overall Rating and Sentiment Comparison
* There is a clear correlation between higher overall ratings (4 and 5 stars) and higher sentiment scores, while lower ratings (1 and 2 stars) are associated with lower sentiment scores.
* This suggests that customers who give higher ratings also express more positive sentiments in their reviews.

![image](https://github.com/user-attachments/assets/fe28f742-9c35-4ead-809f-82b15726eb91)

5. #### Average Rating by Quarter and Year
* Similar to sentiment scores, the average ratings show a general decrease from Q1 to Q2 and an increase towards Q4.
* The year 2014 shows the highest overall average ratings, indicating better product performance or customer satisfaction.

![image](https://github.com/user-attachments/assets/58739b1c-b695-4432-b9c5-312c98fce801)

6. #### Summary Metrics
* Total Votes: 7478, indicating active engagement from customers in reviewing and voting.
* Overall Rating: 4.59, suggesting a generally high level of satisfaction with the products.
* Total Reviews: 4915, showing a substantial volume of customer feedback.

![image](https://github.com/user-attachments/assets/c1d34eca-4334-41ea-a5fe-c3cc593bbed6)

7. #### Percentage of Helpful Reviews
* Only 6% of the reviews are marked as helpful, indicating that a small portion of reviews are perceived as valuable by other customers.

8. #### Total Helpful and Unhelpful Reviews
* Helpful Reviews: There are 413 helpful reviews.
* Unhelpful Reviews: There are 241 unhelpful reviews.
* This suggests that while a minority of reviews are deemed helpful, there is a significant number of reviews that customers do not find useful.

9. #### Most Helpful Reviews
* The top review received nearly 2000 helpful votes, significantly more than others. This indicates that certain reviews resonate strongly with customers, providing valuable insights or guidance.
* Reviews with high helpful votes often contain detailed and specific information, making them more useful to potential buyers.

10. #### Products with Reliable Ratings
* A scatter plot shows the distribution of ratings against the Wilson lower bound, indicating the reliability of product ratings.
* Products with higher Wilson lower bound scores are more likely to have consistent and reliable ratings, suggesting a general consensus among reviewers about the product quality.

![image](https://github.com/user-attachments/assets/273d13aa-c4dd-4252-9312-1adbd56c6e9e)

11. #### Helpful and Unhelpful Reviews by Rating
* 5-Star and 1-Star Reviews: These ratings have the highest counts of both helpful and unhelpful reviews.
* This suggests that extreme ratings (very positive or very negative) attract more attention and engagement from customers, who may find these reviews more compelling or polarizing

12. #### Least Helpful Reviews
* These reviews have negative helpful counts, indicating they were not useful to other customers.
* The least helpful reviews often lack detail or fail to provide actionable information, reducing their value to potential buyers.

13. #### Average Review Length by Helpful Count
* Reviews with higher helpful counts tend to be longer, containing more detailed information.
* This highlights the importance of comprehensive reviews in helping customers make informed purchasing decisions.

14. #### Percentage of Helpful Reviews by Month and Year
* The percentage of helpful reviews fluctuates over different months and years, with no clear upward or downward trend.
* This suggests variability in the perceived helpfulness of reviews over time, potentially influenced by factors like product releases or changes in review guidelines.

![image](https://github.com/user-attachments/assets/03d087f7-6968-4cb9-a1de-5a1b006a088b)

15. #### Total Votes by Month and Year
* Noticeable peaks occur in february 2013, May & June 2013, and October 2012. These peaks could correspond to major product launches or seasonal shopping periods.

![image](https://github.com/user-attachments/assets/1f7e775a-01ff-47a0-a745-325586115644)

16. #### Average Sentiment Score by Month
* The horizontal bar chart indicates that the average sentiment score is relatively consistent across months, with minor variations.
* This suggests a generally steady sentiment across different times of the year.

![image](https://github.com/user-attachments/assets/e7a6dfaa-971d-4ce7-b2a7-9971630a92c7)

17. #### Helpful Count by Sentiment Score
* The scatter plot shows most data points clustered around a sentiment score of 0, with a few outliers.
* Higher sentiment scores tend to correlate with more helpful votes, indicating that more positive reviews are often seen as more helpful by other users.

18. #### Average Sentiment Score
* The average sentiment score is 0.28, indicating that reviews are slightly positive on average.
* This score reflects the general sentiment trend over the period analyzed.

19. #### Weighted Rating Distribution
* The bar chart shows the highest frequency of ratings at 3.00, followed by 1.00 and 2.52.
* The weighted rating distribution helps understand the overall perception of products based on review ratings.
