Part I: EDA 
	- Exploratory Data Analysis & Pre-processing
	- Data Import: Load the dataset.
	- Data Cleaning: Handle missing data and correct errors.
	- Data Description: Compute summary statistics.
	- Data Visualization: Create visualizations to explore relationships.
	- Outlier Detection: Identify and handle outliers.
	- Correlation Analysis: Examine correlations between features.
	- Data Transformation: Standardize or normalize data.
	- Feature Selection: Determine important features using PCA.
	
Part II: KMeans Clustering
	- Determine optimal clusters.
	- Pre-process data.
	- Initialize centroids.
	- Assign data points to clusters.
	- Update centroids.
	- Repeat until convergence.
	
Part III: Hierarchical Clustering
	- Pre-process data.
	- Determine optimal clusters using dendrogram.
	
Part IV: PCA - Principal Component Analysis
	- Analyze variance explained by each principal component.
	
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
			- Features with the highest importance specific to Principal Component Analysis (PCA) are: Fresh, Delicassen, Frozen.
	2. KMeans Clustering:
		- The data can be effectively separated into 4 clusters.
		- Using log transformation and standard scaling improves clustering results with this data. 
	3. Hierarchical Clustering :
		- The data can also be separated into 4 clusters effectively using hierarchical clustering. 
	4. PCA:
		- PC1 captures 44.4% of the variance in the data
		- PC2 captures 25.6%
		- PC3 captures 11.1%
		- PC4 captures 10.6%
		- PC5 captures 4.9%
		- PC6 captures the remaining 3.1%.
