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

**Convergence of K-Means**

> - Recomputation monotonically decreases each square error since (mj is number of members in cluster j):
>
 >       Σ (xi - a)^2 reaches minimum for:
 >             
 >       Σ -2(xi - a) = 0
 >       
 >         Σ xi =  Σ a = mja
 >       
 >      a = 1/mj  Σ xi = cj
 >      
 > - K-Means typically converges quickly.

***Time Complexity of K-Means Clustering***

> - Computing distance between two item is O(n) where n is the dimensionality of the vectors.
>
> - Reassigning clusters: O(km) distance computations, or O(kmn).
> 
> - Computing centroids: Each item gets addedd once to some centroid ; O(mn).
> 
> - Assume these two steps are each done once for t iterations: O(tknm).


**EXAMPLES**

> Suppose we have two variables M1 and M2. The x-y axis scatter plot of these two variables is given below:
> 
> ![kmeans1](https://user-images.githubusercontent.com/107355282/236619834-faa4b53b-764a-4c06-ac82-842c0e0b840c.png)
>
> - Let's take number k of clusters, i.e., K=2, to identify the dataset and to put them into different clusters. It means here we will try to group these datasets into > two different clusters.
> - We need to choose some random k points or centroid to form the cluster. These points can be either the points from the dataset or any other point. So, here we are >    selecting the below two points as k points, which are not the part of our dataset. Consider the below image:
>
>![kmeans](https://user-images.githubusercontent.com/107355282/236620213-b140ca53-a4b8-415d-b048-dea76c333f47.png)
>
> - Now we will assign each data point of the scatter plot to its closest K-point or centroid. We will compute it by applying some mathematics that we have studied to > calculate the distance between two points. So, we will draw a median between both the centroids. Consider the below image:
>  
>![kmeans2](https://user-images.githubusercontent.com/107355282/236620491-8e57f8c8-1a92-479b-a28b-a6165c43e8b9.png)
>
>From the above image, it is clear that points left side of the line is near to the K1 or blue centroid, and points to the right of the line are close to the yellow >centroid. Let's color them as blue and yellow for clear visualization.
>
>From the above image, it is clear that points left side of the line is near to the K1 or blue centroid, and points to the right of the line are close to the yellow >centroid. 

