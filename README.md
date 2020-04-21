# Financial-aid-for-countries-clustering-and-pca
# Understanding of Data and Approach 
1. From the data we can see that it is of unsupervised machine learning problem.
2. The features in the dataset is aboumut the various indices of the countries, based on those indices we have to determine which of these countries require the financial aid during any disaster.
3. As these features or indices are derived from different parameters and metrics if we use scaling for these features it would might loose there significance.
4. We can use PCA to reduce the dimensionality and have uncorrelated features.
5. Now to prepare our data for clustering we will use PCA.
6. To determine the optimum number of features which explains about 80-90% of the variance we will use SCREE plot which is the line plot between the cumulative sum of explained variance ratio and number of principal components 
8. From the scree plot we can see that 4 Principal components are explaining about 87% of variance. So, we'll take 4 prinicipal components for our clustering.
9. We still encounter the problem of outliers in the PCA data, we can either delete these outliers if removing them not cause so much lose in data or we can cap these outliers.
10. The hopkins score is 75% which states that our data set is good for clustering 
11. From elbow curve and sillhouete score we can see that 4 clusters are optimum number of clusters 
12. We combine the clustering results with the original dataset to determine the clusters of the countries 
13. As there are many features we will reduce our analysis to 3 features Net income, GDP per capita and Child Mortality Rate. If the countries have above 0.85 quantile child mortality, below 0.15 Net income and GDP will be in dire need of funds for in case of disaster.
14. Heirarchical clustering also have same countries clustered in dire need of financial aid as KMeans clustering.
