
# **## 1. Decision Tree Induction**

A **Decision Tree** is a predictive model that uses a tree-like structure of decisions and outcomes.

---

## **### 1.1 Components**

* **Root Node** → Represents entire dataset
* **Internal Nodes** → Tests on attributes
* **Branches** → Outcomes of tests
* **Leaf Nodes** → Final class labels

---

## **### 1.2 How Decision Trees Are Built (Algorithm Steps)**

1. **Select Attribute to Split**

   * Choose the attribute that best splits the data.
   * Based on:

     * **Information Gain** (Entropy-Based)
     * **Gini Index** (used in CART)
     * **Gain Ratio**

2. **Split the Data**

   * Partition dataset based on attribute values.

3. **Repeat**

   * For each subset, choose best attribute again.
   * Continue until:

     * All samples belong to one class OR
     * No attribute remains OR
     * Node has too few samples.

4. **Stop and Assign Class Label**

   * Most common class becomes the leaf node’s label.

---

## **### 1.3 Advantages**

* Easy to understand & interpret
* Can handle numeric and categorical data
* No feature scaling required
* Fast and non-parametric

---

## **### 1.4 Disadvantages**

* Can overfit
* Unstable (small data change → big tree change)
* Greedy approach (locally optimal splits)

---

---

# **## 2. Bayes Classification Methods**

Bayesian classification uses **probabilities** to predict class labels.
Based on **Bayes’ Theorem**:

### **P(A | B) = [ P(B | A) × P(A) ] / P(B)**

---

## **### 2.1 Naïve Bayes Classifier**

A simple yet powerful classifier.

### **Assumption:**

All features are **independent** given the class. (Often false, but still works well)

---

## **### 2.2 Types of Naïve Bayes**

* **Gaussian NB** → continuous features
* **Multinomial NB** → text data, word counts
* **Bernoulli NB** → binary features

---

## **### 2.3 Advantages**

* Very fast training
* Works well with small data
* Performs great with text (spam detection, sentiment analysis)

## **### 2.4 Disadvantages**

* Assumes independence (not always true)
* Zero-frequency problem (solved via Laplace smoothing)

---

---

# **## 3. Rule-Based Classification**

Classification using **IF–THEN rules**.

---

## **### 3.1 Rule Structure**

```
IF <condition1> AND <condition2> THEN Class = C
```

Example:

```
IF age > 18 AND income > 50k THEN Class = Premium Customer
```

---

## **### 3.2 Rule Generation**

1. **From Decision Trees**

   * Each path = one rule.

2. **Rule Induction Algorithms**

   * RIPPER
   * CN2
   * PART

3. **Expert-defined Rules**

   * Manual rules written by domain experts.

---

## **### 3.3 Advantages**

* Human-readable
* Easy to modify
* Good for business usage

---

## **### 3.4 Disadvantages**

* Hard to maintain many rules
* Rules may conflict
* Not suitable for continuous data without preprocessing

---

---

# **## 4. Model Evaluation and Selection**

Evaluating how good the model performs on **unseen data**.

---

## **### 4.1 Train–Test Split**

* Split dataset:

  * **Training Set**: Build model
  * **Test Set**: Evaluate model

---

## **### 4.2 Cross-Validation (k-fold)**

* Data is split into *k* parts
* Train on k-1 folds
* Test on remaining 1 fold
* Repeat k times
* Average performance = final score

More stable & unbiased.

---

---

# **## 5. Metrics for Evaluating Classifier Performance**

---

## **### 5.1 Confusion Matrix**

|                 | Predicted Positive | Predicted Negative |
| --------------- | ------------------ | ------------------ |
| Actual Positive | TP                 | FN                 |
| Actual Negative | FP                 | TN                 |

---

## **### 5.2 Accuracy**

```
Accuracy = (TP + TN) / (TP + TN + FP + FN)
```

---

## **### 5.3 Precision**

```
Precision = TP / (TP + FP)
```

How many predicted positives are actually correct?

---

## **### 5.4 Recall (Sensitivity)**

```
Recall = TP / (TP + FN)
```

Out of all actual positives, how many predicted correctly?

---

## **### 5.5 F1-Score**

```
F1 = 2 * (Precision * Recall) / (Precision + Recall)
```

---

## **### 5.6 Specificity**

```
Specificity = TN / (TN + FP)
```

---

## **### 5.7 ROC Curve**

* Plots True Positive Rate vs False Positive Rate

## **### 5.8 AUC**

* Area under ROC curve
* Higher AUC → better classifier

---

---

# **## 6. Training Bayesian Belief Networks (BBN)**

A **Bayesian Belief Network** is a graphical model with:

* **Nodes** → Variables
* **Directed Edges** → Dependencies
* **Conditional Probability Tables (CPTs)**

---

## **### 6.1 Learning BBN**

Two tasks:

---

### **1. Structure Learning**

Find graph structure:

* Which node depends on which
* Use heuristics, score-based methods, or constraint-based methods

---

### **2. Parameter Learning**

Estimate probabilities in CPT:

* Maximum Likelihood
* Bayesian Estimation

---

## **### 6.2 Inference**

Used to compute probability of unknown variables given evidence.

---

## **### 6.3 Applications**

* Medical diagnosis
* Fraud detection
* Weather prediction

---

---

# **## 7. Classification by Backpropagation (Neural Networks)**

Backpropagation trains a **Multi-Layer Neural Network**.

---

## **### 7.1 Process**

### **Step 1: Forward Pass**

* Input → Hidden layers → Output
* Computes predicted value

---

### **Step 2: Compute Error**

```
Error = Actual - Predicted
```

---

### **Step 3: Backward Pass**

* Calculate partial derivatives
* Propagate error backwards
* Update weights using gradient descent

---

### **Step 4: Repeat**

* Iterate until error is minimized
* Called "training epochs"

---

## **### 7.2 Activation Functions**

* Sigmoid
* ReLU
* Tanh
* Softmax

---

## **### 7.3 Advantages**

* Can model complex patterns
* Works great with large datasets

## **### 7.4 Disadvantages**

* Slow training
* Requires high computation
* Can overfit

---
# **### 8.1 Case 1: Data is Linearly Separable**

SVM finds a **hyperplane** that perfectly separates classes.

---

## **### Max-Margin Principle**

* Margin = distance between hyperplane & the nearest points
* Nearest points = **Support Vectors**

SVM chooses the hyperplane with **maximum margin**
→ best generalization.

---

## **### Equation of Hyperplane**

```
w·x + b = 0
```

---

## **### Advantages**

* Excellent accuracy
* Robust to outliers
* Works well for high-dimensional data

---

---

# **### 8.2 Case 2: Data is Linearly Inseparable**

Data cannot be separated by a straight line.

Solution:

## **👉 Use Kernel Trick**

Maps data to higher dimension where separation becomes possible.

---

## **### Common Kernels**

* **Linear Kernel**
* **Polynomial Kernel**
* **RBF (Gaussian) Kernel**
* **Sigmoid Kernel**

---

## **### Soft Margin SVM**

Allows some misclassification to avoid overfitting.

---

## **### Advantages**

* Handles complex data
* Flexible through kernels

---

## **### Disadvantages**

* Choosing right kernel is difficult
* Slow for large datasets

---
