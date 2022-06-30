# Unsupervised-Machine-Learning-Crypto
Unsupervised Learning is a machine learning technique in which the users do not need to supervise the model. Instead, it allows the model to work on its own to discover patterns and information that was previously undetected.

Finding useful insights, hidden patterns from the unknown dataset is the objective of the unsupervised learning.

Unsupervised Learning includes various algorithms like KNN, Apriori Algorithm, and Clustering.

For this project I am using Clustering.

First, I needed to preprocess the data to perform PCA (Principal Component Analysis) using pandas’ library.

- Unfortunately, I was having difficulties Installing hvplot and plotly packages so I had to do a “!pip install”. 

- I dropped all cryptocurrency that wasn’t active with the IsTrading column.

- Dropped rows with null values

- Kept rows where coins are mined

- Drop the Name column for algorithm

- Create a new dataframe copy including the changes

![image](https://user-images.githubusercontent.com/79386482/176541891-a106639f-64b7-4694-811a-31e31998a7e9.png)


- features from the X DataFrame have been standardized using the StandardScaler

- Using PCA to reduce dimension to three principal components.

![image](https://user-images.githubusercontent.com/79386482/176541741-43435f2f-e684-4e72-b8e5-250b37d3b728.png)


- Create an elbow curve to find the best value for K

- Initialize the K-Means model, Fit the model, Predict clusters

![image](https://user-images.githubusercontent.com/79386482/176542095-85fc8dea-b283-497f-972e-abdb816ad9a7.png)

- Add back the Column 'CoinName' and Append predicted data column 'Class'

![image](https://user-images.githubusercontent.com/79386482/176574421-0e06bc49-3dd4-40fa-8dad-097eed3d9b53.png)

- Finally, make a 3D scatterplot with the PCA data and clusters
