# Unsupervised-ML
In this repository, I learned unsupervised Machine Learning technique and how to find the best hyperparameter in each algorithm of DBscan, kmean, Hierarchical Clustering, and GaussianMixture.learn how to clean the dataset and preprocessing and how to use silhouette_score. finally, learn PCA and how to use it.

## 1. DBscan clustering:
Density-Based Clustering refers to unsupervised learning methods that identify distinctive groups/clusters in the data, based on the idea that a cluster in data space is a contiguous region of high point density, separated from other such clusters by contiguous regions of low point density.

  1.1 The DBSCAN algorithm uses two parameters:
  
    minPts: The minimum number of points (a threshold) clustered together for a region to be considered dense.

    eps (ε): A distance measure that will be used to locate the points in the neighborhood of any point.
  
  1.2 There are three types of points after the DBSCAN clustering is complete:
  
    Core — This is a point that has at least m points within distance n from itself.

    Border — This is a point that has at least one Core point at a distance n.

    Noise — This is a point that is neither a Core nor a Border. And it has less than m points within distance n from itself.
  
  ![1_yT96veo7Zb5QeswV7Vr7YQ](https://user-images.githubusercontent.com/101005712/207862051-5835243e-312e-432f-913d-09c298b3f40f.png)
  
  [click there to find Code of DBscan clustering](https://github.com/AlaaSayed164/Unsupervised-ML/blob/main/DBSCAN--Class%2018_Blank.rar)
  
  ## 2. kmean clustering:
K-means clustering is one of the simplest and most popular unsupervised machine learning algorithms. Typically, unsupervised algorithms make inferences from datasets using only input vectors without referring to known, or labeled, outcomes. identifies k number of centroids, and then allocates every data point to the nearest cluster, while keeping the centroids as small as possible.

  -It halts creating and optimizing clusters when either:

    The centroids have stabilized — there is no change in their values because the clustering has been successful.

    The defined number of iterations has been achieved.

![method-k-means-steps-example](https://user-images.githubusercontent.com/101005712/207865880-9c57427f-a12f-4b8a-80b1-e8316e383bb9.png)

  [click there to find Code of kmean clustering](https://github.com/AlaaSayed164/Unsupervised-ML/blob/main/k%20mean.ipynb)


 ## 3. Hierarchical Clustering clustering:
Hierarchical clustering is a popular method for grouping objects. It creates groups so that objects within a group are similar to each other and different from objects in other groups. Clusters are visually represented in a hierarchical tree called a dendrogram.

-Hierarchical clustering has a couple of key benefits:

  * There is no need to pre-specify the number of clusters. Instead, the dendrogram can be cut at the appropriate level to obtain the desired number of clusters.
  
  * Data is easily summarized/organized into a hierarchy using dendrograms. Dendrograms make it easy to examine and interpret clusters.
  
-Applications:

There are many real-life applications of Hierarchical clustering. They include:

  * Bioinformatics: grouping animals according to their biological features to reconstruct phylogeny trees

  * Business: dividing customers into segments or forming a hierarchy of employees based on salary.

  * Image processing: grouping handwritten characters in text recognition based on the similarity of the character shapes.

  * Information Retrieval: categorizing search results based on the query.
  
-There are two main types of hierarchical clustering:

  * Agglomerative: Initially, each object is considered to be its own cluster. According to a particular procedure, the clusters are then merged step by step until a 
  single cluster remains. At the end of the cluster merging process, a cluster containing all the elements will be formed.

  * Divisive: The Divisive method is the opposite of the Agglomerative method. Initially, all objects are considered in a single cluster. Then the division process 
  is performed step by step until each object forms a different cluster. The cluster division or splitting procedure is carried out according to some principles that 
  maximum distance between neighboring objects in the cluster.

  ![0_afzanWwrDq9vd2g-](https://user-images.githubusercontent.com/101005712/207868597-d23740ae-5aab-4556-a417-7ffcdcba1f43.png)
 
 -Similarity between Clusters:
  * Min (Single) Linkage: find the minimum distance between points in those clusters. That is, we can find the point in the first cluster nearest to a point in the 
  other cluster and calculate the distance between those points. 
  
  ![Sample-data-min-distance-single-linkage width-1200](https://user-images.githubusercontent.com/101005712/207869017-e065a1e5-8258-4a27-8abb-929aaa5728fc.jpg)

  * Max (Complete) Linkage: find the maximum distance between points in two clusters. We can find the points in each cluster that are furthest away from each other and 
  calculate the distance between those points.
  
  ![Sample-data-max-distance-complete-linkage width-1200](https://user-images.githubusercontent.com/101005712/207871973-d19b290b-7688-4221-a815-1dbdb3e854f7.jpg)
  
  * Average Linkage:The Average method defines the distance between clusters as the average pairwise distance among all pairs of points in the clusters.
  
  ![Sample-data-average-distance-linkage width-1200](https://user-images.githubusercontent.com/101005712/207872482-72314948-fdc4-42ae-b748-c16dd3a9f48b.jpg)

  *  Centroid Linkage: defines the distance between clusters as being the distance between their centers/centroids. After calculating the centroid for each cluster, 
  the distance between those centroids is computed using a distance function.
  
  ![Sample-data-centroid-distance-linkage width-1200](https://user-images.githubusercontent.com/101005712/207872311-35856c8a-7d37-47d4-9bb4-af426ee9946b.jpg)

  

  [click there to find Code of  Hierarchical Clustering clustering](https://github.com/AlaaSayed164/Unsupervised-ML/blob/main/Hierarchical%20Clustering_Lab.ipynb)

 ## 3. Apply previous Algorithms on Credit Card Fraud Detection Dataset  :
 
 1. we started by cleanning  dataset :

>>this was ower own project for  you can finded here https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud
