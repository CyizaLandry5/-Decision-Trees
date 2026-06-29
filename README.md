# Assignment : Decision Trees

## Assignment Information

- **Student Name:** Mpayimana Cyiza Landry
- **Assignment Title:** Practice Lab: Decision Trees
- **Platform:** Stanford University - Machine Learning Specialization
- **Course:** Supervised Machine Learning: Regression and Classification

---

## Assignment Overview

In this Assignment, I implemented a decision tree classifier to classify mushrooms as edible or poisonous based on their physical attributes. The assignment involved building fundamental components of a decision tree algorithm using Python and NumPy.

---

## What I Learned

### 1. **Decision Tree Fundamentals**
- Understood the concept of decision trees as a supervised learning algorithm
- Learned how decision trees make predictions by recursively splitting data based on features
- Understood the importance of choosing the right features for splitting

### 2. **Entropy and Impurity Measures**
- Implemented entropy calculation to measure impurity at a node
- Understood the concept of `p₁` (probability of positive class)
- Learned that entropy is 0 when all examples belong to the same class, and maximum when classes are balanced

### 3. **Information Gain**
- Implemented information gain calculation to evaluate the quality of a split
- Learned the formula: `Information Gain = H(node) - weighted entropy of children`
- Understood that higher information gain indicates a better split

### 4. **Data Splitting**
- Implemented function to split dataset into left and right branches based on a feature value
- Learned to work with one-hot encoded features for binary splits

### 5. **Tree Building Algorithm**
- Implemented the recursive process of building a decision tree
- Understood stopping criteria (maximum depth)
- Learned how to select the best feature at each node

---

## What I Accomplished

### ✅ Implemented Core Functions

1. **`compute_entropy(y)`**
   - Calculated entropy at a given node
   - Handled edge cases (empty arrays, pure nodes)

2. **`split_dataset(X, node_indices, feature)`**
   - Split data into left and right branches based on a feature value
   - Returned indices for both branches

3. **`compute_information_gain(X, y, node_indices, feature)`**
   - Computed information gain from splitting on a feature
   - Used entropy values and branch weights

4. **`get_best_split(X, y, node_indices)`**
   - Determined the best feature to split on
   - Found feature with maximum information gain

### ✅ Built a Decision Tree

- Applied the implemented functions to build a decision tree with maximum depth of 2
- Used the dataset of 10 mushroom examples with 3 features:
  - **Brown Cap** (feature 0)
  - **Tapering Stalk Shape** (feature 1)
  - **Solitary** (feature 2)

### ✅ Achieved Understanding

- Discovered that **Solitary** (feature 2) provides the highest information gain (0.278) at the root node
- Visualized the tree structure and decision-making process
- Understood how the tree classifies mushrooms as edible (1) or poisonous (0)

---

## Dataset Overview

The dataset contains 10 mushroom examples with three features:

| Feature | Description |
|---------|-------------|
| Brown Cap | 1 = Brown, 0 = Red |
| Tapering Stalk Shape | 1 = Tapering, 0 = Enlarging |
| Solitary | 1 = Yes, 0 = No |

**Target variable:**
- 1 = Edible
- 0 = Poisonous

---

## Technical Implementation

### Technologies Used
- **Python 3**
- **NumPy** - for numerical computations
- **Matplotlib** - for visualizations
- **Jupyter Notebook** - for interactive development

