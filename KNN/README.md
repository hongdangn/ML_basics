## KNN for classification
$\star$ Data representation:
  - Each observation is represented by a vector in a $n$ - dimensional space, e.g, $x_i =$ { $x_{i1}, x_{i2},...,x_{in}$ }. Each dimension represents an attribute/feature/variate.
  - There is a set C of pre - defined labels.
    
$\star$ Learning phase:
  - Simply save all the training data $D$, with the labels.
    
$\star$ Prediction (For a new instance $z$):
  - For each instance $x$ in $D$, compute the distance/similarity between $x$ and $z$.
  - Determine a set $NB(z)$ of the nearest neighbors of $z$.
  - Using majority labels in $NB(z)$ to predict the label of $z$.

## KNN for regression
$\star$ Data representation:
  - Each observation is represented by a vector in a $n$ - dimensional space, e.g, $x_i =$ { $x_{i1}, x_{i2},...,x_{in}$ }. Each dimension represents an attribute/feature/variate.
  - The output $y$ is a real number.
    
$\star$ Learning phase:
  - Simply save all the training data $D$, with the labels.
    
$\star$ Prediction (For a new instance $z$):
  - For each instance $x$ in $D$, compute the distance/similarity between $x$ and $z$.
  - Determine a set $NB(z)$ of the nearest neighbors of $z$, with $NB(z) == k$.
  - Predict the label of $z$: $y_z = \dfrac{1}{k} \displaystyle \sum \limits_{x \in NB(z)} y_x$.
