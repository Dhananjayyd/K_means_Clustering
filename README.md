# K_means_Clustering

>K-means clustering is a popular unsupervised machine learning algorithm used to group data points into clusters based on their similarity. The algorithm works by >iteratively assigning each data point to one of K clusters based on their proximity to the cluster centroid, which is the mean of all the points in the cluster.

**ALGORITHM**

>Step 1: Randomly selecti K initial centroids, which can be any data point in the dataset.

>Step 2: For each data point, it calculates its distance to each centroid and assigns it to the cluster with the closest centroid.

>Step 3: After all data points have been assigned to a cluster, 
>the algorithm recalculates the centroid of each cluster as the mean of all the data points in that cluster. 

>Step 4: The process of assigning points to clusters and updating centroids is repeated until the centroids no longer change or 
> a maximum number of iterations is reached.

**Stopping/Convergence criterion**

> We can stop when there is:
>
>i. no re-assignments of data points to different clusters.
>
>ii. no (or minimum) change of Centroids.
>
>iii. minimum decreased in the sum of squared error,
>                     
>             SSE =  Σ   Σ || xi - ui||^2 
>                    
  
**Similarity/Distance measure**
  
-**Distance metric(Scale dependent)**

> --minkowski family of distance measure
>                 
> d(xi , xj) = (  Σ |xis - xjs|^p)^1/p
>                 
>
 > Manhattan (p = 1), Euclidean (p = 2)              
                 
**EXAMPLES**


