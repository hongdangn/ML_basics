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

## K - means: Convergence
$\star$ The algorithm converge if one of these things happens:
   - Very few instances are reassigned to new clusters.
   - The centroids don't change significantly.
   - The following sum doesn't change significantly: $Error = \displaystyle \sum \limits^{k}_{i = 1} \sum _{x \in C_i} d(x, m_i)^2$, where $C_i$ is the $i^{th}$ cluster, $m_i$ is the centroid of cluster $C_i$.
