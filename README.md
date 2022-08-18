# Customer Segmentation

**PROBLEM OVERVIEW:**</br>
Customer segmentation is the process by which you separate customers up based on their common characteristics – such as demographics or spending behaviors, so we can market to those customers more effectively. It can help a business to better understand its target audience and better implementation of marketing strategies, thereby potentially driving an increase in customer loyalty and other marketing metrics. 
We will be segmenting the customers in our source data using unsupervised machine learning algorithms.</br>

**OUR BUSINESS OBJECTIVE:** </br>
•	Segment customers to better provide targeted services for business & sales improvement

**REVIEW OF DATA SOURCE**
- Our data source is a csv file.
- The data has 541909 rows and 8 columns. We have sales data related to customers. 
- The variables are InvoiceNo, StockCode, Description, Quantity InvoiceDate, UnitPrice, CustomerID  and Country  

</br>

## MODELS

**K_means_clustering:**
Determining number of clusters for our rfm uk data.
To determine the optimal number of clusters, we have to select the value of k at the “elbow” i.e the point after which the distortion/inertia start decreasing in a linear fashion. Thus for the given data, we conclude that the optimal number of clusters for the data is 3.
After removing the outliers from our data, we apply k means clustering which gives us 3 clusters of customers.

**Result:**
- Cluster 0 has low monetary values, a wide range of recency and low frequency. 
- Cluster 1 has high monetary values, low recency and moderate frequency
- Cluster 2 have moderate monetary values, low to moderate frequency and low to moderate recency. 
This is also evident by the means of these values for every cluster

![image](https://user-images.githubusercontent.com/86319382/185499873-8c4036f8-6486-4fd3-b944-540109ef3b37.png)

 
**Recommendations:**
 Cluster 0 are at the most risk of churning. They spend less and shop less frequently.
We can set up a referral selling plan for these customers, in which they get offers by referring other customers to the business.
Cluster 1 are good customers as they are big spenders and shop often and more recently. There should be a rewards point for these so they remain loyal to the business.
Cluster 2  customers need more attention. As the recency is very high, it is possible these customers shopped only once. We can contact these customers and do a feedback survey.

**Hierarchical clustering method**
For Hierarchical clustering we determine the number of clusters from the dendrogram which comes out to be 2.
This model gives us 2 clusters instead of 3.
The mean values for our clusters are,

![image](https://user-images.githubusercontent.com/86319382/185499831-5009b522-2d4a-4169-b20e-4eaf2a1a2ed9.png)


 **Results:**
Cluster 0 define good/loyal customers while cluster 1 are customers that are risky or need attention.

**Recommendations:**
We can start a rewards/offers program for customers in cluster 0 while for cluster 0 we can start a feedback survey that targets multiple aspects like quality, customer service, price etc.
