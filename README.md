# Financial-aid-for-countries-clustering-and-pca
# Understanding of Data and Approach 
From the data we can see that it is of unsupervised machine learning problem.
The features in the dataset is aboumut the various indices of the countries, based on those indices we have to determine which of these countries require the financial aid during any disaster.
As these features or indices are derived from different parameters and metrics if we use scaling for these features it would might loose there significance.
We can use PCA to reduce the dimensionality and have uncorrelated features.
Now to prepare our data for clustering we will use PCA.
To determine the optimum number of features which explains about 80-90% of the variance we will use SCREE plot which is the line plot between the cumulative sum of explained variance ratio and number of principal components 
From the scree plot we can see that 4 Principal components are explaining about 87% of variance. So, we'll take 4 prinicipal components for our clustering.
We still encounter the problem of outliers in the PCA data, we can either delete these outliers if removing them not cause so much lose in data or we can cap these outliers.
