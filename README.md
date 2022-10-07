# Cryptocurrencies

## Overview of the Analysis
Unsupervised learning uses machine learning algorithms to analyze and cluster unlabeled data sets. These algorithms discover hidden patterns in data without the need for human intervention. Unsupervised learning models are used for three main tasks: clustering, association and dimensionality reduction.

Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company is getting confused between vast variety of cryptocurrencies. This project is about create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. The data needs to be processed to fit the machine learning models. Clustering algorithm will be used in this project.

## Results
### Deliverable 1: Preprocessing the Data for PCA
Create crypto_df dataframe with following changes.
- All cryptocurrencies that are not being traded are removed
- The IsTrading column is dropped
- All the rows that have at least one null value are removed
- All the rows that do not have coins being mined are removed
- The CoinName column is dropped.
<img width="552" alt="crypto_df" src="https://user-images.githubusercontent.com/106944351/194599611-b64d3de5-62a6-4661-8039-a3e8e03b5979.png">


### Deliverable 2: Reducing Data Dimensions Using PCA
The pcs_df DataFrame is created and has the following three columns, PC 1, PC 2, and PC 3, and has the index from the crypto_df
<img width="880" alt="pcs_df" src="https://user-images.githubusercontent.com/106944351/194601972-57d5655e-9705-49c5-80b1-7857f9240ccd.png">


### Deliverable 3: Clustering Cryptocurrencies Using K-means
- An elbow curve is created using hvPlot to find the best value for K 
<img width="773" alt="elbow_curve" src="https://user-images.githubusercontent.com/106944351/194602244-492eeb6a-af0e-45f3-9c00-c9127af2c6d5.png">


A new DataFrame (scaled_df) is created with the same index as the crypto_df DataFrame and has the following columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class
<img width="1259" alt="scaled_df" src="https://user-images.githubusercontent.com/106944351/194602326-6ce7ac59-e630-4588-a021-88a2c4a1f496.png">


### Deliverable 4: Visualizing Cryptocurrencies Results
3D scatter plot created
<img width="1009" alt="3D_scatter_plot" src="https://user-images.githubusercontent.com/106944351/194603098-4d949163-3ff7-4fe1-b99e-0a4fb1446eb7.png">


Create a table with tradable cryptocurrencies using the hvplot.table() function.
<img width="1260" alt="hvplot table()" src="https://user-images.githubusercontent.com/106944351/194603131-26f55177-f56e-49a9-b508-1b1fa128a2da.png">


Add CoinName and Class columns in clustered_df
<img width="997" alt="clustered_df" src="https://user-images.githubusercontent.com/106944351/194603198-0b0e59ce-f571-4d83-bf90-f0e37df47ff4.png">


Hvplot scatter plot
<img width="1259" alt="hvplot(scatter)" src="https://user-images.githubusercontent.com/106944351/194603223-a9786318-009c-4c33-bd05-967b6b4fea13.png">


## Summary
Each group needs to be analyzed in detail to get to the conclusion that which cryptocurrency will work better for bank's clients.


