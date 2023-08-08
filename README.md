## Customer-Segmentation

### Goal
The goal of this repo is to make use of unsupervise machine learning techniques to segment customers into clusters, so that we can apply appropriate marketing strategies towards each individual cluster. 

### Motivation
The motivation behind this repo is to learn unsupervised ML techniques, and to compare the pros and cons of each clustering algorithms. (K-Means vs Hierarchical) 

### K-Means Clustering
How it works is that, we first randomly select the number of clusters that we want. This represents the 'K' in 'K-Means Clustering'.
So if we select 3 clusters, it will be 3-Means Clustering. 
Then, we would have to randomly select 3 distinct data points, since we have chosen 3 clusters. 
Then, measure the distance between the 1st point, with the 1st cluster point. Then, the 2nd point with the 1st cluster point so on... 
Those nearest to 1st cluster point will be labelled as X. Those nearest to 2nd cluster point will be labelled as Y. Those nearest to 3rd cluster point will be labelled as Z. 

Next, we will calculate the means of each cluster 1, 2, 3. 
Now that the data are clustered, we will then sum the variance of these clusters. Then repeat the first step where the 3 cluster points are randomly selected. It will keep going on until the variance is the least biased among all 3 clusters. 

#### For K-Means clustering, it is important to find the optimal number of clusters: 
Need to first specify the number of clusters. 
We can make use of WCSS to find the optimal number of clusters after apply K-Means with different number of cluster.
WCSS formula is as follows: 

![WCSS](https://github.com/chingjie98/Customer-Segmentation/assets/35895182/afd98c69-1615-43c7-aa7b-fafd01ce9363)

It is simply the euclidean distance between 2 points. Think of it as pythagorams theorem, and trying to find the distance of C. 
After we use the WCSS techniques, we will be able to plot out the graph which indicate the distance between each centroid to the other depending on the number of clusters. 
With lesser cluster, the higher the WCSS. 
We are looking for an 'elbow' which is known as the 'elbow' method so that we can find the optimal number of clusters. 

![elbow](https://github.com/chingjie98/Customer-Segmentation/assets/35895182/70e6256f-1a6d-4bdc-8821-3544e24702d0)
