# Cryptocurrencies Analysis

## Description of the Project

Martha is a senior manager for the Advisory Services Team at Accountability Accounting, one of my most important clients. Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. So, they’ve asked me to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment.

The data Martha will be working with is not ideal, so it will need to be processed to fit the machine learning models. Since there is no known output for what Martha is looking for, she has decided to use unsupervised learning. To group the cryptocurrencies, Martha decided on a clustering algorithm. She’ll use data visualizations to share her findings with the board.

## Unsupervised Machine Learning Process 

**1. Preprocessing the data for PCA:** I organized the data by formatting, cleaning and sampling it, to perform PCA.

**2. Reducing Data Dimensions using PCA:** I reduced the dimensions of the X DataFrame to three principal components to placed them in a new DataFrame called pcs_df.

**3. Clustering Cryptocurrencies using K-means:** I created an elbow curve using hvplot to find the best value for K from the pcs_df DataFrame. Then I ran the K-means algorithm to predict the K clusters for the cryptocurrencies data.

**4. Visualizing Cryptocurrencies Results:** I visualized the distinct gropus that correspond to the three principal components that I created before, and then, I created a table with all the currently tradable cryptocurrencies using the hvplot.table function.

## Results
### Elbow Curve

![image](https://user-images.githubusercontent.com/108365182/199527406-01dd8e43-fa41-4f34-b781-84315b3b470d.png)

### Distinct groups visualization 

![image](https://user-images.githubusercontent.com/108365182/199526412-f0e20611-a9f8-461b-8acd-8ad886773bc1.png)

### Scatter plot with x="TotalCoinsMined", y="TotalCoinSupply", and by="Class"

![image](https://user-images.githubusercontent.com/108365182/199527210-fffec736-54d8-4f7d-937b-a675e07e71cb.png)

