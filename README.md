# Cryptocurrencies

## Overview of the Analysis
Unsupervised learning uses machine learning algorithms to analyze and cluster unlabeled data sets. These algorithms discover hidden patterns in data without the need for human intervention. Unsupervised learning models are used for three main tasks: clustering, association and dimensionality reduction.

Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company is getting confused between vast variety of cryptocurrencies. This project is about create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. The data needs to be processed to fit the machine learning models. Clustering algorithm will be used in this project.

## Results
1) Deliverable 1: Preprocessing the Data for PCA
Create crypto_df dataframe with following changes.
- All cryptocurrencies that are not being traded are removed
- The IsTrading column is dropped
- All the rows that have at least one null value are removed
- All the rows that do not have coins being mined are removed
- The CoinName column is dropped.


2) Deliverable 2: Reducing Data Dimensions Using PCA
The pcs_df DataFrame is created and has the following three columns, PC 1, PC 2, and PC 3, and has the index from the crypto_df DataFrame



3) Deliverable 3: Clustering Cryptocurrencies Using K-means
- An elbow curve is created using hvPlot to find the best value for K 


A new DataFrame (scaled_df) is created with the same index as the crypto_df DataFrame and has the following columns: Algorithm, ProofType, TotalCoinsMined, TotalCoinSupply, PC 1, PC 2, PC 3, CoinName, and Class


4) Deliverable 4: Visualizing Cryptocurrencies Results
3D scatter plot created


Create a table with tradable cryptocurrencies using the hvplot.table() function.


total number of tradable cryptocurrencies in the clustered_df DataFrame.


Add CoinName and Class columns in clustered_df


Hvplot scatter plot


## Summary
Each group needs to be analyzed in detail to get to the conclusion that which cryptocurrency will work better for bank's clients.


