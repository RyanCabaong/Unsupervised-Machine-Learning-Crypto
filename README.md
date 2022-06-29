# Unsupervised-Machine-Learning-Crypto
Unsupervised Learning is a machine learning technique in which the users do not need to supervise the model. Instead, it allows the model to work on its own to discover patterns and information that was previously undetected.

Finding useful insights, hidden patterns from the unknown dataset is the objective of the unsupervised learning.

Unsupervised Learning includes various algorithms like KNN, Apriori Algorithm, and Clustering.

For this project I am using Clustering.

First, I needed to preprocess the data to perform PCA (Principal Component Analysis) using pandas’ library.

- Unfortunately, I was having difficulties Installing hvplot and plotly packages so I had to do a “!pip install”. 

- I dropped all cryptocurrency that wasn’t active with the IsTrading column.

-Dropped rows with null values
-Kept rows where coins are mined
-Drop the Name column for algorithm
-Create a new dataframe copy including the changes
-features from the X DataFrame have been standardized using the StandardScaler
