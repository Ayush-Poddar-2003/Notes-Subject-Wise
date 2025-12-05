# Market Basket Analysis ?
- Data Mining technique, to identify relationships b/w produts,being purchased together in transaction.  
- Based on **Association rule mining**
- To find frequent itemsets & generate association rules.
- By analyzing purchasing behavior businesses can  optimize product placement, improve cross-selling opportunities, design effective promotions, and manage inventory
---
## <center> METRICS TO UNDERSTAND FURTHER
**1. SUPPORT ?**  
Higher support → more frequent.
>**Support(X) = (Transactions containing X) / (Total transactions)**  

**2. CONFIDENCE ?**  
How often Y is bought when X is bought.      
>**Confidence(X⇒Y) = Support(X∪Y) / Support(X)** 



**3. LIFT ?**  
Measures strength of rule.  
>**Lift = Confidence(X⇒Y)/Support(Y)**   

    Lift > 1 = Strong association  
    Lift = 1 = No association  
    Lift < 1 = Negative association

---
### Frequent Itemsets ?
  
>Itemsets with **support ≥ minimum support threshold**

---
### Closed Itemsets

A frequent itemset is closed if, **no superset has the same support**.


{milk, bread} appears 10 times  
{milk, bread, butter} also appears 10 times  
So {milk, bread} is NOT closed.

Closed itemsets are useful to reduce number of patterns.

---
### 