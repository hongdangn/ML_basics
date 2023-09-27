## Random forest (RF)

$\star$ Main idea:
- Prediction based on combination of many decision trees, by taking the average of all individual prediction.
- Each tree in RF is simple but random.
- Each tree is grown differently, depending on the choices of the attributes and training data.


$\star$ RF algorithm:
- Input: training data $D$.
- Learning: grow K trees as follows
  + Generate a training set $D_i$ by sampling with replacement from D.
  + Learn the $i^{th}$ tree from $D_i$:
    + At each node:
      + Select randomly a subset S of atttributes.
      + Split node into subtrees according to S.
    + Grow this tree upto its largest size without prunning.
- Prediction: taking the average of all predictions from individual tree.
