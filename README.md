# CryptoClustering

## Module 19 Challenge

For this challenge, I analyzed cryptocurrency price changes over time to predict if they are affected by 24-hour or 7-day price changes. I used unsupervised learning methods, including KMeans and Principal Component Analysis (PCA) to accomplish this machine learning challenge.

Some of the libraries I used include sklearn, where I imported KMeans, PCA, and StandardScaler for normalizing the imported data (via pandas DataFrames). I also used hvplot.pandas to create scatter plots and line charts. The line charts were done to showcase the Elbow Method, while scatter plots were used for displaying the clustered data.

Some of the processes learned and used throughout the notebook include preparing the data via the StandardScaler module. This allowed for the data to be scaled and normalized appropriately before running the models on it. I also identified the best value for k via the Elbow Method, where I run the KMeans model on a range of potential k values and plot their inertia values on a line chart. Once the best number of clusters is identified, the KMeans model is ran on the original data with it and predicted clusters are produced. Finally, a scatter plot comparing price changes 24-hour and price changes 7-days is produced with the predicted clusters. In addition, the process is repeated using the PCA model, where the data is reduced to three principal components. After identifying the explained variance ratio, the Dataframe containing the PCA data is used to run the Elbow Method and clustered with KMeans. In the end, the resulting plots are compared to the previously created plots to surmise the impact of reducing the features.