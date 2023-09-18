## Classification problem
$\star$ Data representation:
- Each observation is represented by n attributes/features, e.g., $x_i =$ $[x_{i1}, x_{i2},..., x_{in}]^T$.
- Each attribute is nominal/categorical, i.e., represents names, labels or categories, e.g., $x_{i1} \in$ { $high, normal$ } and $x_{i2} \in$ { $male, female, other$ }.
- There is a set C of pre - defined labels.

$\star$ We have to learn a function from a training dataset: $D =$ { $(x_1, y_1), (x_2, y_2),..., (x_m, y_m)$ }. 

## Tree representation
$\star$ Each internal node represents an attribute for testing incoming data.

$\star$ Each branch/subtree of a node corresponds to a value of the attribute of that node.

$\star$ Each leaf node represents a class label.

$\star$ Once a tree has been learned, we can predict the label for a new instance by using its attributes to travel from root to leaf and the label of leaf will be used to assign to the new instance.

## Learning a decision tree by ID3 (Iteractive Dichotomiser 3)
$\star$ At each node N, select a test attribute A which can help us best do classification for the data N.
- Generate the branch for each value of A, and then separate the data into its branches accordingly.

$\star$ Grow the tree until:
- It classifies correctly all the training data or all attributes are used.
