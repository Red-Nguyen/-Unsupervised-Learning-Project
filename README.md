Part I: EDA 
- Exploratory Data Analysis & Pre-processing
  
	Data Import: Load the dataset.

	Data Cleaning: Handle missing data and correct errors.

	Data Description: Compute summary statistics.

	Data Visualization: Create visualizations to explore relationships.

	Outlier Detection: Identify and handle outliers.

	Correlation Analysis: Examine correlations between features.

	Data Transformation: Standardize or normalize data.

	Feature Selection: Determine important features using PCA.
	
Part II: KMeans Clustering
	- Determine optimal clusters.
	- Pre-process data.
	- Initialize centroids.
	- Assign data points to clusters.
	- Update centroids.
	- Repeat until convergence.
	- Cluster analysis:
        	- Cluster 0 (Luxury Grocery Shoppers): High spending on Milk, Grocery, and Detergents_Paper. Moderate spending on Fresh.
       	 	- Cluster 1 (Fresh Produce Enthusiasts): Predominantly purchases Fresh products, followed by Frozen goods. Also, spends moderately on Milk, Grocery.
        	- Cluster 2 (Grocery Bulk Buyers): Major purchases are made in the Grocery category, closely followed by Fresh and Milk. They also have a considerable purchase of Detergents_Paper.
       	 	- Cluster 3 (Budget Shoppers): Low spending across all categories except for Fresh, Frozen & Grocery
	
Part III: Hierarchical Clustering

	- Pre-process data.
	- Determine optimal clusters using dendrogram.
	
Part IV: PCA - Principal Component Analysis

	- Analyze variance explained by each principal component.
	- Cluster analysis:
        	- Cluster 0:  Given their high spending on Milk, Grocery, and Detergents_Paper but lower spending on Detergents_Paper and frozen products, this cluster likely represents stores that don't focus on perishable items. These could be smaller supermarkets or convenience stores.
        	- Cluster 1: Given their high spending on Fresh items and low spending on Delicassen and Detergents_Paper, these are likely establishments that need a lot of fresh produce. This points towards restaurants, cafes, or fresh markets.
        	- Cluster 2: This cluster has a diversified spending pattern, leaning more towards Fresh, Milk, and Grocery items, but also has a significant spend on Delicassen. This could represent larger supermarkets or hypermarkets which have a broad range of items, including specialty or delicacy items.
Part V: Conclusion

	1. EDA: 
		- The data does not follow a normal distribution.
		- Some features exhibit high correlation:
			- Detergents_Paper & Grocery: 0.89
			- Grocery & Milk: 0.77
			- Detergents_Paper & Milk: 0.70
		- Some features have low correlation:
			- Frozen & Grocery: -0.16
			- Milk & Fresh: -0.14
			- Frozen & Milk: -0.05    
			- Features with the highest importance specific to Principal Component Analysis (PCA) are: Grocery, Milk, Detergents_Paper.
	2. KMeans Clustering:
		- The data can be effectively separated into 4 clusters.
		- Using log transformation and standard scaling improves clustering results with this data. 
	3. Hierarchical Clustering :
		- The data can also be separated into 3 clusters effectively using hierarchical clustering. 
	4. PCA:
		- PC1 captures 44.4% of the variance in the data
		- PC2 captures 25.6%
		- PC3 captures 11.1%
		- PC4 captures 10.6%
		- PC5 captures 4.9%
		- PC6 captures the remaining 3.1%.
