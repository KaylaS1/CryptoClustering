# Week 11 Crypto Clustering Notebook

## Classify cryptocurrencies according to their price fluctuations across various timeframes using K-Means and PCA

### Step 1:
* Read in and scale the cryptocurrencies price percent change data from the csv file.
* Find the best value for k using scaled data and a plot showing the elbow curve.
* Note that the best value for k seems to be 5 using scaled data.
* Cluster cryptocurrencies using K-Means and scaled data and display using a scatter plot.

### Step 2: Principal Component Analysis (PCA)
* Using PCA, reduce the original scaled dataframe to 3 features.
* Retrieve the total explained variance of the 3 principal components.
* Find the best value for k using PCA data and a plot showing the elbow curve.
* Note that the best value for k seems to be 4 using scaled data.
* Cluster cryptocurrencies using K-Means and PCA data and display using a scatter plot.
* Display the weight of each feature on the principal components.

### Conclusions:
* The best value for k appears to be 5 using scaled data, but changes to 4 when PCA data is used.
* If scaled dataframe is reduced to 3 features for a Principal Component Analysis, the total explained variance of the 3 principal components is over 89%. 
* 'price_change_percentage_200d' and 'price_change_percentage_1y' have the strongest positive influence on PCA1. 'price_change_percentage_24h' has the strongest negative influence on PCA1.
* 'price_change_percentage_30d', 'price_change_percentage_14d' and 'price_change_percentage_60d' have the strongest positive influence on PCA2.
* 'price_change_percentage_7d' has the strongest positive influence on PCA3 and 'price_change_percentage_60d' has the strongest negative influence on PCA3.