# Online-Retail-Customer-Segmentation

Greetings everyone, my name is Rajat Srivastava and I am excited to present my fourth capstone project! In this project, I will be conducting data analysis and visualization while also creating an unsupervised machine learning clustering model. Before diving into the project presentation, let's first briefly go over the problem statement and the steps involved in the process.

We have been provided with transaction data from a UK-based online retailer that specializes in unique all-occasion gifts. Our main goal is to segment customers into distinct groups based on their purchasing behavior and characteristics, which will allow us to develop targeted marketing strategies to improve customer retention and increase sales.

Here's an overview of the process we followed:

First, we needed to understand the data to get a better business context. We had access to customer IDs, product IDs, product costs, country, invoice numbers, and dates. Once we understood the data, we did some data wrangling to check for null values, duplicates, and created some new features as per our requirements.

Next, we performed customer behavior and product performance analysis. This analysis helped us develop marketing strategies, optimize pricing, and tailor promotions to specific customer segments, as well as make informed decisions about inventory management and product development.

After that, we conducted hypothesis tests by formulating a null hypothesis and an alternative hypothesis. We then chose a significance alpha level to determine the threshold for rejecting the null hypothesis. We compared the p-value to the alpha level and accepted or rejected the null hypothesis accordingly using ANOVA and t-tests. These hypothesis tests helped us understand patterns and relationships in the data, identify significant differences between groups or segments, and make data-driven decisions.

We then did feature engineering and selection. As we were doing customer segmentation and creating clustering algorithms, it was important to have certain KPIs to categorize customers based on their purchase behavior. So, we performed RFM analysis and created a new data frame with variables for recency, frequency, and monetary, along with customer IDs, which we fed into our clustering algorithms. Recency indicates how recently a customer made a purchase, Frequency indicates how often a customer makes a purchase, and Monetary indicates how much a customer spent on purchases.

We removed outliers using the IQR method, which is particularly useful for data that is not normally distributed or has a high degree of skewness. As our data was highly right-skewed, we also applied log transformation as it helped normalize the data and reduce the impact of outliers.

Before data modeling, we scaled the data using standard scaler as Recency, Frequency, and Monetary were likely to be measured using different scales. By applying the standard scaler, we could bring them to a common scale and ensure that they were equally weighted.

Next, we implemented the KMeans machine learning model. We created a simple model by selecting the optimal cluster using the elbow method. Then, we created a hyperparameter-tuned KMeans model using the best parameters obtained using grid search CV. Similarly, we implemented a hierarchical clustering model as well.

Finally, we compared and chose the best performing model using industry knowledge, business requirements, and taking into consideration the silhouette score, Calinski-Harabasz index, and Davies-Bouldin index scores. We also found the feature importance of the chosen model using the SHAP model explainability tool. Lastly, we saved the best performing model as a pickle file and predicted unseen data for sanity check.
