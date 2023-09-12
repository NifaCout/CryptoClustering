# CryptoClustering
Challenge 19
**Prepare the Data**
  •	Used the StandardScaler() module from scikit-learn to normalize the data from the CSV file.
  •	Created a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

**Find the Best Value for k Using the Original Scaled DataFrame**
  •	Created a list with the number of k values from 1 to 11.
  •	Created an empty list to store the inertia values.
  •	Created a for loop to compute the inertia with each possible value of k.
  •	Created a dictionary with the data to plot the elbow curve.
  •	Plotted a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for      k.
**Cluster Cryptocurrencies with K-means Using the Original Scaled Data**
  •	Initialize the K-means model with the best value for k.
  •	Fit the K-means model using the original scaled DataFrame.
  •	Predict the clusters to group the cryptocurrencies using the original scaled DataFrame.
  •	Created a copy of the original data and add a new column with the predicted clusters.
  
**Optimize Clusters with Principal Component Analysis**
  •	Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components.
  •	Retrieve the explained variance to determine how much information can be attributed to each principal component and then answer       the following question in your notebook:
  o	What is the total explained variance of the three principal components?
  •	Created a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new       
    DataFrame.
**Visualize and Compare the Results**
