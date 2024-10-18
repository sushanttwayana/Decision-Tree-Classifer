# Decision Tree Classifier

This is a simple implementation of simple Decision Tree classifier from scratch in Python, designed to classify fruits based on their color and diameter. The implementation covers fundamental concepts such as Gini Impurity, Information Gain, and recursive tree-building.
  
## Features

- **Gini Impurity Calculation**: Measures the impurity of a dataset to determine how mixed the classes are.
- **Information Gain**: Calculates the reduction in impurity by splitting the dataset using different features.
- **Decision Tree Construction**: Builds the tree recursively by finding the best splits.
- **Classification**: Classifies new data points by traversing the decision tree.
- **Tree Visualization**: Prints the structure of the decision tree for easy visualization and understanding.

## Dataset

The training dataset consists of fruits categorized by their color and diameter, with labels indicating the type of fruit.

### Training Data

| Color  | Diameter | Label |
|--------|----------|-------|
| Green  | 3        | Mango |
| Yellow | 3        | Mango |
| Red    | 1        | Grape |
| Red    | 1        | Grape |
| Yellow | 3        | Lemon |

### Testing Data

The testing dataset is used to evaluate the classifier's performance.

| Color  | Diameter | Label |
|--------|----------|-------|
| Green  | 3        | Apple |
| Yellow | 4        | Apple |
| Red    | 2        | Grape |
| Red    | 1        | Grape |
| Yellow | 3        | Lemon |



## Output

The tree structure and classification results will be printed in the console.

```bash
Is diameter >= 3?
--> True:
  Is color == Yellow?
  --> True:
    Predict {'Mango': 1, 'Lemon': 1}
  --> False:
    Predict {'Mango': 1}
--> False:
  Predict {'Grape': 2}
```
