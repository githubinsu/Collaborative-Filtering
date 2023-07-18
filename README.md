# Collaborative Filtering for Product Recommendation
## Collaborative Filtering
Collaborative filtering involves analyzing the purchase histories of users to calculate the similarity between them. This information is then used to recommend products to each user based on the purchases of other similar users. For example, if “User A and User B have similar purchase histories,” then products purchased by User A but not by User B could be recommended to User B.

## Objective
The goal of this project is to use collaborative filtering to generate personalized product recommendations for customers. 

## Data Description
I have utilized publicly available sales data, which has been anonymized and processed for the purpose of analysis.
The dataset contains transaction data, where each row represents an individual order and the columns include information such as Order Date, Customer ID, Product Number, Price, Sector, Category, and Subcategory.

## Method
I used the surprise library to implement collaborative filtering. First, I preprocessed the data by creating a rating for each product based on the number of times a customer has purchased it. Then, I used the surprise library to train an SVD model on this data.

## Results
The resulting recommendations represent products that are likely to be of interest to a specific customer based on their purchase history. By recommending products that are likely to be relevant, we can increase customer satisfaction and sales.

## Performance Evaluation
The performance of the collaborative filtering model can be evaluated using metrics such as RMSE and MAE. In this case, the model achieved an RMSE of 0.4972 and an MAE of 0.2959 during cross-validation, indicating that it has excellent performance as both values are below 0.5.

## Future Applications
This collaborative filtering code can be used by stores to make personalized product recommendations to their customers. One of the main advantages of collaborative filtering is that it can help users discover new interests by recommending items that similar users are interested in, even if the system may not know that the user is interested in that item. This can lead to serendipitous recommendations and increase customer engagement. In addition, this analysis can be extended to other areas such as market basket analysis and customer segmentation.
