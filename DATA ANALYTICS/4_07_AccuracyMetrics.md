# **Metrics Used to Evaluate Accuracy**

Evaluation metrics help measure how well a classification model performs. 
These metrics are derived from the **Confusion Matrix**:

|                     | **Predicted Positive** | **Predicted Negative** |
| ------------------- | ---------------------- | ---------------------- |
| **Actual Positive** | True Positive (TP)     | False Negative (FN)    |
| **Actual Negative** | False Positive (FP)    | True Negative (TN)     |

---

## **1. Accuracy**


```
Accuracy = (TP + TN) / (TP + TN + FP + FN)
```

Measures the percentage of total correct predictions. 



## **2. Precision**


```
Precision = TP / (TP + FP)
```

Shows how many predicted positives are actually positive.


## **3. Recall (Sensitivity)**

```
Recall = TP / (TP + FN)
```
how many actual positives were correctly identified. 


## **4. F1-Score**

```
F1 Score = 2 * (Precision * Recall) / (Precision + Recall)
```



## **5. Specificity** 

```
Specificity = TN / (TN + FP)
```


## **6. Error Rate**



```
Error Rate = (FP + FN) / (TP + TN + FP + FN)
```

Percentage of total incorrect predictions.

---

## **7. ROC Curve & AUC**

### **ROC Curve:**

A plot of **True Positive Rate vs. False Positive Rate** at different thresholds.

### **AUC (Area Under ROC Curve):**

Represents overall model performance.  
Higher AUC → Better model.