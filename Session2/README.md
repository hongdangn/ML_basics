## K - means for clustering
$\star$ Data representation: $D =$ \{ $x_1, x_2,..., x_r$ \}, each $x_i$ is a vector n - dimensional Euclidean space.

$\star$ K - means partitions D into K clusters:
   - Each cluster has a central point which is called centroid.
   - K is the pre-specified constant.

## K - means: Main steps
$\star$ Input: training data D, number K of clusters, and distance measure $d(x, y)$.

$\star$ Initialization: select randomly K instances in D as the initial centroids.

$\star$ Repeat the following two steps until convergence:
  - Step 1: For each instance, assign it to the cluster with the nearest centroid.
  - Step 2: For each cluster, recompute its centroid from all the instances assign to that cluster.
